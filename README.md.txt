# ДЗ: Docker и микросервисная архитектура

## Dockerfile

Смотри отдельный файл `Dockerfile` в этой папке.

## Лог сборки образа

```text
[+] Building 263.7s (10/10) FINISHED                                                               docker:desktop-linux
 => [internal] load build definition from Dockerfile                                                               0.0s
 => => transferring dockerfile: 204B                                                                               0.0s
 => [internal] load metadata for docker.io/continuumio/miniconda3:latest                                           1.6s
 => [internal] load .dockerignore                                                                                  0.0s
 => => transferring context: 2B                                                                                    0.0s
 => [1/5] FROM docker.io/continuumio/miniconda3:latest@sha256:eca594d684f495c1a02beff33a9fab53aec8c5830eaf431bb14  0.1s
 => => resolve docker.io/continuumio/miniconda3:latest@sha256:eca594d684f495c1a02beff33a9fab53aec8c5830eaf431bb14  0.1s
 => [internal] load build context                                                                                  0.0s
 => => transferring context: 25B                                                                                   0.0s
 => CACHED [2/5] WORKDIR /app                                                                                      0.0s
 => CACHED [3/5] COPY 1.sh /app/1.sh                                                                                 0.0s
 => CACHED [4/5] RUN chmod +x /app/1.sh                                                                             0.0s
 => [5/5] RUN pip install --no-cache-dir mlflow boto3 pymysql                                                    136.3s
 => exporting to image                                                                                           125.2s
 => => exporting layers                                                                                           73.8s
 => => exporting manifest sha256:5ada8f5640aca44942df3e5a00e0334a0acb7b22c222428be9465d5cd5584706                  0.0s
 => => exporting config sha256:5a21d23a0fbb5027db657f1f3e29d7f00eeb917b7bc1ca9c64234b9325f4211d                    0.0s
 => => exporting attestation manifest sha256:bf807c903179a41f942631632b1c5449a1a2ae58597d68a04cc638d6edac1099      0.1s
 => => exporting manifest list sha256:d444fe73a9f232758d9d735c26b312449905bcb24afc6922bc794025636aea14             0.0s
 => => naming to docker.io/library/netology-ml:netology-ml                                                         0.0s
 => => unpacking to docker.io/library/netology-ml:netology-ml                                                     51.1s
