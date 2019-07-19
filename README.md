# scrap_us_proxy

* Using scrapy to scrap ip and port from us-proxy.org
* Using scrapy-splash to navigate all pages
## sample output
```json
[
    {
        "ip": "192.241.142.123",
        "port": "8080"
    },
    {
        "ip": "165.227.105.81",
        "port": "3128"
    },
    {
        "ip": "134.209.1.204",
        "port": "8080"
    }
]
```

## Run

```sh
$ cd scrap_us_proxy
$ docker run -p 8050:8050 scrapinghub/splash
$ scrapy crawl usproxy -o txt.json
```

or run in docker-compose

```sh
$  docker-compose up --build
```
