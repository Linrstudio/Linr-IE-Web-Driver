# Linr IE Web Driver

* IE 原生 Web Driver 调用，通过简单配置，即可自动化测试 IE 浏览器。做一些自动化的操作，都是很容易的。如快速登录、抢票等。

### 下载 download （请选择您对应的 IE 版本）
 
* 请在 [Download](https://github.com/Linrstudio/Linr-IE-Web-Driver/raw/master/download/Linr-IE-Web-Driver-for-IE11.zip 'Download') 下载 for IE11
* 请在 [Download](https://github.com/Linrstudio/Linr-IE-Web-Driver/raw/master/download/Linr-IE-Web-Driver-v1.0.zip 'Download') 下载 for IE Developer Channel

** IE11 用户提示：
* 您需要下载安装 WebDriver library http://go.microsoft.com/fwlink/p/?LinkID=510280

### 操作方法 How to (for IE 11)

* 双击 LinrIEWebDriver.exe （默认使用 config.json 这个配置文件）
* 将配置文件 xxx.json 拖到 LinrIEWebDriver.exe 运行，则使用 xxx.json 作为配置文件

*** config.json 文件示例

    {
    	"newSession":[],
    	"get":"http://bing.com",
    	"wait":20,
    	"maximizeWindow":{},
    	"takeScreenshot":"^^^"
    }

*** config-lite.json 文件示例

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


### 操作方法 How to (for IE Developer Channel)

* 开始-运行-cmd
* 粘贴或输入 格式：LinrIEWebDriver.exe xxx.json /appvve:9BD02EED-6C11-4FF0-8A3E-0B4733EE86A1_6A0357B5-AB99-4856-8A59-CF2C38579E78
* 如：LinrIEWebDriver.exe config.json /appvve:9BD02EED-6C11-4FF0-8A3E-0B4733EE86A1_6A0357B5-AB99-4856-8A59-CF2C38579E78

### 系统要求 system requred:

* Windows 7/8 + IE11
或
* Windows 7/8 + Internet Explorer Developer Channel (http://devchannel.modern.ie/ 下载)

## Web Driver 命令 JSON 参考：

* http://msdn.microsoft.com/en-us/library/ie/dn800898(v=vs.85).aspx for IE11
* http://msdn.microsoft.com/en-us/library/ie/dn722336(v=vs.85).aspx for IE Developer Channel