# Linr IE Web Driver

* IE 原生 Web Driver 调用，通过简单配置，即可自动化测试 IE 浏览器（目前仅限 Internet Explorer Developer Channel 版本）。做一些自动化的操作，都是很容易的。如快速登录、抢票等。

### 下载 download

请在 [Download](https://github.com/Linrstudio/Linr-IE-Web-Driver/raw/master/download/Linr-IE-Web-Driver-v1.1.zip 'Download') 下载

** 目前仅支持 Internet Explorer Developer Channel 版本（x64, x86）。

### 操作方法 How to

* 开始-运行-cmd
* 粘贴或输入 格式：LinrIEWebDriver.exe xxx.json /appvve:9BD02EED-6C11-4FF0-8A3E-0B4733EE86A1_6A0357B5-AB99-4856-8A59-CF2C38579E78
* 如：LinrIEWebDriver.exe config.json /appvve:9BD02EED-6C11-4FF0-8A3E-0B4733EE86A1_6A0357B5-AB99-4856-8A59-CF2C38579E78

### 系统要求 system requred:

* Windows 7/8 + Internet Explorer Developer Channel (http://devchannel.modern.ie/ 下载)


### 参考配置

* 打开 bing 输入 WebDriver，截屏并弹出 123 提示 config.json：
<pre>
{
	"newSession":[],
	"get":"http://bing.com",
	"wait":20,
	"maximizeWindow":{},
	"findElement":"input[name=q]",
	"sendKeys":["W", "e", "b", "D", "r", "i", "v", "e", "r", "\uE007"],
	"executeScript":"alert(1)",
	"takeScreenshot":"",
	"executeScript(script, args)" : ['alert(arguments[0])', ["123"]]
}
</pre>

## Web Driver 命令 JSON 参考：
http://msdn.microsoft.com/en-us/library/ie/dn722336(v=vs.85).aspx