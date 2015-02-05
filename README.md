# browser-notepad

##浏览器编辑器

###使用方法

打开浏览器，然后将下面的代码输入进地址栏即可。

##最简单朴素的浏览器-编辑器：

浏览器地址栏输入以下内容：

 data:text/html, <html contenteditable>

##支持各种编程语言的编辑器

浏览器地址栏输入以下内容：

data:text/html, <style type="text/css">.e{position:absolute;top:0;right:0;bottom:0;left:0;}</style><div class="e"         id="editor"></div><script src="http://d1n0x3qji82z53.cloudfront.net/src-min-noconflict/ace.js" type="text/javascript"   charset="utf-8"></script><script>var e=ace.edit("editor");e.setTheme("ace/theme/monokai");e.getSession().setMode("ace/mode/ruby");</script>


For other language: Instead of  `ace/mode/ruby`, Use

Markdown -> `ace/mode/markdown`
Python -> `ace/mode/python`
C/C++ -> `ace/mode/c_cpp`
Javscript -> `ace/mode/javascript`
Java -> `ace/mode/java`
Scala- -> `ace/mode/scala`
CoffeeScript -> `ace/mode/coffee`
and 
css, html, php, latex, 
tex, sh, sql, lua, clojure, dart, typescript, go, groovy, json, jsp, less, lisp, 
lucene, perl, powershell, scss, textile, xml, yaml, xquery, liquid, diff and many more...



##想换个主题



For other theme: Instead of  `ace/theme/monokai`, Use

Eclipse -> ace/theme/eclipse
GitHub -> ace/theme/github
TextMate -> ace/theme/textmate
and 
ambiance, dawn, chaos, chrome, dreamweaver, xcode, vibrant_ink, solarized_dark, solarized_light, tomorrow, tomorrow_night, tomorrow_night_blue, 
twilight, tomorrow_night_eighties, pastel_on_dark and many more..

 
 ##想在浏览器编辑Markdown
 
<!-- If you want a markdown converter use this : !-->
data:text/html,<style type="text/css">.e{position:absolute;top:0;right:50%;bottom:0;left:0;} .c{position:absolute;overflow:auto;top:0;right:0;bottom:0;left:50%;}</style><div class="e" id="editor"></div><div class="c"></div><script src="http://d1n0x3qji82z53.cloudfront.net/src-min-noconflict/ace.js" type="text/javascript" charset="utf-8"></script><script src="http://cdnjs.cloudflare.com/ajax/libs/showdown/0.3.1/showdown.min.js"></script><script> function showResult(e){consoleEl.innerHTML=e}var e=ace.edit("editor");e.setTheme("ace/theme/monokai");e.getSession().setMode("ace/mode/markdown");var consoleEl=document.getElementsByClassName("c")[0];var converter=new Showdown.converter;e.commands.addCommand({name:"markdown",bindKey:{win:"Ctrl-M",mac:"Command-M"},exec:function(t){var n=e.getSession().getMode().$id;if(n=="ace/mode/markdown"){showResult(converter.makeHtml(t.getValue()))}},readOnly:true})</script>
<!-- Press Ctrl+M or Command+M to convert your markdown code to html :) -->


作者链接：<https://gist.github.com/jdkanani/4670615>
