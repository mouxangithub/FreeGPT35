[![Docker Pulls][1]](https://hub.docker.com/r/missuo/freegpt35)

[1]: https://img.shields.io/docker/pulls/missuo/freegpt35?logo=docker

使用第三方接口免登3.5转v1，例如[cockroachai-v2](https://github.com/cockroachai/cockroachai-v2)

项目源自[FreeGPT35](https://github.com/missuo/FreeGPT35)，本项目只是更改了chatgpt的基础路径和域名，解决一些因为国内机器无法使用的问题


### 使用蟑螂v2基础域名进行免登3.5转v1

```bash
docker run -d \
 -p 3040:3040 \
 -e BASE_URL=http://127.0.0.1/ \
 -e API_PATH="/backend-anon/conversation" \
 ghcr.io/mouxan/freegpt35
```

```bash
docker run -d \
 -p 3040:3040 \
 -e BASE_URL=http://127.0.0.1/ \
 -e API_PATH="/backend-anon/conversation" \
 mouxan/freegpt35
```
