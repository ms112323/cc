# 環境設定
DockerのBuile
docker build --platform=linux/amd64 -t c-compiler .

Dockerの起動
docker run --platform=linux/amd64 -it --rm -v ~/Documents/git/cc:/cc -w /cc c-compiler /bin/bash

テストの実行
docker run --platform=linux/amd64 --rm -v ~/Documents/git/cc:/cc -w /cc/compiler c-compiler make test
