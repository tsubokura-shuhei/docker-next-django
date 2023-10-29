以下のサンプル docker 構築の手順（コマンド入力手順）
（例）Next.js、Django
（Git:ファイル保存場所）

①【イメージの初期構築】
docker-compose build

②【フロント\_NEXT】
docker-compose run --rm next npx create-next-app tmp --ts\ && mv ./next/tmp/_ ./next && mv ./next/tmp/._ ./next

Rm -r ./next/tmp

③【バックエンド\_Django】
cd django

docker-compose run django django-admin startproject backend .

④【イメージの完成構築】
docker-compose build --no-cache

docker-compose up -d
