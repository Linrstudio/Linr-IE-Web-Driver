# Linr IE Web Driver

* IE ԭ�� Web Driver ���ã�ͨ�������ã������Զ������� IE �������Ŀǰ���� Internet Explorer Developer Channel �汾������һЩ�Զ����Ĳ��������Ǻ����׵ġ�����ٵ�¼����Ʊ�ȡ�

### ���� download

���� [Download](https://github.com/Linrstudio/Linr-IE-Web-Driver/raw/master/download/Linr-IE-Web-Driver-v1.1.zip 'Download') ����

** Ŀǰ��֧�� Internet Explorer Developer Channel �汾��x64, x86����

### �������� How to

* ��ʼ-����-cmd
* ճ�������� ��ʽ��LinrIEWebDriver.exe xxx.json /appvve:9BD02EED-6C11-4FF0-8A3E-0B4733EE86A1_6A0357B5-AB99-4856-8A59-CF2C38579E78
* �磺LinrIEWebDriver.exe config.json /appvve:9BD02EED-6C11-4FF0-8A3E-0B4733EE86A1_6A0357B5-AB99-4856-8A59-CF2C38579E78

### ϵͳҪ�� system requred:

* Windows 7/8 + Internet Explorer Developer Channel (http://devchannel.modern.ie/ ����)


### �ο�����

* �� bing ���� WebDriver������������ 123 ��ʾ config.json��

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

## Web Driver ���� JSON �ο���
http://msdn.microsoft.com/en-us/library/ie/dn722336(v=vs.85).aspx