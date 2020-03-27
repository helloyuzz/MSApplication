# MSApplication
基于C#实现，.NET ClickOnce自动更新

**签证书**
```javascript
根证书：
makecert -r -pe -n "CN=LogicHealth CSSD Root " -sv LogicHealth_root.pvk LogicHealth_root.cer

应用证书：
makecert -n "CN=LogicHealth CSSD" -pe 
         -iv d:\clickonce\LogicHealth_rooot.pvk 
         -ic d:\clickonce\LogicHealth_root.cer 
         -sky exchange -ss My

Pwd:
cssd123
```

MageUI.exe
修改部署文件中的部署地址，并对exe文件重新签名。

适合快速跨服务器部署，可用于单机编译，不依赖IP地址，实现多服务器部署。
