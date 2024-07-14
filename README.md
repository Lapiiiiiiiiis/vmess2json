# VmessUtils

VmessUtils consist of a bundle of python scripts that works with vmess:// format and the subscription.

Formerly named vmess2json, is one of the scripts in the project.

* [vmess2json](https://github.com/boypt/vmess2json/wiki/vmess2json) - parses `vmess://` to client side json config.
* [json2vmess](https://github.com/boypt/vmess2json/wiki/json2vmess) - parses server side json to `vmess://`
* [vmesseditor](https://github.com/boypt/vmess2json/wiki/vmesseditor) - editor for a `vmess://` or a subscription
* [vmesssed](https://github.com/boypt/vmess2json/wiki/vmesssed) - editor for `vmess://` subscription, like `sed` command works for batch job
* [vmessviewer](https://github.com/boypt/vmess2json/wiki/vmessviewer) - viewer for `vmess://` or subscription


```sh
cat ./ghelper_proxy | ./vmess2json.py --select 1 > v2ray_config.json
vim v2ray_config.json # delete error message
V2RAY_LOCATION_ASSET=/etc/v2ray v2ray -config v2ray_config.json > /dev/null 2>&1 &
export http_proxy=http://127.0.0.1:8123; export https_proxy=http://127.0.0.1:8123; export all_proxy=socks5://127.0.0.1:8123
```
