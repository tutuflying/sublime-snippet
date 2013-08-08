---
layout: default
title: 2013-08-08-sublimeText2配置
---
<h1>{{ page.title }}</h1>
<h2>安装package control组件</h2>
<p>1.调出console</p>
<pre>
	<code>Ctrl+`</code>	
</pre>
<p>2.粘贴以下代码到底部命令行并回车</p>
<pre>
	<code>import urllib2,os;pf='Package Control.sublime-package';ipp=sublime.installed_packages_path();os.makedirs(ipp) if not os.path.exists(ipp) else None;open(os.path.join(ipp,pf),'wb').write(urllib2.urlopen('http://sublime.wbond.net/'+pf.replace(' ','%20')).read())</code>
</pre>
<h2>常用插件</h2>
<p>...</p>
<h2>自定义snippet</h2>
<p>con->console.log();</p>
<pre>
	<code><snippet>
	<content><![CDATA[
console.log(${1});
]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	<tabTrigger>con</tabTrigger>
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<scope></scope>
</snippet></code>
</pre>
<p>al->alert();</p>
<pre>
	<code><snippet>
	<content><![CDATA[
alert(${1});
]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	<tabTrigger>al</tabTrigger>
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<scope></scope>
</snippet></code>
</pre>
<p>seajs快捷键</p>
<pre>
	<code><snippet>
	<content><![CDATA[
define(function(require, exports, module){
	${1:/*code*/}
});
]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	<tabTrigger>sdef</tabTrigger>
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<scope>source.js</scope>
</snippet></code>
</pre>
<p>seajs快捷键</p>
<pre>
	<code><snippet>
	<content><![CDATA[
var ${1} = require("${2}");
]]></content>
	<!-- Optional: Set a tabTrigger to define how to trigger the snippet -->
	<tabTrigger>sre</tabTrigger>
	<!-- Optional: Set a scope to limit where the snippet will trigger -->
	<scope>source.js</scope>
</snippet></code>
</pre>
