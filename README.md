
#ルートディレクトリで以下のコマンドを実行
databricks bundle init ./template -p DAB --config-file tmp_config.json --output-dir project

cd project
databricks bundle validate

databricks bundle deploy -t dev -p DAB

