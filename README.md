# CollectProduct

Android 产物收集

- 支持收集apk,并支持重命名
- 支持收集aab,并支持重命名
- 收集`mapping.txt`
- 收集`usage.txt`
- 收集`seeds.txt`
- 收集`R.txt`
- 收集`configuration.txt`
- 支持AGP 8.0+
- 支持AGP 8.0-

# 使用方式

在`apply`脚本之前, 先配置产物名称:

```
ext {
    APP_NAME = "CollectProduct"
    apkName = "#an-#vn_#fn_#bn_#ka"
}

//可用参数: #an:app名字APP_NAME; #vn:版本名; #d:当天日期yyyy-MM-dd; #t:当天时间yyyy-MM-dd_HH-mm; #fn:风味名; #bn:编译类型名;
//         #sn:使用的签名名称; #ka:使用的签名别名;
```

在工程的`build.gradle`中加入脚本:

## 国内

```gradle
apply from: 'https://gitee.com/angcyo/CollectProduct/raw/master/app/collectProduct.gradle'
```

## 国外

```gradle
apply from: 'https://raw.githubusercontent.com/angcyo/CollectProduct/master/app/collectProduct.gradle'
```

# 参数配置

在`gradle.properties`文件中配置产物输出目录, 默认为根目录下的`.apk`文件夹:

```
apk_path='.apk'
```

---
**群内有`各(pian)种(ni)各(jin)样(qun)`的大佬,等你来撩.**

# 联系作者

[点此QQ对话](http://wpa.qq.com/msgrd?v=3&uin=664738095&site=qq&menu=yes)  `该死的空格`    [点此快速加群](https://shang.qq.com/wpa/qunwpa?idkey=cbcf9a42faf2fe730b51004d33ac70863617e6999fce7daf43231f3cf2997460)

[开源地址](https://github.com/angcyo/CollectProduct)

![扫码进群](https://raw.githubusercontent.com/angcyo/res/master/code/all_in1.jpg)

![给点鼓励](https://raw.githubusercontent.com/angcyo/res/master/code/all_in2.jpg)

## 访问统计
<img height="30px" src = "https://profile-counter.glitch.me/CollectProduct/count.svg" alt ="Loading">
