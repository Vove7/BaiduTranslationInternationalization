
# Android Studio string.xml一键翻译

- 优化 (' & 空格)等特殊字符
- 支持自定义 百度翻译 appid
- 支持 string-array

下载：[InternationalizationTranslation.zip](InternationalizationTranslation.zip)

**某些格式化字符需要检查修改**

#### 使用方法

在 string.xml 文件右键选择 `Convert to other languages`

#### 翻译效果

- 原文件

```xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
    <string name="listen_one">接听率: %.2f</string>
    <string name="last_login_time">最后登录:&#160;</string>
    <string name="can_use_gold">可用金币: %d</string>
    <string name="test1">¥ 123 \'&#160;</string>
    <string-array name="weeks">
        <item>周一</item>
        <item>周二</item>
        <item>周三</item>
        <item>周四</item>
        <item>周五</item>
        <item>周六</item>
        <item>周日</item>
    </string-array>
</resources>
```

- English

```xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
	<string name="listen_one">Response rate:%. 2F</string>
	<string name="last_login_time">Last login:&nbsp;</string>
	<string name="can_use_gold">Available gold coins% d</string>
	<string name="test1">¥ 123 \' &nbsp;</string>
	<string-array name="weeks">
		<item>Monday</item>
		<item>Tuesday</item>
		<item>Wednesday</item>
		<item>Thursday</item>
		<item>Friday</item>
		<item>Saturday</item>
		<item>Sunday</item>
	</string-array>
</resources>
```

- 繁体
```xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
	<string name="listen_one">接聽率：%.2f</string>
	<string name="last_login_time">最後登錄： &nbsp;</string>
	<string name="can_use_gold">可用金幣：%d</string>
	<string name="test1">¥123 \' &nbsp;</string>
	<string-array name="weeks">
		<item>週一</item>
		<item>週二</item>
		<item>週三</item>
		<item>週四</item>
		<item>週五</item>
		<item>週六</item>
		<item>周日</item>
	</string-array>
</resources>
```

- 日文
```xml
<?xml version="1.0" encoding="utf-8"?>
<resources>
	<string name="listen_one">受信率:%2 f</string>
	<string name="last_login_time">最終ログイン:&nbsp;</string>
	<string name="can_use_gold">使用可能な金貨:%d</string>
	<string name="test1">¥123&nbsp;</string>
	<string-array name="weeks">
		<item>月曜日</item>
		<item>火曜日</item>
		<item>水曜日</item>
		<item>木曜日</item>
		<item>金曜日</item>
		<item>土曜日</item>
		<item>日曜日</item>
	</string-array>
</resources>

```




> ﻿BaiduTranslationInternationalization
> ====
> 一款AndroidStudio插件，使用该插件，可以快速生成28种语言的string.xml文件
> 
> 
> 最近做一款打印机App，因为主要是销向国外，所以需要国际化。
> 作为一款偷懒的程序员，叫我一个一个去网站翻译，那是不可能的，如果程序员没有一颗偷懒的心，那还叫程序员么？
> 
> 在网上百度，找到一款插件，叫做AndroidLocalizationer。但是这款插件早在两年前就已经停止维护，下载下来安装进去，也没有办法进行使用了。
> 
> 继续百度，又找到了一款，是后来有人在AndroidLocalizationer的基础上更改的。主要是关于翻译方式的更改。结果还是没有办法使用，阅读源码，发现作者是采用谷歌翻译Api就是翻译的。debug，发现作者的key已经过期了。
> 
> 上面两款插件，在我们中国，需要翻墙。不仅仅需要翻墙，还只能是英文翻译成其他语言。也就是说，如果你是中文的软件，想要国际化，还是需要一个一个翻译成英文。这是不能忍的，因为需要App很多所谓的国际化，其实就是多增加了一个英文版本。我TM要你何用？
> 
> 于是我决定把翻译接口改了。注册了百度翻译的一个账号，把接口更换过来，第一是不用翻墙了。第二支持中文翻译成其他语言了。
> 
> 需要说明的一点：我只是往百度翻译冲了50块钱，所以用完即完了，纯粹当做一次探索，下次我要再次使用的时候，就继续冲得了。所以，如果你从现在（2017/12/08）之后不久去使用，应该是可行的。但是如果时间隔了太久，百度翻译钱用完了，也就没办法使用的。
> 
> [https://github.com/westlinkin/AndroidLocalizationer](https://github.com/westlinkin/AndroidLocalizationer "具体操作")