# 用于Cobaltstrike流量分析的工具：

## 1768_v0_0_16
用于提取 Cobalt Strike Beacon 的配置信息

Eg：`python3 1768.py stagebeaconname`

原项目地址：[1768_v0_0_16](https://blog.didierstevens.com/2022/08/27/update-1768-py-version-0-0-16/)

## cs-decrypt-metadata_V0_0_1
用于使用通用密钥或指定密钥元数据解密

Eg：`python3 cs-decrypt-metadata.py -p privetakey encryptedmetadata`

Eg: `python3 cs-decrypt-metadata.py -f .cobaltstrike.beaconkey encryptedmetadata`

原项目地址：[cs-decrypt-metadata_V0_0_1](https://blog.didierstevens.com/2021/10/22/new-tool-cs-decrypt-metadata-py/)

## cs-parse-http-traffic
使用元数据中的密钥(对称密钥)解密pacp流量

Eg：``python3 cs-parse-http-traffic.py -r Rawkey -Y "wireshark filter command" file.pcap ``

Eg：`python3 cs-parse-http-traffic.py -r b555de5dce3b9e3eb4b5722f6aa6bc85 -Y "http && ip.addr==192.168.132.128" demo.pcapng -o res.txt`

原项目地址：[cs-parse-http-traffic](https://blog.didierstevens.com/2021/11/29/new-tool-cs-parse-traffic-py/)
