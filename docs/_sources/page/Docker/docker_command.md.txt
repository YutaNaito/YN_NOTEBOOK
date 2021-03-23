# Dockerコマンド

- 起動中のコンテナを表示
  - `docker ps`

- 起動中、停止中全てのコンテナを表示
  - `docker ps -a`

- 起動中のコンテナを停止
  - `docker stop <CONTAINER ID>`

- コンテナの削除
  - `docker rm <CONTAINER ID>`

- コンテナに入る
  - `docker exec -i -t <CONTAINER ID> bash`

- コンテナのネットワークを表示
  - `docker network ls`

- ネットワークの詳細を表示
  - `docker network inspect <NAME>`