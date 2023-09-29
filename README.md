# SW関門2023用リポジトリ
## webapp : docker+Flask+uwsgi+postgre
### ローカル環境(今井) : windows11のWSL2(Ubuntu) 
### 本番環境(今井) : さくらVPS Ubuntu22.04
#### link : [http://49.212.166.39:8080](http://49.212.166.39:8080/ "ホームページ")

### dockerコマンドメモ
- イメージ作成  
```bash
docker compose build --no-cache
```
- コンテナ起動(バックグラウンド)
```bash
docker compose up -d
```
- 指定したコンテナの中に入る
```bash
docker exec -it {コンテナID/名} bash
```
- コンテナの中から出る  
Ctrl + P + Q

- コンテナ・ネットワーク削除
```bash
docker compose down
```
- コンテナ停止
```bash
docker comopse stop
```
- 停止中のコンテナ起動
```bash
docker comopse start
```
- コンテナ再起動
```bash
docker comopse restart
```
- イメージ削除
```bash
docker image rm {イメージID}
```
- イメージ削除(全て)
```bash
docker image rm $(docker images -q)
```