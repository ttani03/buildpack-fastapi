# buildpack-fastapi

## 準備

- [Docker のインストール](https://docs.docker.com/get-docker/)
- [pack コマンドのインストール](https://buildpacks.io/docs/tools/pack/)

## 使い方

コンテナイメージのビルド

```
pack build buildpack-fastapi --builder paketobuildpacks/builder:base
```

イメージの実行

```
docker run --rm -d -p 8000:8000 buildpack-fastapi
```

動作確認

```
curl localhost:8000/hello/
```

## Tilt との連携

Tilt の起動

```
tilt up
```

Tilt の停止
```
tilt down
```
