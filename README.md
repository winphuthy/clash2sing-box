[中文(zh-cn)](README_CN.md) | English  

## Converting Supports  
- [x]  Shadowsocks  
- [x]  http  
- [x]  socks  
- [x]  VMess  
- [x]  Trojan  
- [x]  Hysteria  
- [ ]  ~~ShadowTLS~~      `Clash.Meta` not support `Shadow-tls` yet  
- [x]  ShadowsocksR     
- [ ]  ~~VLESS~~          `VLESS` had been abandoned officially. See [detail](https://www.v2fly.org/v5/config/proxy/vless.html)  

> to parse clash subscribe link and generate pretty-printed indented minimal avaliable sing-box profile  
```console
./clash2sing-box --subscribe "<URL>" -g -f -o ./config.json
```  

> to parse clash subscribe link  
```console  
./clash2sing-box --subscribe "<URL>"  
```

> to parse clash `config.yaml`  
```console
./clash2sing-box --path <PATH TO config.yaml>  
```   

> converting clash profile to minimal sing-box profile  
```console
./clash2sing-box --path <PATH TO config.yaml> -g -f -o ./config.json   
```

```console
> ./clash2sing-box --help
Usage: clash2sing-box [OPTIONS]

Options:
  -p, --path <PATH>        Read path of clash format config.yaml file
  -s, --subscribe <URL>    Get clash subscription profile by url
  -f                       Output pretty-printed indented JSON
  -g, --gen-profile        Generate minimal avaliable sing-box JSON profile
  -o, --output <PATH>      Output sing-box JSON profile
  -h, --help               Print help information
  -V, --version            Print version information
```

### Credits
+ [Clash](https://github.com/Dreamacro/clash)  
+ [Clash.Meta](https://github.com/MetaCubeX/Clash.Meta)  
+ [sing-box](https://github.com/SagerNet/sing-box)  
+ [json_value_merge](https://github.com/jmfiaschi/json_value_merge)
