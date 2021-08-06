# Introduction
git clone https://github.com/airbytehq/airbyte.git
cd airbyte
docker-compose up
copy source-book from this repo to ->
airbyte/airbyte-integrations/connectors/
docker build . -t airbyte/source-book:dev
docker run --rm -i airbyte/source-book:dev spec
