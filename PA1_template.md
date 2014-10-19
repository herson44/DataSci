<!DOCTYPE html>
<!-- saved from url=(0014)about:internet -->
<html>
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8"/>
<meta http-equiv="x-ua-compatible" content="IE=9" >

<title>Assigment 1  </title>

<style type="text/css">
body, td {
   font-family: sans-serif;
   background-color: white;
   font-size: 12px;
   margin: 8px;
}

tt, code, pre {
   font-family: 'DejaVu Sans Mono', 'Droid Sans Mono', 'Lucida Console', Consolas, Monaco, monospace;
}

h1 { 
   font-size:2.2em; 
}

h2 { 
   font-size:1.8em; 
}

h3 { 
   font-size:1.4em; 
}

h4 { 
   font-size:1.0em; 
}

h5 { 
   font-size:0.9em; 
}

h6 { 
   font-size:0.8em; 
}

a:visited {
   color: rgb(50%, 0%, 50%);
}

pre {	
   margin-top: 0;
   max-width: 95%;
   border: 1px solid #ccc;
   white-space: pre-wrap;
}

pre code {
   display: block; padding: 0.5em;
}

code.r, code.cpp {
   background-color: #F8F8F8;
}

table, td, th {
  border: none;
}

blockquote {
   color:#666666;
   margin:0;
   padding-left: 1em;
   border-left: 0.5em #EEE solid;
}

hr {
   height: 0px;
   border-bottom: none;
   border-top-width: thin;
   border-top-style: dotted;
   border-top-color: #999999;
}

@media print {
   * { 
      background: transparent !important; 
      color: black !important; 
      filter:none !important; 
      -ms-filter: none !important; 
   }

   body { 
      font-size:12pt; 
      max-width:100%; 
   }
       
   a, a:visited { 
      text-decoration: underline; 
   }

   hr { 
      visibility: hidden;
      page-break-before: always;
   }

   pre, blockquote { 
      padding-right: 1em; 
      page-break-inside: avoid; 
   }

   tr, img { 
      page-break-inside: avoid; 
   }

   img { 
      max-width: 100% !important; 
   }

   @page :left { 
      margin: 15mm 20mm 15mm 10mm; 
   }
     
   @page :right { 
      margin: 15mm 10mm 15mm 20mm; 
   }

   p, h2, h3 { 
      orphans: 3; widows: 3; 
   }

   h2, h3 { 
      page-break-after: avoid; 
   }
}

</style>

<!-- Styles for R syntax highlighter -->
<style type="text/css">
   pre .operator,
   pre .paren {
     color: rgb(104, 118, 135)
   }

   pre .literal {
     color: rgb(88, 72, 246)
   }

   pre .number {
     color: rgb(0, 0, 205);
   }

   pre .comment {
     color: rgb(76, 136, 107);
   }

   pre .keyword {
     color: rgb(0, 0, 255);
   }

   pre .identifier {
     color: rgb(0, 0, 0);
   }

   pre .string {
     color: rgb(3, 106, 7);
   }
</style>

<!-- R syntax highlighter -->
<script type="text/javascript">
var hljs=new function(){function m(p){return p.replace(/&/gm,"&amp;").replace(/</gm,"&lt;")}function f(r,q,p){return RegExp(q,"m"+(r.cI?"i":"")+(p?"g":""))}function b(r){for(var p=0;p<r.childNodes.length;p++){var q=r.childNodes[p];if(q.nodeName=="CODE"){return q}if(!(q.nodeType==3&&q.nodeValue.match(/\s+/))){break}}}function h(t,s){var p="";for(var r=0;r<t.childNodes.length;r++){if(t.childNodes[r].nodeType==3){var q=t.childNodes[r].nodeValue;if(s){q=q.replace(/\n/g,"")}p+=q}else{if(t.childNodes[r].nodeName=="BR"){p+="\n"}else{p+=h(t.childNodes[r])}}}if(/MSIE [678]/.test(navigator.userAgent)){p=p.replace(/\r/g,"\n")}return p}function a(s){var r=s.className.split(/\s+/);r=r.concat(s.parentNode.className.split(/\s+/));for(var q=0;q<r.length;q++){var p=r[q].replace(/^language-/,"");if(e[p]){return p}}}function c(q){var p=[];(function(s,t){for(var r=0;r<s.childNodes.length;r++){if(s.childNodes[r].nodeType==3){t+=s.childNodes[r].nodeValue.length}else{if(s.childNodes[r].nodeName=="BR"){t+=1}else{if(s.childNodes[r].nodeType==1){p.push({event:"start",offset:t,node:s.childNodes[r]});t=arguments.callee(s.childNodes[r],t);p.push({event:"stop",offset:t,node:s.childNodes[r]})}}}}return t})(q,0);return p}function k(y,w,x){var q=0;var z="";var s=[];function u(){if(y.length&&w.length){if(y[0].offset!=w[0].offset){return(y[0].offset<w[0].offset)?y:w}else{return w[0].event=="start"?y:w}}else{return y.length?y:w}}function t(D){var A="<"+D.nodeName.toLowerCase();for(var B=0;B<D.attributes.length;B++){var C=D.attributes[B];A+=" "+C.nodeName.toLowerCase();if(C.value!==undefined&&C.value!==false&&C.value!==null){A+='="'+m(C.value)+'"'}}return A+">"}while(y.length||w.length){var v=u().splice(0,1)[0];z+=m(x.substr(q,v.offset-q));q=v.offset;if(v.event=="start"){z+=t(v.node);s.push(v.node)}else{if(v.event=="stop"){var p,r=s.length;do{r--;p=s[r];z+=("</"+p.nodeName.toLowerCase()+">")}while(p!=v.node);s.splice(r,1);while(r<s.length){z+=t(s[r]);r++}}}}return z+m(x.substr(q))}function j(){function q(x,y,v){if(x.compiled){return}var u;var s=[];if(x.k){x.lR=f(y,x.l||hljs.IR,true);for(var w in x.k){if(!x.k.hasOwnProperty(w)){continue}if(x.k[w] instanceof Object){u=x.k[w]}else{u=x.k;w="keyword"}for(var r in u){if(!u.hasOwnProperty(r)){continue}x.k[r]=[w,u[r]];s.push(r)}}}if(!v){if(x.bWK){x.b="\\b("+s.join("|")+")\\s"}x.bR=f(y,x.b?x.b:"\\B|\\b");if(!x.e&&!x.eW){x.e="\\B|\\b"}if(x.e){x.eR=f(y,x.e)}}if(x.i){x.iR=f(y,x.i)}if(x.r===undefined){x.r=1}if(!x.c){x.c=[]}x.compiled=true;for(var t=0;t<x.c.length;t++){if(x.c[t]=="self"){x.c[t]=x}q(x.c[t],y,false)}if(x.starts){q(x.starts,y,false)}}for(var p in e){if(!e.hasOwnProperty(p)){continue}q(e[p].dM,e[p],true)}}function d(B,C){if(!j.called){j();j.called=true}function q(r,M){for(var L=0;L<M.c.length;L++){if((M.c[L].bR.exec(r)||[null])[0]==r){return M.c[L]}}}function v(L,r){if(D[L].e&&D[L].eR.test(r)){return 1}if(D[L].eW){var M=v(L-1,r);return M?M+1:0}return 0}function w(r,L){return L.i&&L.iR.test(r)}function K(N,O){var M=[];for(var L=0;L<N.c.length;L++){M.push(N.c[L].b)}var r=D.length-1;do{if(D[r].e){M.push(D[r].e)}r--}while(D[r+1].eW);if(N.i){M.push(N.i)}return f(O,M.join("|"),true)}function p(M,L){var N=D[D.length-1];if(!N.t){N.t=K(N,E)}N.t.lastIndex=L;var r=N.t.exec(M);return r?[M.substr(L,r.index-L),r[0],false]:[M.substr(L),"",true]}function z(N,r){var L=E.cI?r[0].toLowerCase():r[0];var M=N.k[L];if(M&&M instanceof Array){return M}return false}function F(L,P){L=m(L);if(!P.k){return L}var r="";var O=0;P.lR.lastIndex=0;var M=P.lR.exec(L);while(M){r+=L.substr(O,M.index-O);var N=z(P,M);if(N){x+=N[1];r+='<span class="'+N[0]+'">'+M[0]+"</span>"}else{r+=M[0]}O=P.lR.lastIndex;M=P.lR.exec(L)}return r+L.substr(O,L.length-O)}function J(L,M){if(M.sL&&e[M.sL]){var r=d(M.sL,L);x+=r.keyword_count;return r.value}else{return F(L,M)}}function I(M,r){var L=M.cN?'<span class="'+M.cN+'">':"";if(M.rB){y+=L;M.buffer=""}else{if(M.eB){y+=m(r)+L;M.buffer=""}else{y+=L;M.buffer=r}}D.push(M);A+=M.r}function G(N,M,Q){var R=D[D.length-1];if(Q){y+=J(R.buffer+N,R);return false}var P=q(M,R);if(P){y+=J(R.buffer+N,R);I(P,M);return P.rB}var L=v(D.length-1,M);if(L){var O=R.cN?"</span>":"";if(R.rE){y+=J(R.buffer+N,R)+O}else{if(R.eE){y+=J(R.buffer+N,R)+O+m(M)}else{y+=J(R.buffer+N+M,R)+O}}while(L>1){O=D[D.length-2].cN?"</span>":"";y+=O;L--;D.length--}var r=D[D.length-1];D.length--;D[D.length-1].buffer="";if(r.starts){I(r.starts,"")}return R.rE}if(w(M,R)){throw"Illegal"}}var E=e[B];var D=[E.dM];var A=0;var x=0;var y="";try{var s,u=0;E.dM.buffer="";do{s=p(C,u);var t=G(s[0],s[1],s[2]);u+=s[0].length;if(!t){u+=s[1].length}}while(!s[2]);if(D.length>1){throw"Illegal"}return{r:A,keyword_count:x,value:y}}catch(H){if(H=="Illegal"){return{r:0,keyword_count:0,value:m(C)}}else{throw H}}}function g(t){var p={keyword_count:0,r:0,value:m(t)};var r=p;for(var q in e){if(!e.hasOwnProperty(q)){continue}var s=d(q,t);s.language=q;if(s.keyword_count+s.r>r.keyword_count+r.r){r=s}if(s.keyword_count+s.r>p.keyword_count+p.r){r=p;p=s}}if(r.language){p.second_best=r}return p}function i(r,q,p){if(q){r=r.replace(/^((<[^>]+>|\t)+)/gm,function(t,w,v,u){return w.replace(/\t/g,q)})}if(p){r=r.replace(/\n/g,"<br>")}return r}function n(t,w,r){var x=h(t,r);var v=a(t);var y,s;if(v){y=d(v,x)}else{return}var q=c(t);if(q.length){s=document.createElement("pre");s.innerHTML=y.value;y.value=k(q,c(s),x)}y.value=i(y.value,w,r);var u=t.className;if(!u.match("(\\s|^)(language-)?"+v+"(\\s|$)")){u=u?(u+" "+v):v}if(/MSIE [678]/.test(navigator.userAgent)&&t.tagName=="CODE"&&t.parentNode.tagName=="PRE"){s=t.parentNode;var p=document.createElement("div");p.innerHTML="<pre><code>"+y.value+"</code></pre>";t=p.firstChild.firstChild;p.firstChild.cN=s.cN;s.parentNode.replaceChild(p.firstChild,s)}else{t.innerHTML=y.value}t.className=u;t.result={language:v,kw:y.keyword_count,re:y.r};if(y.second_best){t.second_best={language:y.second_best.language,kw:y.second_best.keyword_count,re:y.second_best.r}}}function o(){if(o.called){return}o.called=true;var r=document.getElementsByTagName("pre");for(var p=0;p<r.length;p++){var q=b(r[p]);if(q){n(q,hljs.tabReplace)}}}function l(){if(window.addEventListener){window.addEventListener("DOMContentLoaded",o,false);window.addEventListener("load",o,false)}else{if(window.attachEvent){window.attachEvent("onload",o)}else{window.onload=o}}}var e={};this.LANGUAGES=e;this.highlight=d;this.highlightAuto=g;this.fixMarkup=i;this.highlightBlock=n;this.initHighlighting=o;this.initHighlightingOnLoad=l;this.IR="[a-zA-Z][a-zA-Z0-9_]*";this.UIR="[a-zA-Z_][a-zA-Z0-9_]*";this.NR="\\b\\d+(\\.\\d+)?";this.CNR="\\b(0[xX][a-fA-F0-9]+|(\\d+(\\.\\d*)?|\\.\\d+)([eE][-+]?\\d+)?)";this.BNR="\\b(0b[01]+)";this.RSR="!|!=|!==|%|%=|&|&&|&=|\\*|\\*=|\\+|\\+=|,|\\.|-|-=|/|/=|:|;|<|<<|<<=|<=|=|==|===|>|>=|>>|>>=|>>>|>>>=|\\?|\\[|\\{|\\(|\\^|\\^=|\\||\\|=|\\|\\||~";this.ER="(?![\\s\\S])";this.BE={b:"\\\\.",r:0};this.ASM={cN:"string",b:"'",e:"'",i:"\\n",c:[this.BE],r:0};this.QSM={cN:"string",b:'"',e:'"',i:"\\n",c:[this.BE],r:0};this.CLCM={cN:"comment",b:"//",e:"$"};this.CBLCLM={cN:"comment",b:"/\\*",e:"\\*/"};this.HCM={cN:"comment",b:"#",e:"$"};this.NM={cN:"number",b:this.NR,r:0};this.CNM={cN:"number",b:this.CNR,r:0};this.BNM={cN:"number",b:this.BNR,r:0};this.inherit=function(r,s){var p={};for(var q in r){p[q]=r[q]}if(s){for(var q in s){p[q]=s[q]}}return p}}();hljs.LANGUAGES.cpp=function(){var a={keyword:{"false":1,"int":1,"float":1,"while":1,"private":1,"char":1,"catch":1,"export":1,virtual:1,operator:2,sizeof:2,dynamic_cast:2,typedef:2,const_cast:2,"const":1,struct:1,"for":1,static_cast:2,union:1,namespace:1,unsigned:1,"long":1,"throw":1,"volatile":2,"static":1,"protected":1,bool:1,template:1,mutable:1,"if":1,"public":1,friend:2,"do":1,"return":1,"goto":1,auto:1,"void":2,"enum":1,"else":1,"break":1,"new":1,extern:1,using:1,"true":1,"class":1,asm:1,"case":1,typeid:1,"short":1,reinterpret_cast:2,"default":1,"double":1,register:1,explicit:1,signed:1,typename:1,"try":1,"this":1,"switch":1,"continue":1,wchar_t:1,inline:1,"delete":1,alignof:1,char16_t:1,char32_t:1,constexpr:1,decltype:1,noexcept:1,nullptr:1,static_assert:1,thread_local:1,restrict:1,_Bool:1,complex:1},built_in:{std:1,string:1,cin:1,cout:1,cerr:1,clog:1,stringstream:1,istringstream:1,ostringstream:1,auto_ptr:1,deque:1,list:1,queue:1,stack:1,vector:1,map:1,set:1,bitset:1,multiset:1,multimap:1,unordered_set:1,unordered_map:1,unordered_multiset:1,unordered_multimap:1,array:1,shared_ptr:1}};return{dM:{k:a,i:"</",c:[hljs.CLCM,hljs.CBLCLM,hljs.QSM,{cN:"string",b:"'\\\\?.",e:"'",i:"."},{cN:"number",b:"\\b(\\d+(\\.\\d*)?|\\.\\d+)(u|U|l|L|ul|UL|f|F)"},hljs.CNM,{cN:"preprocessor",b:"#",e:"$"},{cN:"stl_container",b:"\\b(deque|list|queue|stack|vector|map|set|bitset|multiset|multimap|unordered_map|unordered_set|unordered_multiset|unordered_multimap|array)\\s*<",e:">",k:a,r:10,c:["self"]}]}}}();hljs.LANGUAGES.r={dM:{c:[hljs.HCM,{cN:"number",b:"\\b0[xX][0-9a-fA-F]+[Li]?\\b",e:hljs.IMMEDIATE_RE,r:0},{cN:"number",b:"\\b\\d+(?:[eE][+\\-]?\\d*)?L\\b",e:hljs.IMMEDIATE_RE,r:0},{cN:"number",b:"\\b\\d+\\.(?!\\d)(?:i\\b)?",e:hljs.IMMEDIATE_RE,r:1},{cN:"number",b:"\\b\\d+(?:\\.\\d*)?(?:[eE][+\\-]?\\d*)?i?\\b",e:hljs.IMMEDIATE_RE,r:0},{cN:"number",b:"\\.\\d+(?:[eE][+\\-]?\\d*)?i?\\b",e:hljs.IMMEDIATE_RE,r:1},{cN:"keyword",b:"(?:tryCatch|library|setGeneric|setGroupGeneric)\\b",e:hljs.IMMEDIATE_RE,r:10},{cN:"keyword",b:"\\.\\.\\.",e:hljs.IMMEDIATE_RE,r:10},{cN:"keyword",b:"\\.\\.\\d+(?![\\w.])",e:hljs.IMMEDIATE_RE,r:10},{cN:"keyword",b:"\\b(?:function)",e:hljs.IMMEDIATE_RE,r:2},{cN:"keyword",b:"(?:if|in|break|next|repeat|else|for|return|switch|while|try|stop|warning|require|attach|detach|source|setMethod|setClass)\\b",e:hljs.IMMEDIATE_RE,r:1},{cN:"literal",b:"(?:NA|NA_integer_|NA_real_|NA_character_|NA_complex_)\\b",e:hljs.IMMEDIATE_RE,r:10},{cN:"literal",b:"(?:NULL|TRUE|FALSE|T|F|Inf|NaN)\\b",e:hljs.IMMEDIATE_RE,r:1},{cN:"identifier",b:"[a-zA-Z.][a-zA-Z0-9._]*\\b",e:hljs.IMMEDIATE_RE,r:0},{cN:"operator",b:"<\\-(?!\\s*\\d)",e:hljs.IMMEDIATE_RE,r:2},{cN:"operator",b:"\\->|<\\-",e:hljs.IMMEDIATE_RE,r:1},{cN:"operator",b:"%%|~",e:hljs.IMMEDIATE_RE},{cN:"operator",b:">=|<=|==|!=|\\|\\||&&|=|\\+|\\-|\\*|/|\\^|>|<|!|&|\\||\\$|:",e:hljs.IMMEDIATE_RE,r:0},{cN:"operator",b:"%",e:"%",i:"\\n",r:1},{cN:"identifier",b:"`",e:"`",r:0},{cN:"string",b:'"',e:'"',c:[hljs.BE],r:0},{cN:"string",b:"'",e:"'",c:[hljs.BE],r:0},{cN:"paren",b:"[[({\\])}]",e:hljs.IMMEDIATE_RE,r:0}]}};
hljs.initHighlightingOnLoad();
</script>




</head>

<body>
<h1>Assigment 1  </h1>

<p>This is a R markdown in my computer for assigment 1</p>

<p>Loading and preprocessing the data</p>

<pre><code class="r">Data_Raw &lt;- read.csv(&quot;activity.csv&quot;, header=TRUE)
Data_Clean &lt;- Data_Raw[which(Data_Raw$steps != &quot;NA&quot;), ]
library(plyr)
Data_day &lt;- ddply(Data_Clean, .(date), summarise, steps=sum(steps))
</code></pre>

<p>What is mean total number of steps taken per day?</p>

<p>a. Histogram of Steps per day</p>

<pre><code class="r">hist(Data_day$steps, main=&quot;Number of Steps&quot;, 
     xlab=&quot;Total number of steps taken each day&quot;, col=&quot;blue&quot;)
</code></pre>

<p><img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAfgAAAH4CAMAAACR9g9NAAAAolBMVEX9/v0AAAAAACoAAFQAAP8AKioAKlQAKn8AVX8AVakqAAAqACoqAFQqKgAqKlQqKn8qVakqf38qf9NUAABUACpUAFRUKgBUKn9UVQBUVSpUVVRUqalUqf1/KgB/Kip/KlR/VQB/fyp/f1R/qX9/1Kl/1NN/1P2pVQCpVSqpqVSp1H+p/tOp/v3TfyrT1H/T/qnT/v39qVT91H/9/qn9/tP9/v0g9zfRAAAANnRSTlP//////////////////////////////////////////////////////////////////////wChj04xAAAACXBIWXMAAAsSAAALEgHS3X78AAAQeElEQVR4nO2dDXviuBVG10nbLOm0mYXZz8JMvza029CGr///12rZMpjJJXCRJVu+5zzPDImNX6x7kGwIRt/swSTf9L0D0A+INwrijYJ4oyDeKIg3CuKNgnijIN4oiDcK4o2CeKMg3iiINwrijYJ4oyDeKIg3CuKNgnijIN4oiDcK4o2CeKMg3ihjE7+dFfP9fre4fxFXn11xwuaxuHtu4oqH1/KH5bzDnRwCIxRfigoUvyzmh7SSSWvJaBih+GJa+a0cb2cPr+vi20Vx/7IqSnnlwn/7Plz+Xg8Odz83/dstchsX/i5l13943c7u/7Oo9R82cSHuGVQODcU1z6QBMj7x9z/V0lviG9zC6odS67L64URzvWhyIr7q6bta/Mkm7i71gFDfNTdGKP63x+lX4u9fnMHt7O65dDbdux9cX/YDg+vLjs1j2fHduuPAXil2XdotaW8yrU4mqiWZMkLxL8u7X0/FT6rF5aD+XB/jS41+GHBL/Di/X1fPgFWpuHVEX9bm3ZLWJi5kVUyrHs9QPwic4e3s27fiH15vEu+He1l8dYxvThAyY4zi3UlYNSDPy5++Ft8e6h1H8cJQv2rO6A9Dfb2JH+qr3zI94R+l+N2iHp7rU6+vxJ+c3NVL/bb+5K7lsurRPmvS2sT/cFidIaMUv3fnc9Uru7+8Heqbl3PL+gnQEu9fzrU7sVPr1pe3/slSn+D5kGZ1hoxNfAquexdo4CBeD+KNgnjIF8QbBfFGQbxREG8UxBsF8UZBvFEQbxTEGwXxRkG8URBvFMQbBfFGQbxREG8UxBsF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" alt="plot of chunk unnamed-chunk-2"/> </p>

<p>b. Calculation of the mean and median total number of steps taken per day</p>

<pre><code class="r">mean(Data_day$steps)
</code></pre>

<pre><code>## [1] 10766.19
</code></pre>

<pre><code class="r">median(Data_day$steps)
</code></pre>

<pre><code>## [1] 10765
</code></pre>

<p>What is the average daily activity pattern?</p>

<p>a. A time series plot (i.e. type = &ldquo;l&rdquo;) of the 5-minute interval (x-axis) and the average number of steps taken, averaged across all days (y-axis)</p>

<pre><code class="r">Average_interval &lt;- ddply(Data_Clean, .(interval), summarise, steps=mean(steps))
plot(Average_interval$interval, Average_interval$steps, type=&quot;l&quot;, 
     col=&quot;Black&quot;,
     xlab=&quot;5-minute Interval&quot;, 
     ylab=&quot;Average Number of Steps Taken&quot;,
     main=&quot;Pattern of Average Activity per Day&quot;)
</code></pre>

<p><img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAfgAAAH4CAMAAACR9g9NAAAAllBMVEX9/v0AAAAAACoAAFQAKioAKlQAKn8AVX8AVakqAAAqACoqAFQqKlQqKn8qVVQqVakqf38qf9NUAABUACpUAFRUKgBUVSpUVVRUqf1/KgB/Kip/KlR/VQB/f1R/f9N/qX9/1NN/1P2pVQCpqVSp1H+p/qmp/tOp/v3TfyrT1H/T/qnT/tPT/v39qVT91H/9/qn9/tP9/v3e3VdUAAAAMnRSTlP/////////////////////////////////////////////////////////////////AA1QmO8AAAAJcEhZcwAACxIAAAsSAdLdfvwAABTxSURBVHic7Z2NmqO2GYWj2XTr6Xab2tm0nk3bZNym427GP9z/zRUJBAgkI4EAwTnvMz82oE+yXktIGPB3GYHku6ULQJaB4kGheFAoHhSKB4XiQaF4UCgeFIoHheJBoXhQKB4UigeF4kGheFAoHhSKB4XiQaF4UCgeFIoHheJBoXhQKB4UigclOfG3g5AcG4tOR/3Hh+uzeHpVj+4vYjeiJJ3keRFuhw9vjaLKJ94Fs7205UhVfOlOcpJVdfKur3rL/C3Q0BRMO7m9CP4F0y9N7IeXKR4Jiv/4Lqtzn12U/7zdCfFH+Sdvfueiwdxfnv4mnn59+fBvUbs5qypVm8sIasnfi/eMbLinTvrXS/kGy9N8+E1le242yDK5CvnhTQXeyUZexcuf/LcoXV6IS+HzXhfKzCzTPcRFqK2L11YnnJt0xRft4+PvDfGnssEUdtUaobvjYt2uIT6v1v8872RN589vh7zuzfTfigze1bPvn/ON9PqsmVytFoViJb6Kp8XvzrngU9FHFVuLRrC6ROV+Iu8jytf23kg4NwmKb3T1qqqqrv4q5chWUux987/7wmom++U8RWm3bLPX551qUnmTe1XbtdLrDK7P+Ubn5nojuVotg8pfuX0Vryqd3jQrC5W/hqMjs0z2BMc66yrh3CQqvuwaVadZib+I8j2hqr4QWnQQslnL2j2XfhTyiarkc+7Ckl5noJLKONV6I3nVFWvxVbxK/P0l7z4Ku4XHfItOZqb4IutGwrlJUHy5h87HVqJHfL7SLf5e7Qnybb4dyh1rI73OwC6+Sn6pdyalax2v7o/OT78878tce8Wf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" alt="plot of chunk unnamed-chunk-4"/> </p>

<p>b. Which 5-minute interval, on average across all the days in the dataset, contains the maximum number of steps?</p>

<pre><code class="r">Average_interval[Average_interval$steps==max(Average_interval$steps),]
</code></pre>

<pre><code>##     interval    steps
## 104      835 206.1698
</code></pre>

<p>Imputing missing values</p>

<p>a. Reporting total number of missing values in the dataset </p>

<pre><code class="r">sum(is.na(Data_Raw$steps))
</code></pre>

<pre><code>## [1] 2304
</code></pre>

<p>b. Filling  all of the missing values in the dataset. We fill the values with the avarage of the values presented.</p>

<pre><code class="r">colnames(Average_interval)[2] &lt;- &quot;Avg_interval&quot;

Data_missfill &lt;- arrange(join(Data_Raw, Average_interval), interval)
</code></pre>

<pre><code>## Joining by: interval
</code></pre>

<p>c. New dataset that is equal to the original dataset but with the missing data filled in.</p>

<pre><code class="r">Data_missfill$steps[is.na(Data_missfill$steps)] &lt;- Data_missfill$Avg_interval[is.na(Data_missfill$steps)]
</code></pre>

<p>d.1. A histogram of the total number of steps taken each day</p>

<pre><code class="r">New_data_hist &lt;- ddply(Data_missfill, .(date), summarise, steps=sum(steps))
hist(New_data_hist$steps, main=&quot;Number of Steps (missing values fill in)&quot;, 
     xlab=&quot;Total number of steps per day&quot;, col=&quot;blue&quot;,)
</code></pre>

<p><img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAfgAAAH4CAMAAACR9g9NAAAAn1BMVEX9/v0AAAAAACoAAFQAAP8AKioAKlQAKn8AVX8AVakqAAAqACoqAFQqKlQqKn8qVakqf38qf9NUAABUACpUAFRUKgBUKn9UVQBUVSpUVVRUqalUqf1/KgB/Kip/KlR/VQB/fyp/f1R/qX9/1Kl/1NN/1P2pVQCpVSqpqVSp1H+p/qmp/tOp/v3TfyrT/qnT/v39qVT91H/9/qn9/tP9/v1QOkbzAAAANXRSTlP/////////////////////////////////////////////////////////////////////AHy10AoAAAAJcEhZcwAACxIAAAsSAdLdfvwAABFmSURBVHic7Z0Ne9u2FUZLe11qL0smpe3ayc3WNda+rFpf//+3jQBBmoyuTF2BIAnfc54nli2RL4F7BJJSROibI5jkm6kbANOAeKMg3iiINwrijYJ4oyDeKIg3CuKNgnijIN4oiDcK4o2CeKMg3iiINwrijYJ4oyDeKIg3CuKNgnijIN4oiDcK4o0yvfj9slgdj4eH2yfx4bMPdNjdFzePdVzx7rn8Zb3qXWsT1mlacrop6b4zXLCoa+Zv5WL78O9ktd394sKtxTIL8aWoSPHrYtWkldy17nlty3eqlvbG9ba0blRb/FdLXPw8i2QW4ouF9+sd75fvnrfFdw/F7dOmKOtU3vnvMIbLv6udw81P9fh2d7mVi7BIOWTePZcl/d9Dpb9ZxYW4mpZjrqhruykfam/Kq6gXCLfuvpe1yw3d/ndZbWnt8v3PbbmRsj1h0aoLzaZbW6ya+bsw4l+2sC1GGvJzEH/716piLfE17k7/S1nKtf+lo7m6664j3lf7UInvrOIWqXYI1aLlE+jx2N5UpaO7YKWl2kwV8+19tfrWxeyXN4/dRWvx9aZbW3xNfNhCeNKMwCzE/+d+8ZX42ydn0JW1rMnC19eN5bBjKMIuenfvB1r5o9mx+xK6irp72qt4Bavd/UtdfY3bm3IK6gXq26Bl4T3v7svkTfd587JYR3yz6fYWfaP2svhqCxce2QZgFuKf1jdfuuLvQj2c+KAxjE13T31OtvXPALfHbh3R15X5td+PN6u4kE2x8OMvlNYraW+qGfG+GUVrV++fX1W7XsZkGRe26xb+Snyz6fYW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" alt="plot of chunk unnamed-chunk-9"/> </p>

<p>d.2. Report the mean and median total number of steps taken per day</p>

<pre><code class="r">mean(New_data_hist$steps)
</code></pre>

<pre><code>## [1] 10766.19
</code></pre>

<pre><code class="r">median(New_data_hist$steps)
</code></pre>

<pre><code>## [1] 10766.19
</code></pre>

<p>d.3. The impact of imputing missing data on the estimates of the total daily number of steps? (Using sum  as operation of difference)</p>

<pre><code class="r">sum_steps_data &lt;- sum(Data_Clean$steps)
sum_steps_data_missfillin  &lt;- sum(Data_missfill$steps)
total_diff &lt;- sum_steps_data_missfillin -sum_steps_data []
total_diff
</code></pre>

<pre><code>## [1] 86129.51
</code></pre>

<p>Are there differences in activity patterns between weekdays and weekends?</p>

<p>a. New factor variable in the dataset with two levels - &ldquo;weekday&rdquo; and &ldquo;weekend&rdquo; indicating whether a given date is a weekday or weekend day.</p>

<pre><code class="r">week_day &lt;- weekdays(as.Date(Data_missfill$date))
</code></pre>

<pre><code>## Warning in strptime(xx, f &lt;- &quot;%Y-%m-%d&quot;, tz = &quot;GMT&quot;): unable to identify current timezone &#39;H&#39;:
## please set environment variable &#39;TZ&#39;
</code></pre>

<pre><code>## Warning in strptime(xx, f &lt;- &quot;%Y-%m-%d&quot;, tz = &quot;GMT&quot;): unknown timezone
## &#39;localtime&#39;
</code></pre>

<pre><code class="r">data_weekday &lt;- transform(Data_missfill, day=weekdays)
</code></pre>

<pre><code>## Error in data.frame(structure(list(steps = c(1.71698113207547, 0, 0, 47, : arguments imply differing number of rows: 17568, 0
</code></pre>

<pre><code class="r">data__weekday$week &lt;- ifelse(data_weekday$day %in% c(&quot;Saturday&quot;, &quot;Sunday&quot;),&quot;weekend&quot;, &quot;weekday&quot;)
</code></pre>

<pre><code>## Error in match(x, table, nomatch = 0L): objeto &#39;data_weekday&#39; no encontrado
</code></pre>

<pre><code class="r">Average_interval_week &lt;- ddply(data_weekday, .(interval, week), summarise, steps=mean(steps))
</code></pre>

<pre><code>## Error in empty(.data): objeto &#39;data_weekday&#39; no encontrado
</code></pre>

<p>b. panel plot containing a time series plot (i.e. type = &ldquo;l&rdquo;) of the 5-minute interval (x-axis) and the average number of steps taken, averaged across all weekday days or weekend days (y-axis). The plot should look something like the following, which was creating using simulated data:</p>

<pre><code class="r">library(lattice)
xyplot(steps ~ interval | wk, data = Average_interval_week, layout = c(1, 2), type=&quot;l&quot;)
</code></pre>

<pre><code>## Error in eval(substitute(groups), data, environment(x)): objeto &#39;Average_interval_week&#39; no encontrado
</code></pre>

</body>

</html>

