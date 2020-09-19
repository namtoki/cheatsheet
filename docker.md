
image
-----
- docker (image) build
- docker (image) history
  - イメージの生成履歴
- docker (image) import
  - tar archive (docker container export) からイメージを作成
- docker imange inspect
- docker (imange) load
  - tar archive (docker image save) からイメージを作成
- docker imange ls / docker images
- docker imange prune
  - タグがついていなくてコンテナで使われていないイメージを削除する
- docker (image) pull
- docker (image) push
- docker image rm / docker rmi
- docker (image) save
- docker (image) tag

container
---------
- docker (container) attach
  - exec 後はコンテナは停止する
- docker (container) commit
  - コンテナ内部で変更されたファイルを元にイメージを作成する
- docker (container) cp
  - ファイルやフォルダをコンテナとホスト環境の間でコピーする
- docker (container) create
- docker (container) diff
  - コンテナ内部で変更のあったファイルを調べる
- docker (container) exec
  - 実行中のコンテナ内部でコマンドを実行する
  - exec 後もコンテナは停止しない
- docker (container) export
- docker container inspect
- docker (container) kill
- docker (container) logs
- docker container ls / docker ps
- docker (container) pause
- docker (container) port
  - コンテナのポートマッピングを表示する
- docker container prune
- docker (container) rename
- docker (container) restart
- docker (container) rm
- docker (container) run
  - 新しいコンテナでコマンドを実行する
- docker (container) start
- docker (container) stats
  - top コマンドのようなもの
- docker (container) stop
- docker (container) top
  - ps のようなもの
- docker (container) unpause
- docker (container) update
- docker (container) wait

volume
------
- docker volume create
- docker volume inspect
- docker volume ls
- docker volume prune
- docker volume rm

network
-------
- docker network connect
- docker network create
- docker network disconnect
- docker network inspect
- docker network ls
- docker network prune
- docker network rm
