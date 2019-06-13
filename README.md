<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.1//EN"
    "http://www.w3.org/TR/xhtml11/DTD/xhtml11.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en">
<head>
<meta http-equiv="Content-Type" content="application/xhtml+xml; charset=UTF-8" />
<meta name="generator" content="AsciiDoc 8.6.10" />
<title>FAI Guide (Fully Automatic Installation)</title>
<style type="text/css">
/* Shared CSS for AsciiDoc xhtml11 and html5 backends */

/* Default font. */
body {
  font-family: Georgia,serif;
}

/* Title font. */
h1, h2, h3, h4, h5, h6,
div.title, caption.title,
thead, p.table.header,
#toctitle,
#author, #revnumber, #revdate, #revremark,
#footer {
  font-family: Arial,Helvetica,sans-serif;
}

body {
  margin: 1em 5% 1em 5%;
}

a {
  color: blue;
  text-decoration: underline;
}
a:visited {
  color: fuchsia;
}

em {
  font-style: italic;
  color: navy;
}

strong {
  font-weight: bold;
  color: #083194;
}

h1, h2, h3, h4, h5, h6 {
  color: #527bbd;
  margin-top: 1.2em;
  margin-bottom: 0.5em;
  line-height: 1.3;
}

h1, h2, h3 {
  border-bottom: 2px solid silver;
}
h2 {
  padding-top: 0.5em;
}
h3 {
  float: left;
}
h3 + * {
  clear: left;
}
h5 {
  font-size: 1.0em;
}

div.sectionbody {
  margin-left: 0;
}

hr {
  border: 1px solid silver;
}

p {
  margin-top: 0.5em;
  margin-bottom: 0.5em;
}

ul, ol, li > p {
  margin-top: 0;
}
ul > li     { color: #aaa; }
ul > li > * { color: black; }

pre {
  padding: 0;
  margin: 0;
}

#author {
  color: #527bbd;
  font-weight: bold;
  font-size: 1.1em;
}
#email {
}
#revnumber, #revdate, #revremark {
}

#footer {
  font-size: small;
  border-top: 2px solid silver;
  padding-top: 0.5em;
  margin-top: 4.0em;
}
#footer-text {
  float: left;
  padding-bottom: 0.5em;
}
#footer-badges {
  float: right;
  padding-bottom: 0.5em;
}

#preamble {
  margin-top: 1.5em;
  margin-bottom: 1.5em;
}
div.imageblock, div.exampleblock, div.verseblock,
div.quoteblock, div.literalblock, div.listingblock, div.sidebarblock,
div.admonitionblock {
  margin-top: 1.0em;
  margin-bottom: 1.5em;
}
div.admonitionblock {
  margin-top: 2.0em;
  margin-bottom: 2.0em;
  margin-right: 10%;
  color: #606060;
}

div.content { /* Block element content. */
  padding: 0;
}

/* Block element titles. */
div.title, caption.title {
  color: #527bbd;
  font-weight: bold;
  text-align: left;
  margin-top: 1.0em;
  margin-bottom: 0.5em;
}
div.title + * {
  margin-top: 0;
}

td div.title:first-child {
  margin-top: 0.0em;
}
div.content div.title:first-child {
  margin-top: 0.0em;
}
div.content + div.title {
  margin-top: 0.0em;
}

div.sidebarblock > div.content {
  background: #ffffee;
  border: 1px solid #dddddd;
  border-left: 4px solid #f0f0f0;
  padding: 0.5em;
}

div.listingblock > div.content {
  border: 1px solid #dddddd;
  border-left: 5px solid #f0f0f0;
  background: #f8f8f8;
  padding: 0.5em;
}

div.quoteblock, div.verseblock {
  padding-left: 1.0em;
  margin-left: 1.0em;
  margin-right: 10%;
  border-left: 5px solid #f0f0f0;
  color: #777777;
}

div.quoteblock > div.attribution {
  padding-top: 0.5em;
  text-align: right;
}

div.verseblock > pre.content {
  font-family: inherit;
  font-size: inherit;
}
div.verseblock > div.attribution {
  padding-top: 0.75em;
  text-align: left;
}
/* DEPRECATED: Pre version 8.2.7 verse style literal block. */
div.verseblock + div.attribution {
  text-align: left;
}

div.admonitionblock .icon {
  vertical-align: top;
  font-size: 1.1em;
  font-weight: bold;
  text-decoration: underline;
  color: #527bbd;
  padding-right: 0.5em;
}
div.admonitionblock td.content {
  padding-left: 0.5em;
  border-left: 3px solid #dddddd;
}

div.exampleblock > div.content {
  border-left: 3px solid #dddddd;
  padding-left: 0.5em;
}

div.imageblock div.content { padding-left: 0; }
span.image img { border-style: none; }
a.image:visited { color: white; }

dl {
  margin-top: 0.8em;
  margin-bottom: 0.8em;
}
dt {
  margin-top: 0.5em;
  margin-bottom: 0;
  font-style: normal;
  color: navy;
}
dd > *:first-child {
  margin-top: 0.1em;
}

ul, ol {
    list-style-position: outside;
}
ol.arabic {
  list-style-type: decimal;
}
ol.loweralpha {
  list-style-type: lower-alpha;
}
ol.upperalpha {
  list-style-type: upper-alpha;
}
ol.lowerroman {
  list-style-type: lower-roman;
}
ol.upperroman {
  list-style-type: upper-roman;
}

div.compact ul, div.compact ol,
div.compact p, div.compact p,
div.compact div, div.compact div {
  margin-top: 0.1em;
  margin-bottom: 0.1em;
}

tfoot {
  font-weight: bold;
}
td > div.verse {
  white-space: pre;
}

div.hdlist {
  margin-top: 0.8em;
  margin-bottom: 0.8em;
}
div.hdlist tr {
  padding-bottom: 15px;
}
dt.hdlist1.strong, td.hdlist1.strong {
  font-weight: bold;
}
td.hdlist1 {
  vertical-align: top;
  font-style: normal;
  padding-right: 0.8em;
  color: navy;
}
td.hdlist2 {
  vertical-align: top;
}
div.hdlist.compact tr {
  margin: 0;
  padding-bottom: 0;
}

.comment {
  background: yellow;
}

.footnote, .footnoteref {
  font-size: 0.8em;
}

span.footnote, span.footnoteref {
  vertical-align: super;
}

#footnotes {
  margin: 20px 0 20px 0;
  padding: 7px 0 0 0;
}

#footnotes div.footnote {
  margin: 0 0 5px 0;
}

#footnotes hr {
  border: none;
  border-top: 1px solid silver;
  height: 1px;
  text-align: left;
  margin-left: 0;
  width: 20%;
  min-width: 100px;
}

div.colist td {
  padding-right: 0.5em;
  padding-bottom: 0.3em;
  vertical-align: top;
}
div.colist td img {
  margin-top: 0.3em;
}

@media print {
  #footer-badges { display: none; }
}

#toc {
  margin-bottom: 2.5em;
}

#toctitle {
  color: #527bbd;
  font-size: 1.1em;
  font-weight: bold;
  margin-top: 1.0em;
  margin-bottom: 0.1em;
}

div.toclevel1, div.toclevel2, div.toclevel3, div.toclevel4 {
  margin-top: 0;
  margin-bottom: 0;
}
div.toclevel2 {
  margin-left: 2em;
  font-size: 0.9em;
}
div.toclevel3 {
  margin-left: 4em;
  font-size: 0.9em;
}
div.toclevel4 {
  margin-left: 6em;
  font-size: 0.9em;
}

span.aqua { color: aqua; }
span.black { color: black; }
span.blue { color: blue; }
span.fuchsia { color: fuchsia; }
span.gray { color: gray; }
span.green { color: green; }
span.lime { color: lime; }
span.maroon { color: maroon; }
span.navy { color: navy; }
span.olive { color: olive; }
span.purple { color: purple; }
span.red { color: red; }
span.silver { color: silver; }
span.teal { color: teal; }
span.white { color: white; }
span.yellow { color: yellow; }

span.aqua-background { background: aqua; }
span.black-background { background: black; }
span.blue-background { background: blue; }
span.fuchsia-background { background: fuchsia; }
span.gray-background { background: gray; }
span.green-background { background: green; }
span.lime-background { background: lime; }
span.maroon-background { background: maroon; }
span.navy-background { background: navy; }
span.olive-background { background: olive; }
span.purple-background { background: purple; }
span.red-background { background: red; }
span.silver-background { background: silver; }
span.teal-background { background: teal; }
span.white-background { background: white; }
span.yellow-background { background: yellow; }

span.big { font-size: 2em; }
span.small { font-size: 0.6em; }

span.underline { text-decoration: underline; }
span.overline { text-decoration: overline; }
span.line-through { text-decoration: line-through; }


/*
 * xhtml11 specific
 *
 * */

tt {
  font-family: monospace;
  font-size: inherit;
  color: navy;
}

div.tableblock {
  margin-top: 1.0em;
  margin-bottom: 1.5em;
}
div.tableblock > table {
  border: 3px solid #527bbd;
}
thead, p.table.header {
  font-weight: bold;
  color: #527bbd;
}
p.table {
  margin-top: 0;
}
/* Because the table frame attribute is overriden by CSS in most browsers. */
div.tableblock > table[frame="void"] {
  border-style: none;
}
div.tableblock > table[frame="hsides"] {
  border-left-style: none;
  border-right-style: none;
}
div.tableblock > table[frame="vsides"] {
  border-top-style: none;
  border-bottom-style: none;
}


/*
 * html5 specific
 *
 * */

.monospaced {
  font-family: monospace;
  font-size: inherit;
  color: navy;
}

table.tableblock {
  margin-top: 1.0em;
  margin-bottom: 1.5em;
}
thead, p.tableblock.header {
  font-weight: bold;
  color: #527bbd;
}
p.tableblock {
  margin-top: 0;
}
table.tableblock {
  border-width: 3px;
  border-spacing: 0px;
  border-style: solid;
  border-color: #527bbd;
  border-collapse: collapse;
}
th.tableblock, td.tableblock {
  border-width: 1px;
  padding: 4px;
  border-style: solid;
  border-color: #527bbd;
}

table.tableblock.frame-topbot {
  border-left-style: hidden;
  border-right-style: hidden;
}
table.tableblock.frame-sides {
  border-top-style: hidden;
  border-bottom-style: hidden;
}
table.tableblock.frame-none {
  border-style: hidden;
}

th.tableblock.halign-left, td.tableblock.halign-left {
  text-align: left;
}
th.tableblock.halign-center, td.tableblock.halign-center {
  text-align: center;
}
th.tableblock.halign-right, td.tableblock.halign-right {
  text-align: right;
}

th.tableblock.valign-top, td.tableblock.valign-top {
  vertical-align: top;
}
th.tableblock.valign-middle, td.tableblock.valign-middle {
  vertical-align: middle;
}
th.tableblock.valign-bottom, td.tableblock.valign-bottom {
  vertical-align: bottom;
}


/*
 * manpage specific
 *
 * */

body.manpage h1 {
  padding-top: 0.5em;
  padding-bottom: 0.5em;
  border-top: 2px solid silver;
  border-bottom: 2px solid silver;
}
body.manpage h2 {
  border-style: none;
}
body.manpage div.sectionbody {
  margin-left: 3em;
}

@media print {
  body.manpage div#toc { display: none; }
}


/*
 * Theme specific overrides of the preceding (asciidoc.css) CSS.
 *
 */
body {
  font-family: Garamond, Georgia, serif;
  font-size: 17px;
  color: #3E4349;
  line-height: 1.3em;
}
h1, h2, h3, h4, h5, h6,
div.title, caption.title,
thead, p.table.header,
#toctitle,
#author, #revnumber, #revdate, #revremark,
#footer {
  font-family: Garmond, Georgia, serif;
  font-weight: normal;
  border-bottom-width: 0;
  color: #3E4349;
}
div.title, caption.title { color: #596673; font-weight: bold; }
h1 { font-size: 240%; }
h2 { font-size: 180%; }
h3 { font-size: 150%; }
h4 { font-size: 130%; }
h5 { font-size: 115%; }
h6 { font-size: 100%; }
#header h1 { margin-top: 0; }
#toc {
  color: #444444;
  line-height: 1.5;
  padding-top: 1.5em;
}
#toctitle {
  font-size: 20px;
}
#toc a {
    border-bottom: 1px dotted #999999;
    color: #444444 !important;
    text-decoration: none !important;
}
#toc a:hover {
    border-bottom: 1px solid #6D4100;
    color: #6D4100 !important;
    text-decoration: none !important;
}
div.toclevel1 { margin-top: 0.2em; font-size: 16px; }
div.toclevel2 { margin-top: 0.15em; font-size: 14px; }
em, dt, td.hdlist1 { color: black; }
strong { color: #3E4349; }
a { color: #004B6B; text-decoration: none; border-bottom: 1px dotted #004B6B; }
a:visited { color: #615FA0; border-bottom: 1px dotted #615FA0; }
a:hover { color: #6D4100; border-bottom: 1px solid #6D4100; }
div.tableblock > table, table.tableblock { border: 3px solid #E8E8E8; }
th.tableblock, td.tableblock { border: 1px solid #E8E8E8; }
ul > li > * { color: #3E4349; }
pre, tt, .monospaced { font-family: Consolas,Menlo,'Deja Vu Sans Mono','Bitstream Vera Sans Mono',monospace; }
tt, .monospaced { font-size: 0.9em; color: black;
}
div.exampleblock > div.content, div.sidebarblock > div.content, div.listingblock > div.content { border-width: 0 0 0 3px; border-color: #E8E8E8; }
div.verseblock { border-left-width: 0; margin-left: 3em; }
div.quoteblock { border-left-width: 3px; margin-left: 0; margin-right: 0;}
div.admonitionblock td.content { border-left: 3px solid #E8E8E8; }


@media screen {
  body {
    max-width: 50em; /* approximately 80 characters wide */
    margin-left: 16em;
  }

  #toc {
    position: fixed;
    top: 0;
    left: 0;
    bottom: 0;
    width: 13em;
    padding: 0.5em;
    padding-bottom: 1.5em;
    margin: 0;
    overflow: auto;
    border-right: 3px solid #f8f8f8;
    background-color: white;
  }

  #toc .toclevel1 {
    margin-top: 0.5em;
  }

  #toc .toclevel2 {
    margin-top: 0.25em;
    display: list-item;
    color: #aaaaaa;
  }

  #toctitle {
    margin-top: 0.5em;
  }
}
</style>
<script type="text/javascript">
/*<![CDATA[*/
var asciidoc = {  // Namespace.

/////////////////////////////////////////////////////////////////////
// Table Of Contents generator
/////////////////////////////////////////////////////////////////////

/* Author: Mihai Bazon, September 2002
 * http://students.infoiasi.ro/~mishoo
 *
 * Table Of Content generator
 * Version: 0.4
 *
 * Feel free to use this script under the terms of the GNU General Public
 * License, as long as you do not remove or alter this notice.
 */

 /* modified by Troy D. Hanson, September 2006. License: GPL */
 /* modified by Stuart Rackham, 2006, 2009. License: GPL */

// toclevels = 1..4.
toc: function (toclevels) {

  function getText(el) {
    var text = "";
    for (var i = el.firstChild; i != null; i = i.nextSibling) {
      if (i.nodeType == 3 /* Node.TEXT_NODE */) // IE doesn't speak constants.
        text += i.data;
      else if (i.firstChild != null)
        text += getText(i);
    }
    return text;
  }

  function TocEntry(el, text, toclevel) {
    this.element = el;
    this.text = text;
    this.toclevel = toclevel;
  }

  function tocEntries(el, toclevels) {
    var result = new Array;
    var re = new RegExp('[hH]([1-'+(toclevels+1)+'])');
    // Function that scans the DOM tree for header elements (the DOM2
    // nodeIterator API would be a better technique but not supported by all
    // browsers).
    var iterate = function (el) {
      for (var i = el.firstChild; i != null; i = i.nextSibling) {
        if (i.nodeType == 1 /* Node.ELEMENT_NODE */) {
          var mo = re.exec(i.tagName);
          if (mo && (i.getAttribute("class") || i.getAttribute("className")) != "float") {
            result[result.length] = new TocEntry(i, getText(i), mo[1]-1);
          }
          iterate(i);
        }
      }
    }
    iterate(el);
    return result;
  }

  var toc = document.getElementById("toc");
  if (!toc) {
    return;
  }

  // Delete existing TOC entries in case we're reloading the TOC.
  var tocEntriesToRemove = [];
  var i;
  for (i = 0; i < toc.childNodes.length; i++) {
    var entry = toc.childNodes[i];
    if (entry.nodeName.toLowerCase() == 'div'
     && entry.getAttribute("class")
     && entry.getAttribute("class").match(/^toclevel/))
      tocEntriesToRemove.push(entry);
  }
  for (i = 0; i < tocEntriesToRemove.length; i++) {
    toc.removeChild(tocEntriesToRemove[i]);
  }

  // Rebuild TOC entries.
  var entries = tocEntries(document.getElementById("content"), toclevels);
  for (var i = 0; i < entries.length; ++i) {
    var entry = entries[i];
    if (entry.element.id == "")
      entry.element.id = "_toc_" + i;
    var a = document.createElement("a");
    a.href = "#" + entry.element.id;
    a.appendChild(document.createTextNode(entry.text));
    var div = document.createElement("div");
    div.appendChild(a);
    div.className = "toclevel" + entry.toclevel;
    toc.appendChild(div);
  }
  if (entries.length == 0)
    toc.parentNode.removeChild(toc);
},


/////////////////////////////////////////////////////////////////////
// Footnotes generator
/////////////////////////////////////////////////////////////////////

/* Based on footnote generation code from:
 * http://www.brandspankingnew.net/archive/2005/07/format_footnote.html
 */

footnotes: function () {
  // Delete existing footnote entries in case we're reloading the footnodes.
  var i;
  var noteholder = document.getElementById("footnotes");
  if (!noteholder) {
    return;
  }
  var entriesToRemove = [];
  for (i = 0; i < noteholder.childNodes.length; i++) {
    var entry = noteholder.childNodes[i];
    if (entry.nodeName.toLowerCase() == 'div' && entry.getAttribute("class") == "footnote")
      entriesToRemove.push(entry);
  }
  for (i = 0; i < entriesToRemove.length; i++) {
    noteholder.removeChild(entriesToRemove[i]);
  }

  // Rebuild footnote entries.
  var cont = document.getElementById("content");
  var spans = cont.getElementsByTagName("span");
  var refs = {};
  var n = 0;
  for (i=0; i<spans.length; i++) {
    if (spans[i].className == "footnote") {
      n++;
      var note = spans[i].getAttribute("data-note");
      if (!note) {
        // Use [\s\S] in place of . so multi-line matches work.
        // Because JavaScript has no s (dotall) regex flag.
        note = spans[i].innerHTML.match(/\s*\[([\s\S]*)]\s*/)[1];
        spans[i].innerHTML =
          "[<a id='_footnoteref_" + n + "' href='#_footnote_" + n +
          "' title='View footnote' class='footnote'>" + n + "</a>]";
        spans[i].setAttribute("data-note", note);
      }
      noteholder.innerHTML +=
        "<div class='footnote' id='_footnote_" + n + "'>" +
        "<a href='#_footnoteref_" + n + "' title='Return to text'>" +
        n + "</a>. " + note + "</div>";
      var id =spans[i].getAttribute("id");
      if (id != null) refs["#"+id] = n;
    }
  }
  if (n == 0)
    noteholder.parentNode.removeChild(noteholder);
  else {
    // Process footnoterefs.
    for (i=0; i<spans.length; i++) {
      if (spans[i].className == "footnoteref") {
        var href = spans[i].getElementsByTagName("a")[0].getAttribute("href");
        href = href.match(/#.*/)[0];  // Because IE return full URL.
        n = refs[href];
        spans[i].innerHTML =
          "[<a href='#_footnote_" + n +
          "' title='View footnote' class='footnote'>" + n + "</a>]";
      }
    }
  }
},

install: function(toclevels) {
  var timerId;

  function reinstall() {
    asciidoc.footnotes();
    if (toclevels) {
      asciidoc.toc(toclevels);
    }
  }

  function reinstallAndRemoveTimer() {
    clearInterval(timerId);
    reinstall();
  }

  timerId = setInterval(reinstall, 500);
  if (document.addEventListener)
    document.addEventListener("DOMContentLoaded", reinstallAndRemoveTimer, false);
  else
    window.onload = reinstallAndRemoveTimer;
}

}
asciidoc.install(3);
/*]]>*/
</script>
</head>
<body class="article">
<div id="header">
<h1>FAI Guide (Fully Automatic Installation)</h1>
<span id="author">Thomas Lange</span><br />
<span id="email"><code>&lt;<a href="mailto:lange@informatik.uni-koeln.de">lange@informatik.uni-koeln.de</a>&gt;</code></span><br />
<span id="revnumber">version 5.3,</span>
<span id="revdate">16 Jan 2017</span>
<div id="toc">
  <div id="toctitle">Table of Contents</div>
  <noscript><p><b>JavaScript must be enabled in your browser to display the table of contents.</b></p></noscript>
</div>
</div>
<div id="content">
<div class="sect1">
<h2 id="_abstrait">Abstrait</h2>
<div class="sectionbody">
<div class="paragraph"><p>FAI est un système non interactif permettant d&#8217;installer, de personnaliser et de gérer les configurations de systèmes et de logiciels Linux sur les ordinateurs ainsi que sur les machines virtuelles et les environnements chroot, des petits réseaux aux grandes infrastructures et clusters.</p></div>
<div class="paragraph"><p>Ce manuel décrit le logiciel d&#8217;installation entièrement automatique. Cela inclut l&#8217;installation des paquets, la configuration du serveur, la création de la configuration et la gestion des erreurs.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>     +-----------------------------------------------------------------------+
     | This manual describes FAI 5.3 but most things are also valid for 4.x. |
     +-----------------------------------------------------------------------+</code></pre>
</div></div>
<div class="paragraph"><p>(c) 2000-2017 Thomas Lange</p></div>
<div class="paragraph"><div class="title">Copyright</div><p>Ce manuel est un logiciel libre; Vous pouvez le redistribuer et / ou le modifier selon les termes de la Licence Publique Générale GNU publiée par la Free Software Foundation; Soit la version 2, soit (à votre choix) toute version ultérieure.</p></div>
<div class="paragraph"><p>Ceci est distribué dans l&#8217;espoir qu&#8217;il sera utile, mais sans aucune garantie ; Sans même la garantie implicite de qualité marchande ou d&#8217;adaptation à un usage particulier. Pour plus de détails, consultez la GNU General Public License.&lt;</p></div>
<div class="paragraph"><p>Une copie de la GNU General Public License est disponible sous la forme /usr/share/common-licenses/GPL dans la distribution Debian GNU/Linux ou sur le World Wide Web sur le site GNU Vous pouvez également l&#8217;obtenir en écrivant à la Free Software Foundation , Inc., 59 Temple Place - Suite 330, Boston, MA 02111-1307, États-Unis.</p></div>
<div style="page-break-after:always"></div>
</div>
</div>
<div class="sect1">
<h2 id="_a_id_introduction_a_introduction"><a id="Introduction"></a>Introduction</h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_a_id_disponibilité_a_disponibilité"><a id="Disponibilité"></a>Disponibilité</h3>
<div class="dlist"><dl>
<dt class="hdlist1">
Page d&#8217;accueil
</dt>
<dd>
<p>
<a href="http://fai-project.org">http://fai-project.org</a>
</p>
</dd>
<dt class="hdlist1">
FAI wiki
</dt>
<dd>
<p>
<a href="http://wiki.fai-project.org">http://wiki.fai-project.org</a>
</p>
</dd>
<dt class="hdlist1">
Téléchargement
</dt>
<dd>
<p>
<a href="http://fai-project.org/download">http://fai-project.org/download</a>
</p>
</dd>
<dt class="hdlist1">
Entrée pour <em>sources.list</em>
</dt>
<dd>
<p>
<code>deb http://fai-project.org/download jessie koeln</code>
</p>
</dd>
<dt class="hdlist1">
Pages du manuel
</dt>
<dd>
<p>
<a href="http://fai-project.org/doc/man/">http://fai-project.org/doc/man/</a>
</p>
</dd>
<dt class="hdlist1">
Liste de diffusion
</dt>
<dd>
<p>
<a href="https://lists.uni-koeln.de/mailman/listinfo/linux-fai">https://lists.uni-koeln.de/mailman/listinfo/linux-fai</a>
</p>
</dd>
<dt class="hdlist1">
Retour d&#8217;information
</dt>
<dd>
<p>
Envoyez vos commentaires et vos commentaires à <a href="mailto:fai@fai-project.orgou">fai@fai-project.orgou</a> à la liste de diffusion .
</p>
</dd>
<dt class="hdlist1">
Bogues
</dt>
<dd>
<p>
Utiliser le système de suivi des bogues Debian (BTS) <a href="http://bugs.debian.org">http://bugs.debian.org</a>
</p>
</dd>
<dt class="hdlist1">
Changements visibles par l&#8217;utilisateur
</dt>
<dd>
<p>
<a href="http://fai-project.org/NEWS">http://fai-project.org/NEWS</a>
</p>
</dd>
<dt class="hdlist1">
Arbre source via git
</dt>
<dd>
<p>
git clone git://github.com/faiproject/fai.git
</p>
</dd>
<dt class="hdlist1">
Voir l&#8217;arbre source avec http
</dt>
<dd>
<p>
<a href="https://github.com/faiproject/fai">https://github.com/faiproject/fai</a>
</p>
</dd>
</dl></div>
<div class="paragraph"><p>Les pages man incluent toujours des informations à jour et beaucoup de détails sur toutes les commandes FAI. Alors, n&#8217;oubliez pas de les lire attentivement. Lisez maintenant ce manuel, puis profitez de l&#8217;installation entièrement automatique et de votre temps économisé.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_motivation_a_motivation"><a id="Motivation"></a>Motivation</h3>
<div class="paragraph"><p>Avez-vous déjà effectué des installations identiques d&#8217;un système d&#8217;exploitation à plusieurs reprises? Souhaitez-vous être en mesure d&#8217;installer un cluster Linux avec des dizaines de nœuds à lui seul?</p></div>
<div class="paragraph"><p>Répéter la même tâche encore et encore est ennuyeux - et conduira certainement à des erreurs. Aussi beaucoup de temps pourrait être sauvé si les installations ont été faites automatiquement. Un processus d&#8217;installation avec interaction manuelle n&#8217;est pas à l'échelle. Mais les grappes ont l&#8217;habitude de croître au fil des ans. Pensez à long terme plutôt que de planifier quelques mois dans l&#8217;avenir.</p></div>
<div class="paragraph"><p>En 1999, j&#8217;ai dû effectuer une installation d&#8217;un cluster Linux avec un serveur et 16 clients. Puisque j&#8217;ai eu beaucoup d&#8217;expérience en faisant des installations automatiques des systèmes d&#8217;exploitation de Solaris sur le matériel de SUN SPARC, l&#8217;idée de construire une installation automatique pour Debian est née. Solaris dispose d&#8217;une fonctionnalité d&#8217;installation automatique appelée JumpStart <span class="footnote"><br />[Solaris 8 Advanced Installation Guide at <a href="https://docs.oracle.com/cd/E19455-01/806-0957/806-0957.pdf">https://docs.oracle.com/cd/E19455-01/806-0957/806-0957.pdf</a>]<br /></span>. En conjonction avec les scripts d&#8217;auto-installation de Casper Dik <span class="footnote"><br />[<a href="http://www.science.uva.nl/pub/solaris/auto-install">http://www.science.uva.nl/pub/solaris/auto-install</a>]<br /></span>, Je pourrais sauver beaucoup de temps non seulement pour chaque nouvel ordinateur de SUN, mais aussi pour la réinstallation des postes de travail existants. Par exemple, j&#8217;ai dû construire un LAN temporaire avec quatre stations de travail SUN pour une conférence, qui a duré seulement quelques jours. J&#8217;ai retiré ces postes de travail de notre réseau de recherche habituel et mis en place une nouvelle installation pour la conférence. Quand il était terminé, j&#8217;ai simplement intégré les postes de travail dans le réseau de recherche, redémarré une seule fois, et après une demi-heure, tout était opérationnel comme avant. La configuration de tous les postes de travail était exactement la même qu&#8217;avant la conférence, car tout était effectué par le même processus d&#8217;installation. J&#8217;ai également utilisé l&#8217;installation automatique pour réinstaller un poste de travail après un disque dur endommagé avait été remplacé. Il m&#8217;a fallu deux semaines pour recevoir le nouveau disque dur, mais seulement quelques minutes après l&#8217;installation du nouveau disque, le poste de travail fonctionnait comme avant. Et c&#8217;est pourquoi j&#8217;ai choisi d&#8217;adapter cette technique à un cluster de PC sous Linux.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_work_a_comment_fonctionne_fai"><a id="work"></a>Comment fonctionne FAI</h3>
<div class="paragraph"><p>Le client d&#8217;installation qui sera installé à l&#8217;aide de FAI, est démarré via une carte réseau ou à partir d&#8217;un CD ou d&#8217;une clé USB. Il obtient une adresse IP et démarre un noyau Linux qui monte son système de fichiers racine via NFS (nfsroot) du serveur d&#8217;installation. Une fois le noyau démarré, le script de démarrage FAI exécute l&#8217;installation automatique qui n&#8217;a pas besoin d&#8217;interaction. Tout d&#8217;abord, les disques durs seront partitionnés, les systèmes de fichiers seront créés et des progiciels seront ensuite installés. Après cela, le nouveau système d&#8217;exploitation installé est configuré selon vos besoins locaux en utilisant quelques scripts. Enfin, le nouveau système d&#8217;exploitation sera démarré à partir du disque local.</p></div>
<div class="paragraph"><p>Les détails sur la façon d&#8217;installer l&#8217;ordinateur (la configuration) sont stockés dans l&#8217;espace de configuration du serveur d&#8217;installation. Les fichiers de configuration sont partagés entre des groupes d&#8217;ordinateurs s&#8217;ils sont similaires en utilisant le concept de classe. Vous n&#8217;avez donc pas besoin de créer une configuration pour chaque nouvel hôte. Par conséquent, FAI est une méthode évolutive pour installer un gros cluster avec un grand nombre de nœuds même si leur configuration n&#8217;est pas identique.</p></div>
<div class="paragraph"><p>FAI peut également être utilisé comme un système de sauvetage ou pour l&#8217;inventaire matériel. Vous pouvez démarrer votre ordinateur, mais il n&#8217;effectuera pas une installation. Au lieu de cela, il exécutera un Debian GNU / Linux entièrement fonctionnel sans utiliser les disques durs locaux. Ensuite, vous pouvez effectuer une connexion à distance et sauvegarder ou restaurer une partition de disque, vérifier un système de fichiers, inspecter le matériel ou effectuer toute autre tâche.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_features_a_caractéristiques"><a id="features"></a>Caractéristiques</h3>
<div class="ulist"><ul>
<li>
<p>
Une installation entièrement automatisée peut être effectuée.
</p>
</li>
<li>
<p>
Très rapide installation sans surveillance.
</p>
</li>
<li>
<p>
Système flexible grâce à un concept de classe simple.
</p>
</li>
<li>
<p>
Mise à jour des systèmes en cours d&#8217;exécution sans réinstallation.
</p>
</li>
<li>
<p>
Création facile d&#8217;un environnement de virtualisation ou d&#8217;un chroot
</p>
</li>
<li>
<p>
Les hôtes peuvent démarrer à partir d&#8217;une carte réseau, d&#8217;un CD, d&#8217;une clé USB.
</p>
</li>
<li>
<p>
Création simple d&#8217;un CD d&#8217;installation ou d&#8217;une clé USB.
</p>
</li>
<li>
<p>
PXE avec la méthode de démarrage DHCP est pris en charge.
</p>
</li>
<li>
<p>
ReiserFS, ext3 / ext4, btrfs et support de système de fichiers XFS.
</p>
</li>
<li>
<p>
Support logiciel RAID et LVM.
</p>
</li>
<li>
<p>
Détection automatique du matériel.
</p>
</li>
<li>
<p>
Vous pouvez déployer Debian, Ubuntu, CentOS, SuSE, Scientific Linux
</p>
</li>
<li>
<p>
Connexion à distance via ssh lors du processus d&#8217;installation possible.
</p>
</li>
<li>
<p>
Toutes les configurations similaires sont partagées entre tous les clients d&#8217;installation.
</p>
</li>
<li>
<p>
Les fichiers journaux de toutes les installations sont enregistrés sur le serveur d&#8217;installation.
</p>
</li>
<li>
<p>
Les scripts Shell, Perl, Python, Ruby, expect et CFEngine sont pris en charge lors de l'étape de personnalisation.
</p>
</li>
<li>
<p>
Prise en charge de nombreux protocoles comme NFS, FTP, HTTP, git
</p>
</li>
<li>
<p>
Peut être utilisé comme un système de sauvetage et pour l&#8217;inventaire matériel.
</p>
</li>
<li>
<p>
Prise en charge du client sans disque.
</p>
</li>
<li>
<p>
Ajoutez facilement vos propres fonctions via des hooks ou modifiez le comportement par défaut.
</p>
</li>
<li>
<p>
Clonage de machines utilisant des images de disque est pris en charge
</p>
</li>
</ul></div>
</div>
<div class="sect2">
<h3 id="_le_temps_de_l_8217_installation">Le temps de l&#8217;installation</h3>
<div class="paragraph"><p>Le temps d&#8217;installation est déterminé par la quantité de logiciel et la vitesse du disque dur. Voici quelques exemples de temps. Tous les clients d&#8217;installation avaient une carte réseau 1Gbit installée.</p></div>
<div class="tableblock">
<table rules="all"
width="80%"
frame="border"
cellspacing="0" cellpadding="4">
<col width="26%" />
<col width="13%" />
<col width="20%" />
<col width="26%" />
<col width="13%" />
<thead>
<tr>
<th align="left" valign="top"> CPU  </th>
<th align="center" valign="top">  RAM </th>
<th align="left" valign="top">   Disk    </th>
<th align="right" valign="top">   Software installed  </th>
<th align="right" valign="top"> time</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left" valign="top"><p class="table">i7-3770T 2.50GHz</p></td>
<td align="center" valign="top"><p class="table">8GB</p></td>
<td align="left" valign="top"><p class="table">SSD</p></td>
<td align="right" valign="top"><p class="table">6 GB software</p></td>
<td align="right" valign="top"><p class="table">8.5 min</p></td>
</tr>
<tr>
<td align="left" valign="top"><p class="table">Core-i7 3.2GHz</p></td>
<td align="center" valign="top"><p class="table">6GB</p></td>
<td align="left" valign="top"><p class="table">SATA disk</p></td>
<td align="right" valign="top"><p class="table">4.3GB software</p></td>
<td align="right" valign="top"><p class="table">7 min</p></td>
</tr>
<tr>
<td align="left" valign="top"><p class="table">Core-i7 3.2GHz</p></td>
<td align="center" valign="top"><p class="table">6GB</p></td>
<td align="left" valign="top"><p class="table">SATA disk</p></td>
<td align="right" valign="top"><p class="table">471 MB software</p></td>
<td align="right" valign="top"><p class="table">77sec</p></td>
</tr>
<tr>
<td align="left" valign="top"><p class="table">Intel Core2 Duo</p></td>
<td align="center" valign="top"><p class="table">2GB</p></td>
<td align="left" valign="top"><p class="table">SATA disk</p></td>
<td align="right" valign="top"><p class="table">3 GB software</p></td>
<td align="right" valign="top"><p class="table">14 min</p></td>
</tr>
</tbody>
</table>
</div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_a_id_impatient_a_quickstart_pour_l_8217_utilisateur_impatient"><a id="impatient"></a>Quickstart - Pour l&#8217;utilisateur impatient</h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_a_id_first_a_ma_première_installation"><a id="first"></a>Ma première installation</h3>
<div class="paragraph"><p>Sans plus tarder, cette section fournira une démonstration rapide et facile d&#8217;une installation entièrement automatique à l&#8217;aide du CD FAI et d&#8217;une machine virtuelle.</p></div>
<div class="paragraph"><p>Il suffit de télécharger l' image ISO du CD à partir de <a href="http://fai-project.org/fai-cd">http://fai-project.org/fai-cd</a> et de démarrer votre VM à l&#8217;aide de ce CD. Vous verrez un menu grub où vous pouvez choisir parmi différents types d&#8217;installation.</p></div>
<div class="paragraph"><p>Cette installation s&#8217;exécutera sans serveur d&#8217;installation. L&#8217;installation du CD est identique à celle exécutée dans un environnement réseau à l&#8217;aide du serveur d&#8217;installation FAI.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_cdserver_a_mon_premier_serveur_d_8217_installation"><a id="cdserver"></a>Mon premier serveur d&#8217;installation</h3>
<div class="paragraph"><p>S&#8217;il vous plaît noter, si vous avez l&#8217;intention d&#8217;utiliser QEMU/KVM, vous devez avoir qemu-kvm qemu-utils bridge-utils installés sur la machine à utiliser fai-mk-network et fai-kvm <span class="footnote"><br />[fai-kvm a besoin de beaucoup de ram pour la vm, à cause de la mise en cache de /var, 2GB sont OK]<br /></span>.</p></div>
<div class="paragraph"><p>Vous pouvez le faire via</p></div>
<div class="listingblock">
<div class="content">
<pre><code># apt-get install qemu-kvm qemu-utils bridge-utils</code></pre>
</div></div>
<div class="paragraph"><p>Si vous avez l&#8217;intention d&#8217;utiliser VMware ou VirtualBox, assurez-vous que votre client utilise une connexion réseau pontée. En outre, il n&#8217;est pas possible d&#8217;utiliser des interfaces réseau pontées via le réseau sans fil, car la plupart des cartes réseau WiFi ne prennent pas en charge cette fonctionnalité.</p></div>
<div class="paragraph"><p>our configurer votre propre serveur FAI, nous vous recommandons de créer un réseau de test sur votre ordinateur et d&#8217;utiliser KVM. Pour créer ce réseau privé, il ya le script fai-mk-network (dans le paquet fai-server). Il configure un pont logiciel avec plusieurs dispositifs de dérivation qui appartiennent à l&#8217;utilisateur&lt;username&gt;.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>fai-mk-network &lt;username&gt;</code></pre>
</div></div>
<div class="paragraph"><p>Après cela, vous pouvez utiliser fai-kvm (-h vous aidera) pour démarrer des machines virtuelles en utilisant KVM qui sont connectés à ce réseau privé. Fais attention. Par défaut, fai-kvm créera les images de disque pour les machines <code>/tmp</code>, qui est un disque RAM sur la plupart des systèmes. Il n&#8217;y a aucun problème à créer une image de disque vide de 20G dans /tmp (même si cette partition est de 4 Go de taille), mais alors que la VM écrit des données sur son disque, cela commencera à consommer de l&#8217;espace dans <code>/tmp</code>.</p></div>
<div class="paragraph"><p>Démarrez le premier hôte virtuel, qui deviendra le serveur FAI <span class="footnote"><br />[Cette installation consommera environ 2 Go d&#8217;espace dans <code>/tmp</code>.]<br /></span>:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>fai-kvm -Vn -s20 -u 1 cd fai-cd.iso</code></pre>
</div></div>
<div class="paragraph"><p>Dans le menu grub faiserver,<code>faiserver, fixed IP</code>. Cela va installer un hôte appelé faiserver avec IP 192.168.33.250 qui contient tous les logiciels nécessaires pour un serveur FAI. Il configurera également un cache de paquets local (en utilisant apt-cacher-ng). Une fois l&#8217;installation terminée, redémarrez la machine. Lors du premier démarrage du nouveau système, il configurera automatiquement le nfsroot. Cela peut prendre quelques minutes.</p></div>
<div class="paragraph"><p>Après cela, vous pouvez démarrer des hôtes supplémentaires en utilisant le démarrage réseau. Pour chaque nouvel hôte, vous devez utiliser une valeur différente pour <code>-u</code>, qui sera utilisée pour générer des adresses MAC différentes et utiliser des noms de fichier d&#8217;image de disque différents.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>fai-kvm -Vn -u 2 pxe</code></pre>
</div></div>
<div class="paragraph"><p>Ces clients d&#8217;installation vous montreront un menu, où vous pouvez sélectionner le type d&#8217;installation que vous souhaitez effectuer. Si le client d&#8217;installation ne trouve pas le serveur, c&#8217;est généralement parce que fai-monitor ne fonctionne plus. Cela peut se produire si vous redémarrez le faiserver après l&#8217;installation. Pour remédier à cela, exécutez simplement fai-monitor sur le faiserver et relancez le démarrage du client.</p></div>
<div class="paragraph"><p>Un autre client pourrait être lancé avec:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>fai-kvm -Vn -u 3 pxe</code></pre>
</div></div>
<div class="paragraph"><p>Vous pouvez démarrer autant de machines dans le réseau que les périphériques de prise sont disponibles. Toutes ces machines peuvent se connecter à l&#8217;Internet extérieur, mais sont seulement accessibles à partir de votre machine hôte.</p></div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_a_id_overview_a_vue_d_8217_ensemble_et_concepts"><a id="overview"></a>Vue d&#8217;ensemble et concepts</h2>
<div class="sectionbody">
<div class="paragraph"><p>FAI est un système non interactif permettant d&#8217;installer, de personnaliser et de gérer les configurations de systèmes et de logiciels Linux sur les ordinateurs ainsi que sur les machines virtuelles et les environnements chroot, des petits réseaux aux grandes infrastructures et clusters. Vous pouvez prendre un ou plusieurs PC vierges, mettre sous tension et après quelques minutes, Linux est installé, configuré et exécuté sur l&#8217;ensemble du cluster, sans aucune interaction nécessaire. Ainsi, il s&#8217;agit d&#8217;une méthode évolutive pour installer et mettre à jour un cluster sans surveillance avec peu d&#8217;efforts impliqués. FAI utilise le système d&#8217;exploitation Linux et une collection de scripts shell et Perl pour le processus d&#8217;installation. Les modifications apportées aux fichiers de configuration du système d&#8217;exploitation peuvent être effectuées par CFEngine, shell (bash et zsh), Perl, Python, Ruby et attendent des scripts.</p></div>
<div class="paragraph"><p>Le groupe cible de FAI sont des administrateurs système qui doivent installer Linux sur une ou même des centaines d&#8217;ordinateurs. Parce qu&#8217;il s&#8217;agit d&#8217;un outil d&#8217;installation à usage général, il peut être utilisé pour l&#8217;installation d&#8217;un cluster Beowulf, d&#8217;une batterie de rendu ou d&#8217;un laboratoire Linux ou d&#8217;une salle de classe. De plus, des réseaux Linux de grande envergure avec différents matériels ou différentes exigences d&#8217;installation sont faciles à établir à l&#8217;aide de FAI. Mais n&#8217;oubliez pas de planifier votre installation. Le chapitre <a href="#plan">[plan]</a> contient quelques conseils utiles pour ce sujet.</p></div>
<div class="sect2">
<h3 id="_a_id_terms_a_conditions_générales"><a id="terms"></a> Conditions Générales</h3>
<div class="paragraph"><p>Premièrement, certains termes utilisés dans ce manuel sont décrits.</p></div>
<div class="dlist"><dl>
<dt class="hdlist1">
Installer le serveur
</dt>
<dd>
<p>
Il fournit les services DHCP, TFTP et NFS ainsi que les données de configuration pour tous les clients d&#8217;installation. Dans les exemples de ce manuel, cet hôte s&#8217;appelle <em>faiserver</em>. L&#8217;hôte où le package <em>fai-server</em> est installé.
</p>
</dd>
<dt class="hdlist1">
Installer le client
</dt>
<dd>
<p>
Un hôte qui sera installé à l&#8217;aide de FAI et une configuration fournie par le serveur d&#8217;installation. Aussi appelé client pour courte. Dans ce manuel, les hôtes d&#8217;exemple sont appelés demohost, xfcehost, gnomehost … Cet ordinateur doit démarrer à partir de son interface réseau à l&#8217;aide de PXE.
</p>
</dd>
<dt class="hdlist1">
Espace de configuration
</dt>
<dd>
<p>
Une structure de sous-répertoire contenant plusieurs fichiers. Ces fichiers décrivent les détails de la manière dont l&#8217;installation des clients sera effectuée. Toutes les données de configuration sont stockées ici. Il est également appelé config space pour le court. Il comprend des informations sur:
</p>
<div class="ulist"><ul>
<li>
<p>
Disposition du disque dur dans un format similaire à fstab
</p>
</li>
<li>
<p>
Systèmes de fichiers locaux, leurs types, points de montage et options de montage
</p>
</li>
<li>
<p>
Logiciels
</p>
</li>
<li>
<p>
Disposition du clavier, fuseau horaire, configuration Xorg, systèmes de fichiers distants,
comptes utilisateurs, imprimantes &#8230;
</p>
</li>
</ul></div>
<div class="paragraph"><p>Le package <em>fai-doc</em> inclut un exemple d&#8217;espace de configuration incluant des exemples pour les hôtes utilisant l&#8217;environnement XFCE et GNOME parmi d&#8217;autres exemples.</p></div>
</dd>
<dt class="hdlist1">
nfsroot, NFS-Root
</dt>
<dd>
<p>
Un système de fichiers situé sur le serveur d&#8217;installation. Pendant le processus d&#8217;installation, c&#8217;est le système de fichiers complet pour les clients d&#8217;installation. Tous les clients partagent le même nfsroot, qu&#8217;ils montent en lecture seule. Le nfsroot a besoin d&#8217;environ 690 Mo d&#8217;espace disque libre.
</p>
</dd>
<dt class="hdlist1">
TFTP
</dt>
<dd>
<p>
Sert aux clients l&#8217;initrd et le noyau utilisés pour le processus d&#8217;installation. Avec le système de fichiers servi par NFS, ces deux composent un OS temporaire dans lequel les installations sont exécutées.
</p>
</dd>
<dt class="hdlist1">
Classes FAI
</dt>
<dd>
<p>
Les classes sont des noms qui déterminent quel fichier de configuration est sélectionné. Si un client appartient à la classe WEBSERVER, il sera configuré en tant que serveur Web, la classe DESKTOP pour, par exemple, détermine les progiciels qui seront installés.
</p>
</dd>
<dt class="hdlist1">
profil
</dt>
<dd>
<p>
Un profil FAI est juste une liste de classes FAI assiged à un nom de profil, qui est étendu par une description de ce profil. C&#8217;est-à-dire que l&#8217;on peut avoir deux profils "Webserver", l&#8217;un incluant la classe APACHE, y compris la classe NGINX, pour ensuite installer la solution webserver respective.
</p>
</dd>
<dt class="hdlist1">
les tâches
</dt>
<dd>
<p>
L&#8217;installation d&#8217;un client se compose de plusieurs parties, appelées tâches. Les tâches sont des sous-programmes prédéfinis qui effectuent une certaine partie de la FAI. Les tâches FAI suivantes sont exécutées au cours d&#8217;une installation sur les clients d&#8217;installation.
</p>
</dd>
</dl></div>
<div class="quoteblock">
<div class="content">
<div class="paragraph"><p>confdir               # get the config space
setup                 # some initialization, start sshd on demand
defclass              # define FAI classes
defvar                # define variables
action                # evaluate FAI_ACTION
install               # Start the installation
partition             # partition the harddisks, create file systems
mountdisks            # mount the file systems
extrbase              # extract the base.tar.xz
debconf               # do the Debian debconf preseeding
repository            # prepare access to the package repository
updatebase            # Set up package tools and update packages
instsoft              # install software packages
configure             # call customization scripts
finish                # do some cleanup, show installation statistics
tests                 # call tests if defined
chboot                # call fai-chboot on the install server
savelog               # save log files to local and remote location
faiend                # reboot host, eject CD if needed</p></div>
</div>
<div class="attribution">
</div></div>
<div class="quoteblock">
<div class="content">
<div class="paragraph"><p>Il s&#8217;agit de tâches qui ne sont exécutées que lorsqu&#8217;une action différente est exécutée</p></div>
<div class="paragraph"><p>dirinstall           # install a chroot environment
softupdate           # only do the system configuration
sysinfo              # print detailed system information
inventory            # print short hardware inventory list</p></div>
</div>
<div class="attribution">
</div></div>
<div class="paragraph"><p>Pour une description plus détaillée des <em>tâches</em> , voir <a href="#tasks">[tasks]</a>.</p></div>
<div class="paragraph"><p>Notez que vous n'êtes pas limité aux tâches FAI. Vous pouvez également définir des programmes ou des scripts supplémentaires qui seront exécutés à certaines occasions. On les appelle des <em>hooks</em>.</p></div>
<div class="dlist"><dl>
<dt class="hdlist1">
hooks
</dt>
<dd>
<p>
Les Hooks sont des plugins, ils peuvent ajouter des fonctionnalités supplémentaires au processus d&#8217;installation ou même remplacer des tâches entières de FAI. Les Hooks sont expliqués en détail dans <a href="#hooks">[hooks]</a>.
</p>
</dd>
</dl></div>
</div>
<div class="sect2">
<h3 id="_a_id_classc_a_le_concept_de_classe"><a id="classc"></a>Le concept de classe</h3>
<div class="paragraph"><p>Les classes sont utilisées dans presque toutes les tâches de l&#8217;installation. Les classes déterminent quels fichiers de configuration choisir parmi une liste d&#8217;alternatives disponibles. Pour déterminer les fichiers de configuration à utiliser, FAI recherche la liste des classes définies et utilise tous les fichiers de configuration correspondant à un nom de classe <span class="footnote"><br />[Il est également possible d&#8217;utiliser uniquement le fichier de configuration avec la plus haute priorité puisque l&#8217;ordre des classes définit une priorité de bas à haut dans la liste des classes. ]<br /></span>. La boucle suivante implémente cette fonction en pseudo code shell:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>for class in $all_classes; do
   if [ -r $config_dir/$class ]; then      # if a file with name $class exists
      your_command $config_dir/$class      # call a command with this file name
      # exit if only the first matching file is needed
   fi
done</code></pre>
</div></div>
<div class="paragraph"><p>La caractéristique très intéressante de ceci est que vous pouvez ajouter une nouvelle alternative de configuration et elle sera automatiquement utilisée par FAI sans changer le code, si le fichier de configuration utilise un nom de classe.</p></div>
<div class="paragraph"><p>C&#8217;est parce que la boucle détecte automatiquement les nouveaux fichiers de configuration qui doivent être utilisés. L&#8217;idée d&#8217;utiliser des classes en général et d&#8217;utiliser certains fichiers correspondant à un nom de classe pour une configuration est adoptée à partir des scripts d&#8217;installation par Casper Dik pour Solaris. Cette technique s&#8217;est avérée très utile et facile.</p></div>
<div class="paragraph"><p>Vous pouvez regrouper plusieurs hôtes partageant les mêmes fichiers de configuration en utilisant la même classe. Vous pouvez également diviser l&#8217;ensemble des données de configuration pour tous les clients en plusieurs classes et les utiliser comme des briques de lego et construire la configuration entière pour un seul client en assemblant les briques ensemble.</p></div>
<div class="paragraph"><p>Si un client appartient à la classe <em>A</em>, nous disons que la classe <em>A</em> est définie pour ce client. Une classe n&#8217;a pas de valeur, elle est juste définie ou non définie.</p></div>
<div class="paragraph"><p>Les classes déterminent comment l&#8217;installation est effectuée. Par exemple, un client d&#8217;installation peut être configuré pour obtenir le bureau XFCE en y ajoutant simplement la classe <em>XFCE</em> . Naturellement, des configurations plus granulaires sont également possibles. Par exemple, les classes peuvent décrire comment le disque dur doit être partitionné, ils peuvent définir quels paquets logiciels seront installés ou quelles étapes de personnalisation seront exécutées.</p></div>
<div class="paragraph"><p>Souvent, une configuration client est créée en modifiant ou en ajoutant uniquement les classes auxquelles ce client appartient, ce qui rend l&#8217;installation d&#8217;un nouveau client très facile. Ainsi, aucune information supplémentaire ne doit être ajoutée à l&#8217;espace de configuration si les classes existantes suffisent à vos besoins.</p></div>
<div class="paragraph"><p>Comme vous pouvez le voir, les classes sont un pilier central de la personnalisation de votre espace de configuration et de l&#8217;installation de votre client. Pour définir vos propres classes, reportez-vous à <a href="#defining classes">[defining classes]</a>.</p></div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_a_id_setup_a_configurer_votre_faiserver"><a id="setup"></a>Configurer votre faiserver</h2>
<div class="sectionbody">
<div class="paragraph"><p>Voici comment configurer le serveur d&#8217;installation en quelques minutes. Les étapes suivantes sont nécessaires:</p></div>
<div class="olist arabic"><ol class="arabic">
<li>
<p>
Configurer le serveur d&#8217;installation
</p>
<div class="olist loweralpha"><ol class="loweralpha">
<li>
<p>
Installer des packages FAI
</p>
</li>
<li>
<p>
Créez le nfsroot
</p>
</li>
<li>
<p>
Copiez les exemples dans l&#8217;espace de configuration
</p>
</li>
<li>
<p>
Configurer les démons réseau
</p>
</li>
<li>
<p>
Créer les configurations PXELINUX
</p>
</li>
</ol></div>
</li>
<li>
<p>
Démarrage et installation des clients
</p>
</li>
</ol></div>
<div class="sect2">
<h3 id="_installer_les_paquetages_fai">Installer les paquetages FAI</h3>
<div class="ulist"><ul>
<li>
<p>
Installez la clé du référentiel de package de projet FAI:
</p>
</li>
<li>
<p>
Ajoutez l&#8217;URL du référentiel de packages du projet FAI.
</p>
</li>
<li>
<p>
Installez le paquet fai-quickstart sur votre serveur d' installation .
</p>
</li>
</ul></div>
<div class="listingblock">
<div class="content">
<pre><code># wget -O - http://fai-project.org/download/074BCDE4.asc | apt-key add -
# echo "deb http://fai-project.org/download jessie koeln" &gt; /etc/apt/sources.list.d/fai.list
# apt-get update
# aptitude install fai-quickstart</code></pre>
</div></div>
<div class="paragraph"><p>Cela installera également les paquets pour les démons de serveur DHCP, TFTP et NFS.</p></div>
</div>
<div class="sect2">
<h3 id="_créez_le_nfsroot">Créez le nfsroot</h3>
<div class="ulist"><ul>
<li>
<p>
Activez également le référentiel de package du projet FAI dans un autre fichier <em>sources.list</em> qui est utilisé lors de la construction du nfsroot. Ensuite, activez l&#8217;utilisateur de journal pour FAI.
</p>
</li>
</ul></div>
<div class="listingblock">
<div class="content">
<pre><code># sed -i -e 's/^#deb/deb/' /etc/fai/apt/sources.list
# sed -i -e 's/#LOGUSER/LOGUSER/' /etc/fai/fai.conf</code></pre>
</div></div>
<div class="ulist"><ul>
<li>
<p>
Par défaut, FAI utilise <a href="http://httpredir.debian.org">http://httpredir.debian.org</a> comme mirror de paquets, qui devrait tenter de trouver un référentiel de paquets rapide pour vous. <span class="footnote"><br />[Si vous souhaitez utiliser un miroir plus rapide, ajustez l&#8217;URL dans <em>/etc/fai/apt/sources.list</em> et <code>FAI_DEBOOTSTRAP</code> in <em>/etc/fai/nfsroot.conf</em> avant d&#8217;appeler fai-setup.]<br /></span>
Maintenant, nous pouvons exécuter <code>fai-setup(8)</code> <span class="footnote"><br />[Ceci appellera <code>fai-make-nfsroot(8)</code> interne.]<br /></span> Et vérifier si tout s&#8217;est bien passé. Le fichier journal est écrit dans /var/log/fai/fai-setup.log.
</p>
</li>
</ul></div>
<div class="listingblock">
<div class="content">
<pre><code># fai-setup -v</code></pre>
</div></div>
<div class="ulist"><ul>
<li>
<p>
Ce sont quelques-unes des lignes que vous verrez à la fin de fai-setup . Un exemple complet de fai-setup.log est disponible sur la page Web FAI à l&#8217;adresse <a href="http://fai-project.org/logs/fai-setup.log">http://fai-project.org/logs/fai-setup.log</a>.
</p>
</li>
</ul></div>
<div class="listingblock">
<div class="content">
<pre><code>FAI packages and related packages inside the nfsroot:
dracut             044+189-2
dracut-network     044+189-2
fai-client         5.3.3~bpo8+2
fai-nfsroot        5.3.3~bpo8+2
fai-setup-storage  5.3.3~bpo8+2
Waiting for background jobs to finish
fai-make-nfsroot finished properly.
Log file written to /var/log/fai/fai-make-nfsroot.log
Adding line to /etc/exports: /srv/fai/config 192.168.33.250/25(async,ro,no_subtree_check)
Adding line to /etc/exports: /srv/fai/nfsroot 192.168.33.250/25(async,ro,no_subtree_check,no_root_squash)
Reloading nfs-kernel-server configuration (via systemctl): nfs-kernel-server.service.

   You have no FAI configuration space yet. Copy the simple examples with:
   cp -a /usr/share/doc/fai-doc/examples/simple/* /srv/fai/config
   Then change the configuration files to meet your local needs.
Please don't forget to fill out the FAI questionnaire after you've finished your project with FAI.

FAI setup finished.
Log file written to /var/log/fai/fai-setup.log</code></pre>
</div></div>
<div class="ulist"><ul>
<li>
<p>
Fai-setup a créé le LOGUSER, le nfsroot et a ajouté des lignes supplémentaires à <em>/etc/exports</em>. Les sous-répertoires ajoutés à <em>/etc/exports</em> sont exportés via NFS v3, de sorte que tous les clients d&#8217;installation dans le même sous-réseau peuvent les monter via NFS.
</p>
</li>
</ul></div>
</div>
<div class="sect2">
<h3 id="_création_de_l_8217_espace_de_configuration">Création de l&#8217;espace de configuration</h3>
<div class="paragraph"><p>Installez les exemples simples dans l&#8217;espace de configuration <span class="footnote"><br />[Ces fichiers ne doivent pas appartenir au compte racine.]<br /></span>.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>$ cp -a /usr/share/doc/fai-doc/examples/simple/* /srv/fai/config/</code></pre>
</div></div>
<div class="paragraph"><p>Ces exemples contiennent la configuration pour certains hôtes d&#8217;exemple. Selon le nom d&#8217;hôte utilisé, votre ordinateur sera configuré comme suit:</p></div>
<div class="dlist"><dl>
<dt class="hdlist1">
demohost
</dt>
<dd>
<p>
Une machine qui n&#8217;a besoin que d&#8217;un petit disque dur. Cette machine est configurée avec le réseau en tant que client DHCP, et une démo de compte est créée.
</p>
</dd>
<dt class="hdlist1">
xfcehost
</dt>
<dd>
<p>
Un bureau XFCE est installé, utilisant LVM, et la démo du compte est créée.
</p>
</dd>
<dt class="hdlist1">
gnomehost
</dt>
<dd>
<p>
Un bureau GNOME est installé et la démo du compte est créée.
</p>
</dd>
<dt class="hdlist1">
other host names
</dt>
<dd>
<p>
Les hôtes disposant d&#8217;un autre nom d&#8217;hôte utiliseront notamment les classes FAIBASE, DHCPC et GRUB.
</p>
</dd>
</dl></div>
<div class="paragraph"><p>Tous les hôtes auront un compte appelé demo avec mot de passe <em>fai</em>. Le compte root a également le mot de passe <em>fai</em>.</p></div>
<div class="paragraph"><p>Si l&#8217;indicateur FAI <code>menu</code> est ajouté, au lieu d&#8217;utiliser le nom d&#8217;hôte pour déterminer le type d&#8217;installation, un menu est présenté et l&#8217;utilisateur peut choisir un profil pour l&#8217;installation.</p></div>
</div>
<div class="sect2">
<h3 id="_configurer_les_démons_réseau">Configurer les démons réseau</h3>
<div class="paragraph"><p>Pour démarrer le client d&#8217;installation via PXE, le serveur d&#8217;installation a besoin d&#8217;un DHCP et d&#8217;un démon TFTP en cours d&#8217;exécution. Le paquet <em>fai-quickstart</em> a déjà installé les progiciels pour ces daemons. En outre, le paquetage du serveur NFS pour l&#8217;exportation du nfsroot et de l&#8217;espace de configuration a été installé.</p></div>
<div class="sect3">
<h4 id="_a_id_bootdhcp_a_configuration_du_démon_dhcp"><a id="bootdhcp"></a>Configuration du démon DHCP</h4>
<div class="paragraph"><p>déalement, votre faiserver doit également être votre serveur DHCP. Si ce n&#8217;est pas le cas, demandez à l&#8217;administrateur responsable du serveur DHCP de le configurer conformément à cette section. En option, il est possible d'éviter cela en utilisant la fonctionnalité <a href="#autodiscover">[autodiscover]</a> diffusée dans FAI 5.0.</p></div>
<div class="paragraph"><p>n exemple pour <code>dhcpd.conf(5)</code> est fourni avec le paquet <em>fai-doc</em>. Commencez à utiliser cet exemple et regardez toutes les options qui y sont utilisées.</p></div>
<div class="listingblock">
<div class="content">
<pre><code># cp /usr/share/doc/fai-doc/examples/etc/dhcpd.conf /etc/dhcp/</code></pre>
</div></div>
<div class="paragraph"><p>Les seules informations spécifiques FAI contenues dans ce fichier de configuration sont de définir le <code>filename</code> de <code>fai/pxelinux.0</code> et de définir <code>next-server</code> et <code>server-name</code> sur le nom de votre serveur d&#8217;install . Toutes les autres informations sont uniquement des données liées au réseau, qui est utilisé dans presque toutes les configurations DHCP. Ajustez ces paramètres de réseau à vos besoins locaux.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>deny unknown-clients;
option dhcp-max-message-size 2048;
use-host-decl-names on;

subnet 192.168.33.0 netmask 255.255.255.0 {
   option routers 192.168.33.250;
   option domain-name "my.example";
   option domain-name-servers 192.168.33.250;
   option time-servers faiserver;
   option ntp-servers faiserver;
   server-name faiserver;
   next-server faiserver;
   filename "fai/pxelinux.0";
}</code></pre>
</div></div>
<div class="paragraph"><p>Si vous apportez des modifications à la configuration DHCP, vous devez redémarrer le démon.</p></div>
<div class="listingblock">
<div class="content">
<pre><code># /etc/init.d/isc-dhcp-server restart</code></pre>
</div></div>
<div class="paragraph"><p>Si vous disposez de plusieurs interfaces réseau, vous pouvez définir l&#8217;interface que le serveur écoutera dans <em>/etc/default/isc-dhcp-server</em>. Par défaut, le démon DHCP écrit ses messages de journalisation dans <em>/var/log/daemon.log</em>.</p></div>
</div>
<div class="sect3">
<h4 id="_ajout_d_8217_une_entrée_d_8217_hôte_au_dhcp">Ajout d&#8217;une entrée d&#8217;hôte au DHCP</h4>
<div class="paragraph"><p>L&#8217;adresse MAC est donnée par le matériel de la carte réseau. Pour chaque client d&#8217;installation, vous collectez son adresse MAC et la mappez à une adresse IP et à un nom d&#8217;hôte. Tout d&#8217;abord, nous ajoutons l&#8217;adresse IP et le nom d&#8217;hôte à <em>/etc/hosts</em> <span class="footnote"><br />[Vous pouvez également ajouter ceci dans votre système de noms de domaine (DNS)]<br /></span>.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>192.168.33.100    demohost</code></pre>
</div></div>
<div class="paragraph"><p>Le mappage de l&#8217;adresse MAC à l&#8217;adresse IP est effectué dans le fichier <em>dhcpd.conf</em>. Ici, nous ajoutons une entrée d&#8217;hôte en utilisant la commande <code>dhcp-edit(8)</code> . Ici, vous devez remplacer 01:02:03:AB:CD:EF avec le MAC que vous avez trouvé.</p></div>
<div class="listingblock">
<div class="content">
<pre><code># dhcp-edit demohost 01:02:03:AB:CD:EF</code></pre>
</div></div>
<div class="paragraph"><p>Après avoir appelé cette commande, c&#8217;est ce que l&#8217;entrée hôte dans dhcpd.conf ressemblera à:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>host demohost {hardware ethernet 01:02:03:AB:CD:EF;fixed-address demohost;}</code></pre>
</div></div>
</div>
<div class="sect3">
<h4 id="_tftp">TFTP</h4>
<div class="paragraph"><p>Normalement, vous n&#8217;avez pas besoin d&#8217;apporter de modifications à la configuration dameon TFTP. Les fichiers fournis par TFTP sont situés dans <em>/srv/tftp/fai</em>.</p></div>
</div>
<div class="sect3">
<h4 id="_nfs">NFS</h4>
<div class="paragraph"><p>La commande <code>fai-setup</code> a déjà configuré le démon NFS et ajouté quelques lignes au fichier de configuration <em>/etc/exports</em>. Il exporte les répertoires en utilisant NFS v3.</p></div>
</div>
</div>
<div class="sect2">
<h3 id="_création_de_la_configuration_pxelinux">Création de la configuration PXELINUX</h3>
<div class="paragraph"><p>La dernière étape avant de démarrer votre client pour la première fois est de spécifier quelle configuration le client doit démarrer lors de l&#8217;amorçage PXE. Nous fai-chboot(8) la commande <code>fai-chboot(8)</code> pour créer une configuration pxelinux pour chaque client d&#8217;installation. Cela comprend des informations sur le noyau, l&#8217;initrd, l&#8217;espace de configuration et certains paramètres d&#8217;amorçage. Vous devriez lire la page de manuel, qui vous donne quelques bons exemples. Voici la commande pour démarrer l&#8217;installation de l&#8217;hôte demohost.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>$ fai-chboot -IFv -u nfs://faiserver/srv/fai/config demohost
Booting kernel vmlinuz-3.16.0-4-amd64
 append initrd=initrd.img-3.16.0-4-amd64 ip=dhcp
   FAI_FLAGS=verbose,sshd,createvt
   FAI_CONFIG_SRC=nfs://faiserver/srv/fai/config

demohost has 192.168.33.100 in hex C0A82164
Writing file /srv/tftp/fai/pxelinux.cfg/C0A82164 for demohost</code></pre>
</div></div>
<div class="paragraph"><p>À ce stade, vous devriez avoir une configuration faiserver de travail et vos clients devraient démarrer dans FAI et être en mesure d&#8217;installer l&#8217;un des exemples.</p></div>
<div class="paragraph"><p>Dans la section suivante, vous pouvez lire la planification de votre installation, adapter votre espace de configuration à vos besoins particuliers et étendre FAI à l&#8217;aide de hooks.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_custom_server_a_serveur_personnalisé"><a id="custom server"></a>Serveur personnalisé</h3>
<div class="paragraph"><p>Le faiseur et sa configuration n&#8217;est nullement statique. Il est possible de personnaliser et d'étendre votre serveur. Pour cela, reportez-vous à la section <a href="#Customizing your install server setup">[Customizing your install server setup]</a> dans <a href="#advanced">[advanced]</a>.</p></div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_a_id_plan_a_planifiez_votre_installation"><a id="plan"></a>Planifiez votre installation</h2>
<div class="sectionbody">
<div class="paragraph"><p>Avant de commencer votre installation, vous devriez investir beaucoup de temps dans la planification de votre installation. Une fois que vous êtes satisfait de votre concept d&#8217;installation, FAI peut faire toutes les tâches ennuyeuses et répétitives pour transformer vos plans en réalité. FAI ne peut pas faire de bonnes installations si votre concept est imparfait ou manque de quelques détails importants. Commencez à planifier l&#8217;installation en répondant aux questions suivantes:</p></div>
<div class="ulist"><ul>
<li>
<p>
Est-ce que je vais créer un cluster Beowulf ou dois-je installer des machines de bureau?
</p>
</li>
<li>
<p>
À quoi ressemble ma topologie LAN?
</p>
</li>
<li>
<p>
Ai-je un matériel uniforme? Le matériel sera-t-il uniforme à l&#8217;avenir?
</p>
</li>
<li>
<p>
Le matériel a-t-il besoin d&#8217;un noyau spécial?
</p>
</li>
<li>
<p>
Comment nommer les hôtes?
</p>
</li>
<li>
<p>
Comment les disques durs locaux doivent-ils être partitionnés?
</p>
</li>
<li>
<p>
Quelles applications seront éxécuté par les utilisateurs?
</p>
</li>
<li>
<p>
Les utilisateurs ont-ils besoin d&#8217;un système de mise en file d&#8217;attente?
</p>
</li>
<li>
<p>
Quel logiciel doit être installé?
</p>
</li>
<li>
<p>
Quels démons devraient être lancés, et à quoi devrait ressembler la configuration?
</p>
</li>
<li>
<p>
Quels systèmes de fichiers distants doivent être montés?
</p>
</li>
<li>
<p>
Comment effectuer les sauvegardes? How should backups be performed?
</p>
</li>
</ul></div>
<div class="paragraph"><p>Vous devez également penser à des comptes d&#8217;utilisateur, des imprimantes, un système de courrier, des travaux de cron, des cartes graphiques, l&#8217;initialisation double, le NIS, le NTP, le fuseau horaire, la disposition de clavier, l&#8217;exportation et le montage des annuaires via NFS et beaucoup d&#8217;autres choses. Donc, il ya beaucoup à faire avant de commencer une installation. Et rappelez-vous que la connaissance est le pouvoir, et c&#8217;est à vous de l&#8217;utiliser. L&#8217;installation et l&#8217;administration sont un processus et non un produit. FAI ne peut pas faire les choses que vous ne lui dites pas de faire.</p></div>
<div class="paragraph"><p>Mais vous ne devez pas commencer à partir de zéro. Examinez les fichiers et les scripts dans l&#8217;espace de configuration. Il ya beaucoup de choses que vous pouvez utiliser pour votre propre installation. Un bon article intitulé «Bootstrapping an Infrastructure» avec d&#8217;autres aspects de la construction d&#8217;une infrastructure est disponible sur <a href="http://www.infrastructures.org/papers/bootstrap/bootstrap.html">http://www.infrastructures.org/papers/bootstrap/bootstrap.html</a></p></div>
<div class="sect2">
<h3 id="_a_id_c3_a_l_8217_espace_de_configuration_et_ses_sous_répertoires"><a id="c3"></a>L&#8217;espace de configuration et ses sous-répertoires</h3>
<div class="paragraph"><p>L&#8217;espace de configuration est la collection d&#8217;informations sur la façon exacte d&#8217;installer un client. L&#8217;espace de configuration central pour tous les clients d&#8217;installation se trouve sur le serveur d&#8217;installation dans <em>/srv/fai/config</em> et ses sous-répertoires. Cela sera monté par les clients d&#8217;installation dans <em>/var/lib/fai/config</em>. La commande d&#8217;installation principale <code>fai(8)</code> utilise tous ces sous-répertoires dans l&#8217;ordre indiqué sauf pour les hooks.</p></div>
<div class="dlist"><dl>
<dt class="hdlist1">
<em>class/</em>
</dt>
<dd>
<p>
    Scripts et fichiers pour définir des classes et des variables.
</p>
</dd>
<dt class="hdlist1">
<em>disk_config/</em>
</dt>
<dd>
<p>
    Fichiers de configuration pour le partitionnement de disque, RAID logiciel, LVM et création de système de fichiers.
</p>
</dd>
<dt class="hdlist1">
<em>basefiles/</em>
</dt>
<dd>
<p>
Normalement , le fichier <em>base.tar.xz</em> (situé à l' intérieur du nfsroot) est extrait sur le client d&#8217;installation après la création des nouveaux systèmes de fichiers et avant l&#8217;installation du package. Il s&#8217;agit d&#8217;une image de base minimale, créée juste après avoir appelé debootstrap lors de la création du nfsroot sur le serveur d&#8217;installation. Si vous voulez installer une autre distribution que la nfsroot, vous pouvez mettre un fichier tar dans le sous-répertoire <em>basefiles/</em> et le nommer après une classe. Ensuite, la commande &#8216;ftar(8)` est utilisée pour extraire le fichier tar en fonction des classes définies. Ainsi, le fichier doit être nommé<em>&#8217; CLASS.tar.xz</em> et non <em>CLASS.base.tar.xz</em> . Cela se fait dans la tâche <em>extrbase</em>. Utilisez cette option si vous souhaitez installer une autre distribution ou une version différente de celle exécutée pendant l&#8217;installation.
</p>
<div class="paragraph"><p>Ce fichier de base peut également être reçu en fonction des classes FAI via HTTP ou FTP en définissant la variable FAI_BASEFILEURL. FAI téléchargera un fichier CLASSNAME.tar.xz (ou tgz, ou tar.gz, &#8230;) à partir de cette URL, si CLASSNAME correspond à une classe FAI.</p></div>
<div class="paragraph"><p>Exemple:</p></div>
</dd>
</dl></div>
<div class="listingblock">
<div class="content">
<pre><code>FAI_BASEFILEURL=http://fai-project.org/download/basefiles</code></pre>
</div></div>
<div class="paragraph"><p>Le dossier doit prendre en charge la liste des répertoires. FAI ne recherchera pas de fichiers potentiellement correspondants.</p></div>
<div class="paragraph"><p>Voir le chapitre <a href="#otherdists">[otherdists]</a> pour savoir comment installer différentes distributions.</p></div>
<div class="dlist"><dl>
<dt class="hdlist1">
<em>debconf/</em>
</dt>
<dd>
<p>
Ce répertoire contient toutes les données <code>debconf(7)</code>. Le format est le même que celui utilisé par <code>debconf-set-selections(8)</code>.
</p>
</dd>
<dt class="hdlist1">
<em>package_config/</em>
</dt>
<dd>
<p>
Les fichiers contenant des noms de classe contiennent des listes de progiciels à installer ou à désinstallé par &#8216;install_packages(8)<code>. Les fichiers nommés <em>&lt;CLASS&gt;.asc</em> sont ajoutés à la liste des clés utilisées par apt (à l&#8217;aide d&#8217; `apt-key(8)</code> ) pour les dépôts de paquets approuvés.
</p>
</dd>
<dt class="hdlist1">
<em>scripts/</em>
</dt>
<dd>
<p>
Scripts pour la personnalisation de votre site local. Utilisé par <code>fai-do-scripts(1)</code>.
</p>
</dd>
<dt class="hdlist1">
<em>files/</em>
</dt>
<dd>
<p>
Les Fichiers utilisés par les scripts de personnalisation. La plupart des fichiers se trouvent dans une structure de sous-arborescence qui reflète l&#8217;arborescence de répertoires ordinaire. Par exemple, les modèles de <em>nsswitch.conf</em> se trouvent dans <em>$FAI/files/etc/nsswitch.conf</em> et sont nommés en fonction des classes auxquelles ils doivent correspondre: <em>$FAI/files/etc/nsswitch.conf/NIS</em> est la version de <em>/etc/nsswitch.conf</em> à utiliser pour la classe NIS. Notez que le contenu du répertoire n&#8217;est pas automatiquement copié sur la machine cible, mais qu&#8217;il doit être explicitement copié par des scripts de personnalisation à l&#8217;aide de la commande <code>fcopy(8)</code>
.
</p>
</dd>
<dt class="hdlist1">
<em>hooks/</em>
</dt>
<dd>
<p>
    Les hooks sont des programmes ou des scripts définis par l&#8217;utilisateur, qui sont appelés pendant le processus d&#8217;installation. cela peut étendre ou remplacer les tâches par défaut. Le nom du fichier doit être de format <em>taskname.CLASSNAME[.sh]</em>. Un hook appelé <code>updatebase.DEBIAN</code> est exécuté avant la mise à jour de la tâche <code>updatebase</code> et seulement si l&#8217;installation du client appartient à la classe DEBIAN.
</p>
</dd>
</dl></div>
</div>
<div class="sect2">
<h3 id="_a_id_defining_classes_a_définition_des_classes"><a id="defining classes"></a>Définition des classes</h3>
<div class="paragraph"><p>Il existe différentes possibilités pour définir des classes:
. Certaines classes par défaut sont définies pour chaque hôte: DEFAULT, LAST et son nom d&#8217;hôte.
. Les classes peuvent être répertoriées dans un fichier.
. Les classes peuvent être dynamiquement définies par des scripts.</p></div>
<div class="paragraph"><p>La dernière option est une fonctionnalité très intéressante, puisque ces scripts définiront des classes est un moyen très flexible. Par exemple, plusieurs classes peuvent être définies uniquement si certains matériels sont identifiés ou si une classe est définie en fonction des informations de sous-réseau du réseau.</p></div>
<div class="paragraph"><p>Tous les noms de classes, sauf le nom d&#8217;hôte, sont écrits en majuscules.ILs ne doivent pas contenir un trait d&#8217;union, un dièse, un Point-Virgule OÜ un point, mais PEUVENT contenir des characters de soulignement et des Chiffres.</p></div>
<div class="paragraph"><p>La Tache <em>defclass</em> Appelle la commande <code>fai-class(1)</code> pour definir les classes. Tous les scripts correspondant <em>^[0-9][0-9]*</em> (qui Commencent Avec Deux Chiffres) Dans le sous-repertoire <em>$FAI/class</em> sont exécutées afin de definir les classes. Tout ce qui is affiché sur STDOUT est automatiquement definie Comme une classe. pour Plus d&#8217;informations sur Les définisions de Classe , lire les pages de manuel versent <code>fai-class(1)</code>. Le script <em>50-host-classes</em> (voir ci - dessous la version allégée) est utilisé pour les définir des classes en fonction du nom d&#8217;hôte.</p></div>
<div class="listingblock">
<div class="content">
<pre><code># use a list of classes for our demo machines
case $HOSTNAME in
    demohost)
        echo "FAIBASE GRUB DHCPC DEMO" ;;
    xfcehost)
        echo "FAIBASE GRUB DHCPC DEMO XORG XFCE";;
    faiserver)
        echo "FAIBASE DEBIAN DHCPC DEMO FAISERVER" ;;
    *)
        echo "FAIBASE GRUB DHCPC" ;;
esac</code></pre>
</div></div>
<div class="paragraph"><p>Les noms d&#8217;hôtes doivent Rarement Être utilisé Pour Les Fichiers de configuration dans l&#8217;Espace de configuration.à la place une classe Doit Être definie et ensuite ajouté Pour un hôte Donné. En effet, la Plupart du Temps les Données de configuration ne sont pas Spécifiques au d&#8217;nom hôte, mais peut etre partager entre differants hôtes./p&gt;</p></div>
<div class="paragraph"><p>L&#8217;ordre des classes est important car Elle Définit la priorité des classes de Faible à Élevé.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_classvariables_a_définition_des_variables"><a id="classvariables"></a>Définition des Variables</h3>
<div class="paragraph"><p>La Tache <em>defvar</em> definit les variables pour l&#8217;installation du client. Les variables sont définies par les scripts Dans la <em>class/*.var</em>. Toutes les variables Globales PEUVENT Être définies Dans <em>DEFAULT.var</em>. Pour certains groupes d&#8217;hôtes utiliser un Fichier de classe ou Pour un seul hôte utiliser le Fichier <code>$HOSTNAME</code> <em>.var</em> . Ici aussi, il est utile d'étudier Tous les exemples.</p></div>
<div class="paragraph"><p>Les variables suivantes sont utilisées dans les exemples et peuvent etre aussi utiles pour votre installation:</p></div>
<div class="dlist"><dl>
<dt class="hdlist1">
FAI_ACTION
</dt>
<dd>
<p>
Réglez les actions que doit éffectuer FAI. Normalement, ceci se fait par <code>fai-chboot(8)</code>. Si vous ne pouvez pas utiliser cette commande, définir la variable dans le script <em>LAST.var</em>.
</p>
</dd>
<dt class="hdlist1">
FAI_ALLOW_UNSIGNED
</dt>
<dd>
<p>
Si défini à 1, FAI Permet l&#8217;installation de de paquets à partir de référentiels non Signés.
</p>
</dd>
<dt class="hdlist1">
CONSOLEFONT
</dt>
<dd>
<p>
La police de qui est chargée lors de l&#8217;installation par <code>setfont(8)</code>.
</p>
</dd>
<dt class="hdlist1">
KEYMAP
</dt>
<dd>
<p>
Définit les Fichiers de mappage du clavier Dans <em>/usr/share/keymaps</em> et <em>$FAI/files</em>. Vous ne Devez pas spécifier le chemin complet, puisque ce fichier sera localisé automatiquement.
</p>
</dd>
<dt class="hdlist1">
ROOTPW
</dt>
<dd>
<p>
Le mot de passe root chiffré pour le nouveau système. Vous pouvez utiliser &#8216;crypt(3)<code>, md5 et d&#8217; Autres types de hachage pour le mot de passe. Utilisez `mkpasswd(1)</code> pour créer le hachage d&#8217;un certain mot de passe. Par exemple, pour Générer le hachage MD5 pour l&#8217;utilisation du mot de passe.
</p>
</dd>
</dl></div>
<div class="listingblock">
<div class="content">
<pre><code>$ echo "yoursecrectpassword" | mkpasswd -Hmd5 -s</code></pre>
</div></div>
<div class="dlist"><dl>
<dt class="hdlist1">
UTC
</dt>
<dd>
<p>
Réglez l&#8217;horloge du matériel à UTC si <em>UTC=yes</em>. Sinon, régler l&#8217;horloge à l&#8217;heure locale. Voir <code>clock(8)</code> pour en plus d&#8217;informations.
</p>
</dd>
<dt class="hdlist1">
TIMEZONE
</dt>
<dd>
<p>
Est-ce que le fichier d&#8217;initialisation par rapport à <em>/usr/share/zoneinfo/</em>' indique votre fuseau horaire. Par exemple: <em>TIMEZONE=Europe/Berlin</em>.
</p>
</dd>
<dt class="hdlist1">
MODULESLIST
</dt>
<dd>
<p>
Une liste des modules du Noyau qui sont chargés pendent Le démarrage du nouveau systême (Écrit dans /etc/modules).
</p>
</dd>
</dl></div>
</div>
<div class="sect2">
<h3 id="_a_id_diskconfig_a_configuration_du_disque_dur"><a id="diskconfig"></a>Configuration du disque dur</h3>
<div class="paragraph"><p>L&#8217;outil <code>setup-storage(8)</code> lit le fichier dans <em>$FAI/disk_config</em> pour la configuration du disque. Ce fichier décrit comment tous les disques Locaux devrons etre partitionné, Quels types de Systèmes de Fichiers doivent etre écris (Comme ext3/4, xfs, btrfs), et où ils seront Montés. Vous pouvez aussi créer des configurations RAID logiciel et LVM en Utilisant le Fichier de configuration. Il Est aussi possible de la mise en Conservation de le partitionnage du disque ou de conserver Les Donnees sur CERTAINES partitions.</p></div>
<div class="paragraph"><p>Pendant le Processus d&#8217;installation de tous les Systèmes de Fichiers Locaux Sont Montés par rapport à <em>/target</em>. Par exemple, si vous Specifiez le Point de montage <em>/home</em> Dans un Fichier de configuration de disque, ce sera le répertoire <em>/target/home</em> pendant le Processus d&#8217;installation et deviendra <em>/home</em> pour le nouveau systéme Installé.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_extrbase_a_extraction_du_fichier_de_base"><a id="extrbase"></a>Extraction du fichier de base</h3>
</div>
<div class="sect2">
<h3 id="_a_id_debconf_a_debconf_préconfiguration"><a id="debconf"></a>Debconf préconfiguration</h3>
</div>
<div class="sect2">
<h3 id="_a_id_repository_a_l_8217_accès_au_dépôt_de_paquetages"><a id="repository"></a>L&#8217;Accès au dépôt de paquetages</h3>
</div>
<div class="sect2">
<h3 id="_a_id_packageconfig_a_configuration_du_progiciel"><a id="packageconfig"></a>configuration du progiciel</h3>
<div class="paragraph"><p>Avant l&#8217;installation de de paquets, FAI va ajouter le contenu de Tous les Fichiers nommés <em>package_config/class.asc</em> à la liste des clés apt. Si votre depo locale est signé par votre keyid AB12CD34 vous pouvez Facilement ajouter cette clé, aussi FAI l&#8217;utilisera pendant l&#8217;installation. Utilisez cette commande pour Créer le fichier <em>CLASS.asc</em>:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>faiserver$ gpg -a --export AB12CD34 &gt; /srv/fai/config/package_config/MYCLASS.asc</code></pre>
</div></div>
<div class="paragraph"><p>Le script <code>install_packages(8)</code> installe les Logiciels Sélectionnés. Il lira tous les fichiers de configuration Dans <em>$FAI/package_config</em> Dont le nom correspond aux classes definie. La syntaxe est tres simple.</p></div>
<div class="listingblock">
<div class="content">
<pre><code># an example package class

PACKAGES taskinst
german

PACKAGES aptitude
adduser netstd ae
less passwd

PACKAGES remove
gpm xdm

PACKAGES aptitude GRUB
lilo- grub</code></pre>
</div></div>
<div class="paragraph"><p>Commentaires Commencent par un Dièse et se terminent à la fin de la ligne. Chaqué commande de paquetage commence par Le mot <em>PACKAGES</em> Suivi par un nom de commande, Ce qui correspond à l&#8217;outil de package Comme apt-get, aptitude ou yum par exemple. la commande qui définit la commandent qui sera utilisé pour installer les paquets nommés après cette commande. La liste de toutes les commandes disponibles peuvent Être listé en utilisant <em>install_packages -H</em>. Les paquets d&#8217;outils pris en charges son <em>aptitude, apt-get, smart, yast, yum, rpm, zypper</em></p></div>
<div class="dlist"><dl>
<dt class="hdlist1">
hold
</dt>
<dd>
<p>
Mettez un paquet en attente. Ce Paquet ne sera pas pris en charges par dpkg, pas exemple non mis à niveau.
</p>
</dd>
<dt class="hdlist1">
install
</dt>
<dd>
<p>
Installez Tous les paquets (en utilisant <code>apt-get</code>) Qui sont précise dans les lignes Suivantes. Si un tiret est ajouté au nom du paquet (sans espace intermédiaire), le paquet sera supprimé, pas installé. Tous les noms de paquets sont vérifiées pour les fautes d&#8217;orthographe. Tout paquet qui n&#8217;existe pas, seront retiré de la liste des paquets à l&#8217;installation. Soyer donc prudentes de ne pas mal orthographier les noms de paquets.
</p>
</dd>
<dt class="hdlist1">
install-norec
</dt>
<dd>
<p>
Comme install,mais sans installer les paquets recommandés.
</p>
</dd>
<dt class="hdlist1">
remove
</dt>
<dd>
<p>
Supprimer tous les paquets qui sont péciser dans les lignes suivantes. Annexer un + au nom du paquet si le paquet doit Être installé.
</p>
</dd>
<dt class="hdlist1">
taskinst
</dt>
<dd>
<p>
Installez tous les paquets appartenant aux tâches qui sont spécifiées dans les lignes suivantes à l&#8217;aide de <code>tasksel(1)</code>. Vous pouvez aussi utiliser <em>aptitude</em> pour installer les tâches.
</p>
</dd>
<dt class="hdlist1">
aptitude
</dt>
<dd>
<p>
Installez Ttus les paquets avec la commande <code>aptitude</code>. Ce sera la Valeur par défaut à l&#8217;avenir et pourra remplacer apt-get et taskinst. Aptitudes peut aussi installer les paquets
</p>
</dd>
<dt class="hdlist1">
aptitude-r
</dt>
<dd>
<p>
Idem aptitude avec l&#8217;option <em>--with-recommends</em>.
</p>
</dd>
<dt class="hdlist1">
unpack
</dt>
<dd>
<p>
Télécharge les paquets et décompresse seulement. Ne configure pas le paquet.
</p>
</dd>
<dt class="hdlist1">
dselect-upgrade
</dt>
<dd>
<p>
Defini la sélections des paquets en Utilisant les lignes suivantes et installe ou supprime les paquets précisés. Ces lignes sont le résultat de la commande <em>dpkg --get-selections</em>. Il est recommandé de ne pas utiliser ce format, puisque vous devez aussi specifiez tous les paquets qui ne sont pas installés en raison d&#8217;une dépendance ou recommandation. Il vaut mieux juste spécifier le paquet que vous voulez avoir, et de laisser FAI (et apt-get) résoudre les dépendances.
</p>
</dd>
</dl></div>
<div class="paragraph"><p>Plusieurs lignes avec des listes de noms de paquets séparés par des espaces suivent les directive PACKAGES. Toutes les dépendances sont résolues. Les paquetages avec suffixe <em>-</em> (par exemple, <em>lilo-</em>) seront supprimés au lieu d'être installés. L&#8217;ordre des paquet n&#8217;a pas d&#8217;importance. Si vous souhaitez installer des paquets d&#8217;une autre version que la valeur par défaut, vous pouvez ajouter le nom de la version au nom du paquet comme dans <em>openoffice.org/etch-backports</em>. Vous pouvez également spécifier une certaine version comme <em>apt=0.3.1</em>. Plus d&#8217;informations sur ces fonctionnalités sont décrites dans <code>aptitude(8)</code>.</p></div>
<div class="paragraph"><p>Une ligne qui contient la commande <em>PRELOADRM</em>, télécharge un fichier à l&#8217;aide de <code>wget(1)</code> dans un répertoire avant d&#8217;installer les packages. À l&#8217;aide du <em>file:</em> URL, ce fichier est copié de <code>$FAI_ROOT</code> vers le répertoire de téléchargement. Par exemple, le package <code>realplayer</code> a besoin d&#8217;une archive pour installer le logiciel, donc cette archive est téléchargée dans le répertoire <em>/root</em>. Après l&#8217;installation des paquets, ce fichier sera supprimé. Si le fichier ne doit pas être supprimé, utilisez plutôt la commande <em>PRELOAD</em>.</p></div>
<div class="paragraph"><p>Il est possible d&#8217;ajouter une liste de noms de classes après la commande pour apt-get. Ainsi, cette commande <em>PACKAGE</em> ne sera exécutée que si la classe correspondante est définie. Ainsi, vous pouvez combiner de nombreux petits fichiers dans le fichier DEFAULT. ATTENTION! Utilisez cette fonctionnalité uniquement dans le fichier DEFAULT pour garder tout simple. Voir ce fichier pour quelques exemples.</p></div>
<div class="paragraph"><p>Si vous souhaitez supprimer un nom de paquet d&#8217;une certaine classe faisait partie avant de cette classe , vous ne devez pas supprimer le nom du paquet classe, mais plutôt de lui ajouter un tiret (-). Cela garantira que le paquet est enlevé pendant une mise a jour sur des hôtes qui étaient Installé en utilisant l&#8217;ancienne définition de classe qui comprenait ce nom de paquet.</p></div>
<div class="paragraph"><p>Si vous spécifiez un paquet qui n&#8217;existe pas, ce paquet sera supprimé automatiquement de la liste d&#8217;installation uniquement si la commande <em>install</em> est utilisée.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_cscripts_a_scripts_de_personnalisation"><a id="cscripts"></a> Scripts de personnalisation</h3>
<div class="paragraph"><p>La commande <code>fai-do-scripts(1)</code> est appelée pour exécuter tous les scripts dans ce répertoire. Si un répertoire avec un nom de classe existe, tous les scripts correspondant à <em>^[0-9][0-9]*</em> sont exécutés par ordre alphabétique. Il est donc possible d&#8217;utiliser des scripts de différentes langues (shell, cfengine, Perl, Python, Ruby, expect,..) pour une classe.</p></div>
<div class="paragraph"><p>Ces scripts écrivent leur sortie dans différents fichiers journaux, selon le type de script. Par exemple, Tous les scripts shell écrivent leur journal dans <em>shell.log</em>.</p></div>
<div class="sect3">
<h4 id="_a_id_shell_a_scripts_shell"><a id="shell"></a>Scripts shell</h4>
<div class="paragraph"><p>La plupart des scripts sont des scripts Bourne shell. Les scripts shell sont utiles si la tâche de configuration ne doit seulement appeler certaines commandes shell ou créer un fichier à partir de zéro. Afin de ne pas écrire beaucoup de scripts courts, il est possible d&#8217;utiliser la commande <code>ifclass</code> pour tester si certaines classes sont définies.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>ifclass -o A B C</code></pre>
</div></div>
<div class="paragraph"><p>Vérifie si l&#8217;une des classes A, B ou C est définie. L&#8217;utilisation de -a (AND logique) vérifie si toutes les classes d&#8217;une liste sont définies. La commande ifclass C vérifie si seule la classe C est définie.</p></div>
<div class="paragraph"><p>Pour copier des fichiers avec des classes, utilisez la commande <code>fcopy(8)</code>. Si vous voulez extraire une archive à l&#8217;aide de classes, utilisez <code>ftar(8)</code>. Pour ajouter des lignes à un fichier de configuration, utilisez <code>ainsl(1)</code> au lieu de simplement <code>echo string &gt;&gt; filename</code>.</p></div>
<div class="paragraph"><p>FAI prend également en charge les scripts <em>zsh(1)</em> pendant la tâche de personnalisation. Dans les scripts, la variable <code>$classes</code> contient une liste séparée par des espaces avec les noms de toutes les classes définies.</p></div>
</div>
<div class="sect3">
<h4 id="_a_id_cfengine_a_scripts_cfengine"><a id="cfengine"></a>Scripts cfengine</h4>
<div class="paragraph"><p>CFEngine dispose d&#8217;un riche ensemble de fonctions pour modifier les fichiers de configuration existants, par exemple <em>LocateLineMatching, ReplaceAll, InsertLine, AppendIfNoSuchLine, HashCommentLinesContaining</em>. Mais il ne peut pas traiter les variables qui sont indéfinies. Si une variable n&#8217;est pas définie, l&#8217;ensemble du script cfengine s&#8217;arrêtera.</p></div>
<div class="paragraph"><p>Plus d&#8217;informations peuvent être trouvées dans la page de manuel <code>cfengine(8)</code> ou sur la page d&#8217;accueil cfengine <a href="http://www.cfengine.org">http://www.cfengine.org</a>.</p></div>
</div>
</div>
<div class="sect2">
<h3 id="_a_id_hooks_a_hooks"><a id="hooks"></a>Hooks</h3>
<div class="paragraph"><p>Les Hooks vous permettent de spécifier des fonctions ou des programmes qui sont exécutés à certaines étapes du processus d&#8217;installation. Avant qu&#8217;une tâche soit appelée, FAI recherche les hooks existants pour cette tâche et les exécute. Comme on peut s&#8217;y attendre, les classes sont également utilisées lors de l&#8217;appel de hooks. Les hooks sont exécutés pour chaque classe définie. Vous n&#8217;avez qu'à créer le hook avec le nom de la classe désirée et il sera utilisé. Si plusieurs hooks pour une tâche existent, ils sont appelés dans l&#8217;ordre défini par les classes. Si <em>debug</em> est inclus dans <code>$FAI_FLAG</code> l&#8217;option <em>-d</em> est passée à tous les hooks, donc vous pouvez déboguer vos propres hooks. Si certaines tâches par défaut doivent être ignorées, utilisez la sous-routine <em>skiptask</em> et une liste de tâches par défaut comme paramètres. Dans les exemples fournis, les hooks de la classe CENTOS ignorent certaines tâches spécifiques de Debian.</p></div>
<div class="paragraph"><p>Le répertoire <em>$FAI/hooks/</em>' contient tous les hooks. Un hook est un fichier exécutable qui suit le nom de tâche <em>taskname.CLASSNAME[.sh]</em>' (par exemple, <em>repository.CENTOS</em> ou <em>savelog.LAST.sh</em>), un nom de tâche et un nom de classe séparés par un point, éventuellement suivi de '.sh. Le nom de la tâche spécifie la tâche devant précéder l&#8217;exécution de ce hook, si la classe spécifiée est définie pour le client d&#8217;installation. Voir la section <a href="#tasks">[tasks]</a> pour une liste complète des tâches par défaut pouvant être utilisées.</p></div>
<div class="paragraph"><p>Un hook du formulaire <em>hookprefix.classname</em> ne peut pas définir de variables pour le script d&#8217;installation, car il s&#8217;agit d&#8217;un sous-processus. Mais vous pouvez utiliser n&#8217;importe quel exécutable binaire ou n&#8217;importe quel script que vous avez écrit. Les hooks qui ont le suffixe <em>.sh</em> (par exemple, 'partition.DEFAULT.sh) doivent être des scripts Bourne shell et sont sourcé. Il est donc possible de redéfinir des variables pour les scripts d&#8217;installation.</p></div>
<div class="paragraph"><p>Dans la première partie de FAI, tous les hooks avec le préfixe <em>confdir</em> sont appelés. Ces hooks ne peuvent pas être localisés dans l&#8217;espace de configuration, car il n&#8217;est pas encore disponible. Par conséquent, ces hooks sont les seuls hooks situés dans <code>$nfsroot</code><em>/$FAI/hooks</em> sur le serveur d&#8217;installation. Tous les autres hooks se trouvent dans <em>$FAI_CONFIGDIR/hooks</em> sur le serveur d&#8217;installation.</p></div>
<div class="paragraph"><p>Tous les hooks appelés avant la définition des classes ne peuvent utiliser que les classes suivantes: <em>DEFAULT $HOSTNAME LAST</em>. Si un hook pour la classe <em>DEFAULT</em> doit être appelé uniquement si aucun hook pour la classe <code>$HOSTNAME</code> n&#8217;est disponible, insérez ces lignes sur le hook par défaut:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>hookexample.DEFAULT:

#! /bin/sh

# skip DEFAULT hook if a hook for $HOSTNAME exists
scriptname=$(basename $0 .DEFAULT)
[-f $FAI/hooks/$scriptname.$HOSTNAME ] &amp;&amp; exit
# here follows the actions for class DEFAULT
.
.</code></pre>
</div></div>
<div class="paragraph"><p>Quelques exemples de ce que les hooks pourraient être utilisés:</p></div>
<div class="ulist"><ul>
<li>
<p>
Charger les modules du noyau avant que les classes soient définies dans $FAI/class.
</p>
</li>
<li>
<p>
Envoyez un courriel à l&#8217;administrateur si l&#8217;installation est terminée.
</p>
</li>
<li>
<p>
Installez un client sans disque et sautez le partitionnement de disque local.
</p>
</li>
<li>
<p>
Jetez un oeil à hooks/debconf.IMAGE pour savoir comment cloner une machine en utilisant une image de système de fichiers.
</p>
</li>
</ul></div>
</div>
<div class="sect2">
<h3 id="_a_id_faiflags_a_fai_flags"><a id="faiflags"></a>FAI flags</h3>
<div class="paragraph"><p>La variable <code>$FAI_FLAGS</code> contient une liste de flags séparés par des espaces. Les flags suivants sont connus:</p></div>
<div class="dlist"><dl>
<dt class="hdlist1">
verbose
</dt>
<dd>
<p>
Créez une sortie verbeuse pendant l&#8217;installation. Cela doit toujours être le premier flag, de sorte que les définitions consécutives des flags seront affichées verbeusement.
</p>
</dd>
<dt class="hdlist1">
debug
</dt>
<dd>
<p>
Créer une sortie de débogage. Aucune installation sans assistance n&#8217;est effectuée. Pendant l&#8217;installation du paquet, vous devez répondre à toutes les questions des scripts postinstall sur la console du client. Beaucoup d&#8217;informations de débogage seront imprimées. Ce flag n&#8217;est utile que pour les développeurs FAI.
</p>
</dd>
<dt class="hdlist1">
sshd
</dt>
<dd>
<p>
Démarrez le démon ssh pour activer les connexions à distance. Vous pouvez ensuite vous connecter en tant que root à tous les clients d&#8217;installation pendant l&#8217;installation. Le mot de passe par défaut est fai et peut être modifié en définissant FAI_ROOTPW dans nfsroot.conf(5). Pour vous connecter à partir de votre serveur vers le client d&#8217;installation (nommé demohost dans cet exemple), utilisez:
</p>
</dd>
</dl></div>
<div class="listingblock">
<div class="content">
<pre><code>$ ssh root@demohost
Warning: Permanently added 'demohost,192.168.33.100' to the list of known hosts.
root@demohost's password:</code></pre>
</div></div>
<div class="paragraph"><p>Ce n&#8217;est que le mot de passe root pendant le processus d&#8217;installation, pas pour le nouveau système installé. Vous pouvez également vous connecter sans mot de passe lorsque vous utilisez <code>$SSH_IDENTITY</code>.</p></div>
<div class="dlist"><dl>
<dt class="hdlist1">
createvt
</dt>
<dd>
<p>
Créez deux terminaux virtuels et exécutez un bash si <em>ctrl-c</em> est tapé dans le terminal de console. Vous pouvez accéder aux terminaux supplémentaires en tapant <em>Alt-F2</em> ou <em>Alt-F3</em>. Sinon, aucun terminal n&#8217;est disponible et la saisie <em>ctrl-c</em> va redémarrer le client d&#8217;installation. La définition de ce flag est utile pour le débogage. Si vous voulez une installation qui ne devrait pas être interruptible, ne définissez pas ce flag.
</p>
</dd>
<dt class="hdlist1">
menu
</dt>
<dd>
<p>
Cela permet à un menu utilisateur de sélectionner un profil. Tous les fichiers <code>class/*.profile</code> sont lus et un menu basé sur des curses sera créé.
</p>
</dd>
<dt class="hdlist1">
reboot
</dt>
<dd>
<p>
Redémarrez le client d&#8217;installation une fois l&#8217;installation terminée sans taper RETURN sur la console. Si ce drapeau n&#8217;est pas défini, et que error.log contient quelque chose, le client d&#8217;installation s&#8217;arrêtera et attendra que vous appuyez sur RETURN. Si aucune erreur ne s&#8217;est produite, le client redémarre automatiquement automatiquement.
</p>
</dd>
<dt class="hdlist1">
halt
</dt>
<dd>
<p>
Arrêtez le client d&#8217;installation à la fin de l&#8217;installation, au lieu de redémarrer dans le nouveau système.
</p>
</dd>
<dt class="hdlist1">
initial
</dt>
<dd>
<p>
Utilisé par <code>setup-storage(8)</code>. Les partitions marquées avec <code>preserve_reinstall</code> sont préservées à moins que ce flag ne soit défini. Souvent, ce drapeau est placé dans un <em>fichierclass/*.var</em> en utilisant le paramètre <em>flag_initial=1</em>.
</p>
</dd>
</dl></div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_a_id_install_a_fai_installe_votre_planification"><a id="install"></a> FAI installe votre planification</h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_la_première_partie_d_8217_une_installation">La première partie d&#8217;une installation</h3>
<div class="paragraph"><p>Après le démarrage du noyau, il monte le système de fichiers racine via NFS à partir du serveur d&#8217;installation et démarre le script <em>/usr/sbin/fai</em> <span class="footnote"><br />[Puisque le système de fichiers racine sur les clients est monté via NFS, <code>fai</code> est localisé in <em>/srv/fai/nfsroot/usr/sbin</em> sur le servuer d&#8217;installation.]<br /></span>. Ce script contrôle la séquence de l&#8217;installation. Aucun autre script dans <em>/etc/init.d/</em> n&#8217;est utilisé.</p></div>
<div class="paragraph"><p>L&#8217;espace de configuration est rendu disponible via la méthode configurée (un montage NFS par défaut) du serveur d&#8217;installation au chemin défini dans $FAI <span class="footnote"><br />[ <em>$FAI</em> est une variable interne utilisée par les scripts FAI. Par défaut, le chemin est <em>/var/lib/fai/config</em>.]<br /></span>.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_bootmesg_a_messages_de_boot"><a id="bootmesg"></a>Messages de boot</h3>
<div class="paragraph"><p>Lorsque vous démarrez le client d&#8217;installation à partir de la carte réseau avec PXE, vous obtiendrez des messages comme ceci:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>Managed PC Boot Agent (MBA) v4.00
Pre-boot eXecution Environment (PXE) v2.00
DHCP MAC ADDR: 00 A2 A3 04 05 06
DHCP.../

CLIENT MAC ADDR: 00 A2 A3 04 05 06  GUID: 3D6C4552
CLIENT IP: 192.168.33.100 MASK: 255.255.255.0  DHCP IP: 192.168.33.250
GATEWAY IP: 192.168.33.1

!PXE entry point found (we hope) at 9854:0106 via plan A
UNDI code segment at: 9854 len 5260
UNDI data segment at: 921D len 63A2
Getting cached packet  01 02 03
My Ip address seems to be C0A82164 192.168.33.100
ip=192.168.33.100:192.168.33.250:192.168.33.1:255.255.255.0
BOOTIF=01-00-A2-A3-04-05-06
SYSUUID=
TFTP prefix: fai/
Trying to load pxelinux.cfg/C0A82164

Loading vmlinuz-3.16.0-4-amd64..................
Loading initrd.img-3.16.0-4-amd64......................ready.</code></pre>
</div></div>
<div class="paragraph"><p>À ce stade, le client d&#8217;installation a réussi à recevoir le réseau Config via DHCP et le noyau et initrd via TFTP. Il démarre maintenant Le noyau Linux et l&#8217;initrd. Si tout allait bien, l&#8217;initrd Monte nfsroot <span class="footnote"><br />[ <em>/srv/fai/nfsroot</em> depuis le serveur d&#8217;installation via NFS]<br /></span> Et les scripts FAI sont lancés. La première chose que vous voyez est le message en rouge de copyright FAI.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>             -------------------------------------------------
                   Fully Automatic Installation  -  FAI

                   5.3.3~bpo8+2  (c) 1999-2017
               Thomas Lange  &lt;lange@informatik.uni-koeln.de&gt;
             -------------------------------------------------

Calling task_confdir
Kernel currently running: Linux 3.16.0-4-amd64 x86_64 GNU/Linux
Kernel parameters: BOOT_IMAGE=vmlinuz-3.16.0-4-amd64 initrd=initrd.img-3.16.0-4-amd64 \
 rw aufs ip=dhcp root=192.168.33.250:/srv/fai/nfsroot FAI_FLAGS=verbose,sshd,createvt\
 FAI_CONFIG_SRC=nfs://faiserver/srv/fai/cskoeln FAI_ACTION=install quiet\
 BOOTIF=01-00-a2-a3-04-05-06
Reading /tmp/fai/boot.log
FAI_FLAGS: verbose sshd createvt
Setting SERVER=faiserver. Value extracted from FAI_CONFIG_SRC.
FAI_CONFIG_SRC is set to nfs://faiserver/srv/fai/config
Configuration space faiserver:/srv/fai/config mounted to /var/lib/fai/config
Calling task_setup
FAI_FLAGS: verbose sshd createvt
15 Jan 13:22:37 ntpdate[1533]: step time server 192.168.33.250 offset -0.342793 sec
Press ctrl-c to interrupt FAI and to get a shell
Starting FAI execution - 20170115_132237
Calling task_defclass
fai-class: Defining classes.
Executing /var/lib/fai/config/class/10-base-classes.
10-base-classes      OK.
Executing /var/lib/fai/config/class/20-hwdetect.source.
Loading kernel module md-mod
20-hwdetect.source   OK.
Executing /var/lib/fai/config/class/50-host-classes.
50-host-classes      OK.
List of all classes: DEFAULT LINUX AMD64 FAIBASE DHCPC DEMO GRUB client01 LAST</code></pre>
</div></div>
<div class="paragraph"><p>Vous pouvez également voir la liste des classes FAI, qui sont définies pour ce hôte. Cette liste est très importante pour le reste de l&#8217;installation.</p></div>
<div class="paragraph"><p>La première tâche est appelée <em>confdir</em>, qui est chargée de Accès à l&#8217;espace de configuration. Ici, nous utilisons un montage NFS à partir de l&#8217;installation Comme vous pouvez le voir sur la console (et plus tard dans les journaux).</p></div>
<div class="listingblock">
<div class="content">
<pre><code>FAI_CONFIG_SRC is set to nfs://faiserver/srv/fai/config
Configuration space faiserver:/srv/fai/config mounted to /var/lib/fai/config</code></pre>
</div></div>
<div class="paragraph"><p>Avant de lancer l&#8217;installation (<code>$FAI_ACTION=install</code>), l&#8217;ordinateur Bip trois fois. Donc, faites attention quand vous entendez trois bips mais vous Ne voulez pas effectuer une installation et laisser FAI effacer toutes vos données sur Le disque local!</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_reboot_a_redémarrage_de_l_8217_ordinateur_dans_le_nouveau_système"><a id="reboot"></a>Redémarrage de l&#8217;ordinateur dans le nouveau système</h3>
<div class="paragraph"><p>Pour redémarrer l&#8217;ordinateur pendant ou à la fin de l&#8217;installation, vous devez utiliser la commande <code>faireboot</code> en faveur de la commande de redémarrage normal. Utilisez aussi <code>faireboot</code> si vous êtes connecté depuis la télécommande. Si l&#8217;installation n&#8217;est pas terminée, utilisez <em>faireboot -s</em>, donc les fichiers journaux sont également copiés sur le serveur d&#8217;installation.</p></div>
<div class="paragraph"><p>Si l&#8217;installation est terminée, l&#8217;ordinateur doit démarrer un petit système Debian. Vous pouvez vous connecter en tant que <em>demo</em> ou <em>root</em> avec le mot de passe <em>fai</em>.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_isetup_a_démarrage_de_fai_tâche_confdir"><a id="isetup"></a>Démarrage de FAI (tâche confdir)</h3>
<div class="paragraph"><p>Une fois le client d&#8217;installation démarré, seul le script <em>/usr/sbin/fai</em> est exécuté. Il effectuera une initialisation minimale. La variable <code>$FAI_CONFIG_SRC</code> <span class="footnote"><br />[Il a été défini sur la ligne de commande du noyau]<br /></span> est utilisée pour accéder à l&#8217;espace de configuration FAI qui est alors disponible dans le répertoire <code>$FAI</code> <span class="footnote"><br />[/var/lib/fai/config]<br /></span>. FAI ne se déroulera pas sans l&#8217;espace de configuration.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_iclass_a_définition_de_classes_et_de_variables_tâches_defclass_et_defvar"><a id="iclass"></a>Définition de classes et de variables (tâches defclass et defvar)</h3>
<div class="paragraph"><p>La commande <code>fai-class(1)</code> exécute des scripts dans <em>$FAI/class</em> pour définir des classes. Si les scripts écrivent une chaîne sur stdout, cela sera défini comme une classe. Lisez tous les détails dans la page de manuel de <code>fai-class(1)</code>.</p></div>
<div class="paragraph"><p>Après avoir défini les classes, chaque fichier correspondant à <em>.var</em> avec un préfixe qui correspond à une classe définie provient de variables définies. Il doit contenir le code shell vaild.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_ipartition_a_partitionnement_de_disques_locaux_création_de_systèmes_de_fichiers_tâches_de_partitionnement"><a id="ipartition"></a>Partitionnement de disques locaux, création de systèmes de fichiers (tâches de partitionnement)</h3>
<div class="paragraph"><p>Pour le partitionnement du disque, un fichier de configuration de disque de <em>$FAI/disk_config</em> est sélectionné à l&#8217;aide de classes.</p></div>
<div class="paragraph"><p>Le format de la configuration du disque est similaire à un fichier fstab.</p></div>
<div class="paragraph"><p>L&#8217;outil de partitionnement <code>setup-storage(8)</code> exécute toutes les commandes nécessaires à la création de la disposition de la partition du disque, du RAID logiciel, du LVM et de la création des systèmes de fichiers. Lisez la page de manuel de <code>setup-storage(8)</code> pour une description détaillée et quelques exemples du format.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_ipreseed_a_préréglage_debconf_tâche_debconf"><a id="ipreseed"></a>Préréglage Debconf (tâche debconf)</h3>
<div class="paragraph"><p>Les fichiers dans <em>$FAI/debconf</em> sont utilisés par <code>debconf(7)</code> habituel en présselectionnant si les noms de fichier correspondent à un nom de classe.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_ipackages_a_installation_de_progiciels_tâche_instsoft"><a id="ipackages"></a>Installation de progiciels (tâche instsoft)</h3>
<div class="paragraph"><p>La commande <code>install_packages(8)</code> lit les fichiers de configuration à partir de <em>$FAI/package_config</em> en classe et installe des progiciels sur le nouveau système de fichiers.</p></div>
<div class="paragraph"><p>Il installe les paquets en utilisant <code>apt-get(8)</code>, <code>aptitude(1)</code>, <code>yum</code> ou d&#8217;autres outils de paquetage sans aucune interaction manuelle nécessaire. Les paquets sont également résolus par les outils de paquets.</p></div>
<div class="paragraph"><p>Le format des fichiers de configuration est décrit dans <a href="#packageconfig">[packageconfig]</a>.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_icscripts_a_personnalisation_spécifique_au_site_task_configure"><a id="icscripts"></a>Personnalisation spécifique au site (task configure)</h3>
<div class="paragraph"><p>Souvent, les configurations par défaut des progiciels ne répondent pas à vos besoins spécifiques au site. Vous pouvez appeler des scripts arbitraires qui ajustent la configuration du système. Par conséquent, la commande <code>fai-do-scripts(1)</code> exécute des scripts dans <em>$FAI/scripts</em> d&#8217;une manière basée sur la classe. Il est possible d&#8217;avoir plusieurs scripts de différents types (shell, cfengine, &#8230;) à exécuter pour une classe.</p></div>
<div class="paragraph"><p>L&#8217;ensemble de scripts par défaut dans <em>$FAI/scripts</em> inclut des exemples d&#8217;installation de machines Debian et CentOS. Ils définissent le mot de passe root, ajoutent un compte utilisateur démo, paramétrent le fuseau horaire, configurent le réseau pour DHCP ou utilisent une adresse IP fixe,la configuration grub et plus encore. Ils devraient faire un travail raisonnable pour votre installation. Vous pouvez les modifier ou ajouter de nouveaux scripts pour répondre à vos besoins locaux.</p></div>
<div class="paragraph"><p>Plus d&#8217;informations sur ces scripts sont décrits dans <a href="#cscripts">[cscripts]</a>.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_isavelog_a_enregistrement_des_fichiers_journaux_tâche_savelog"><a id="isavelog"></a>Enregistrement des fichiers journaux (tâche savelog)</h3>
<div class="paragraph"><p>Lorsque toutes les tâches sont terminées, les fichiers journaux sont écrits dans <em>/var/log/fai/$HOSTNAME/install/_<span class="footnote"><br />[<em>/var/log/fai/localhost/install/</em> est un lien vers ce répertoire.]<br /></span> sur le nouveau système et sur le compte sur le serveur d&#8217;installation si <code>$LOGUSER</code> est défini. Il est également possible de spécifier un autre hôte comme enregistrement en enregistrant la destination via la variable <code>$LOGSERVER</code>. Si <code>$LOGSERVER</code> n&#8217;est pas défini, FAI utilise la variable <code>$SERVER</code> qui n&#8217;est définie que lors d&#8217;une installation initiale (par get-boot-info). Assurez-vous de définir <code>$LOGSERVER</code> dans un script _class/*.var</em> si vous utilisez l&#8217;action <em>softupdate</em>.</p></div>
<div class="paragraph"><p>De plus, deux liens symboliques seront créés pour indiquer le dernier répertoire écrit. Le lien symbolique <em>last</em> pointe vers le répertoire journal de la dernière action FAI exécutée. Les liens symboliques <em>last-install</em> et <em>last-sysinfo</em> pointent vers le répertoire avec la dernière action correspondante. Par défaut, les fichiers journaux seront copiés sur le serveur de journal à l&#8217;aide de scp. Vous pouvez utiliser la variable <code>$FAI_LOGPROTO</code> dans le fichier <em>fai.conf(5)</em> pour choisir une autre méthode d&#8217;enregistrement des journaux sur le serveur distant. Voici un exemple de structure de lien symbolique:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>lrwxrwxrwx   1 fai fai   23 Dec  2  2013 last-sysinfo -&gt; sysinfo-20131202_161237
drwxr-xr-x   2 fai fai 4096 Dec  2  2013 sysinfo-20131202_161237
drwxr-xr-x   2 fai fai 4096 Feb 14  2014 install-20140214_142150
drwxr-xr-x   2 fai fai 4096 Dec  2 11:47 install-20141202_113918
lrwxrwxrwx   1 fai fai   23 Dec  4 13:22 last-install -&gt; install-20141204_131351
lrwxrwxrwx   1 fai fai   23 Dec  4 13:22 last -&gt; install-20141204_131351
drwxr-xr-x   2 fai fai 4096 Dec  4 13:22 install-20141204_131351</code></pre>
</div></div>
<div class="paragraph"><p>Vous trouverez des exemples de fichiers journaux à l&#8217;adresse <a href="http://fai-project.org/logs">http://fai-project.org/logs</a>.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_ireboot_a_redémarrez_le_nouveau_système_installé"><a id="ireboot"></a>Redémarrez le nouveau système installé</h3>
<div class="paragraph"><p>Avant de redémarrer, le client d&#8217;installation appelle <code>fai-chboot -d &lt;hostname&gt;</code> sur le serveur d&#8217;installation, pour désactiver sa propre configuration PXELINUX. Sinon, il redémarrera l&#8217;installation lors de la prochaine initialisation. Normalement, cela devrait démarrer le nouveau système installé à partir de son second périphérique d&#8217;amorçage, le disque dur local.</p></div>
<div class="paragraph"><p>À la fin, le système est automatiquement redémarré si "reboot" a été ajouté à <code>$FAI_FLAGS</code>.</p></div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_a_id_advanced_a_chapitre_avancés_de_fai"><a id="advanced"></a>Chapitre avancés de FAI</h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_a_id_checkbootp_a_vérification_des_paramètres_reçus_des_serveurs_dhcp"><a id="checkbootp"></a>Vérification des paramètres reçus des serveurs DHCP</h3>
<div class="paragraph"><p>Si le client d&#8217;installation démarre, vous pouvez vérifier si toutes les informations provenant du démon DHCP sont correctement reçues. Les informations reçues sont écrites dans <em>/tmp/fai/boot.log</em>. Un exemple de résultat d&#8217;une requête DHCP peut être trouvé dans les fichiers journaux d&#8217;exemple.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_fai_monitor_a_surveillance_de_plusieurs_installations_clientes"><a id="fai-monitor"></a>Surveillance de plusieurs installations clientes</h3>
<div class="paragraph"><p>Vous pouvez surveiller l&#8217;installation de tous les clients d&#8217;installation avec la commande <code>fai-monitor(8)</code>. Tous les clients vérifient si ce démon est en cours d&#8217;exécution sur le serveur d&#8217;installation (ou sur l&#8217;ordinateur défini par la variable $monserver). Chaque fois qu&#8217;une tâche démarre ou se termine, un message est envoyé. Le démon du moniteur FAI imprime ces messages à la sortie standard. Il ya aussi un frontend graphique disponible, appelé <code>fai-monitor-gui(1)</code>.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>$  fai-monitor | fai-monitor-gui - &amp;</code></pre>
</div></div>
</div>
<div class="sect2">
<h3 id="_a_id_mac_a_collecte_d_8217_adresses_ethernet_pour_plusieurs_hôtes"><a id="mac"></a>Collecte d&#8217;adresses Ethernet pour plusieurs hôtes</h3>
<div class="paragraph"><p>Vous devez collecter toutes les adresses Ethernet (MAC) des clients à l&#8217;installation et affecter un nom d&#8217;hôte et une adresse IP à chaque client. Pour collecter les adresses MAC, démarrez vos clients pour l&#8217;installation. Vous pouvez déjà le faire avant que n&#8217;importe quel démon DHCP s&#8217;exécute dans votre sous-réseau. Ils échoueront à démarrer (en raison du manque de DHCP ou de TFTP manquant), mais vous pouvez toujours collecter les adresses MAC.</p></div>
<div class="paragraph"><p>Pendant que les clients d&#8217;installation démarrent, ils envoient des paquets de diffusion au LAN. Vous pouvez enregistrer les adresses MAC de ces hôtes en exécutant simultanément la commande suivante sur le serveur:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>faiserver# tcpdump -qtel broadcast and port bootpc &gt;/tmp/mac.list</code></pre>
</div></div>
<div class="paragraph"><p>Une fois que les hôtes ont été envoyés, certains paquets de diffusion annule <code>tcpdump</code> en tapant <em>ctrl-c</em>. Vous obtenez une liste de toutes les adresses MAC uniques avec ces commandes:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>faiserver$ perl -ane 'print "\U$F[0]\n"' /tmp/mac.list|sort|uniq</code></pre>
</div></div>
<div class="paragraph"><p>Après cela, vous n&#8217;avez qu'à assigner ces adresses MAC aux noms d&#8217;hôte et aux adresses IP (/etc/ethers et /etc/hosts ou aux cartes NIS correspondantes). Avec ces informations, vous pouvez configurer votre démon DHCP (voir la section [bootdhcp]). <span class="footnote"><br />[Je recommande d'écrire les adresses MAC (les trois derniers octets suffiront si vous avez des cartes réseau du même fournisseur) et le nom d&#8217;hôte à l&#8217;avant de chaque châssis.]<br /></span></p></div>
<div class="sect3">
<h4 id="_débogage_du_trafic_réseau">Débogage du trafic réseau</h4>
<div class="paragraph"><p>Si le client ne peut démarrer correctement à partir de la carte réseau, utilisez <code>tcpdump(8)</code> pour rechercher des paquets Ethernet entre le serveur d&#8217;installation et le client. Recherchez également les entrées de plusieurs fichiers journaux effectués par <code>tftpd(8)</code> et <code>dhcpd(8)</code> :</p></div>
<div class="listingblock">
<div class="content">
<pre><code>faiserver$ egrep "tftpd|dhcpd" /var/log/*</code></pre>
</div></div>
</div>
</div>
<div class="sect2">
<h3 id="_a_id_pxeboot_a_détails_du_démarrage_pxe"><a id="pxeboot"></a>Détails du démarrage PXE</h3>
<div class="paragraph"><p>Ici, nous décrivons les détails du démarrage PXE, qui ne sont nécessaires que si vous avez des problèmes lors du démarrage de vos clients d&#8217;installation.</p></div>
<div class="paragraph"><p>Presque toutes les cartes réseau modernes prennent en charge l&#8217;environnement de démarrage PXE. PXE est l&#8217;environnement d&#8217;exécution de pré-lancement. Cela nécessite le chargeur de démarrage PXELINUX et une version spéciale du démonTFTP, disponible dans les paquets Debian <code>pxelinux</code> et <code>tftpd-hpa</code>. Le démarrage PXE nécessite également un serveur DHCP, afin que la carte réseau puisse configurer ses paramètres IP. Il s&#8217;agit de la séquence d&#8217;une amorce PXE:</p></div>
<div class="ulist"><ul>
<li>
<p>
La carte réseau du client envoie son adresse MAC
</p>
</li>
<li>
<p>
Le serveur DHCP répond à la configuration IP du client
</p>
</li>
<li>
<p>
La carte réseau configure son IP
</p>
</li>
<li>
<p>
Le client d&#8217;installation obtient le binaire pxelinux.0 via TFTP
</p>
</li>
<li>
<p>
Obtenez le fichier de configuration pxelinux.cfg/C0A8210C via TFTP
</p>
</li>
<li>
<p>
C0A8210C est l&#8217;adresse IP du client en hexadécimal
</p>
</li>
<li>
<p>
Cette configuration contient le noyau, initrd et les paramètres de ligne de commande supplémentaires du noyau, qui a été créé par fai-chboot.
</p>
</li>
<li>
<p>
Obtenez le noyau et initrd via TFTP.
</p>
</li>
</ul></div>
<div class="paragraph"><p>Exemple d&#8217;un fichier pxelinux.cfg:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>default fai-generated

label fai-generated
kernel vmlinuz-3.16.0-4-amd64
append initrd=initrd.img-3.16.0-4-amd64 ip=dhcp  root=/srv/fai/nfsroot aufs  FAI_FLAGS=verbose,sshd,createvt FAI_CONFIG_SRC=nfs://faiserver/srv/fai/config FAI_ACTION=install</code></pre>
</div></div>
<div class="paragraph"><p>Voir <em>/usr/share/doc/syslinux/pxelinux.doc</em> pour des informations plus détaillées sur PXELINUX. Il existe un nouveau binaire lpxelinux qui prend également en charge le chargement du noyau et de l&#8217;initrd via FTP ou HTTP. La commande <em>fai-chboot(8)</em>' prend en charge cette option avec l&#8217;option <em>-U</em>.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_customizing_your_install_server_setup_a_personnalisation_de_la_configuration_de_votre_serveur_d_8217_installation"><a id="Customizing your install server setup"></a>Personnalisation de la configuration de votre serveur d&#8217;installation</h3>
<div class="ulist"><ul>
<li>
<p>
Miroir de paquetage local/plus rapide
</p>
</li>
<li>
<p>
Loguser différent
</p>
</li>
<li>
<p>
Local root password dans nfsroot
</p>
</li>
</ul></div>
<div class="paragraph"><p>La configuration du paquet FAI (et non les données de configuration pour les clients d&#8217;installation) est définie dans <em>fai.conf(5)</em>. Les définitions qui sont utilisées uniquement pour créer le nfsroot sont situées dans <em>nfsroot.conf(5)</em>. Vérifiez ces variables importantes dans <em>nfsroot.conf</em> avant d&#8217;appeler <em>fai-setup</em> ou <em>fai-make-nfsroot</em>.</p></div>
<div class="dlist"><dl>
<dt class="hdlist1">
FAI_DEBOOTSTRAP
</dt>
<dd>
<p>
La construction de nfsroot utilise la commande <code>debootstrap(8)</code>. Il a besoin de l&#8217;emplacement d&#8217;un miroir Debian et du nom de la distribution (wheezy, jessie, stretch, sid) pour lequel le système Debian de base devrait être construit. N&#8217;utilisez pas de distributions différentes ici et dans <em>/etc/fai/apt/sources.list</em>. Cela créera un nfsroot brisé.
</p>
</dd>
<dt class="hdlist1">
NFSROOT_ETC_HOSTS
</dt>
<dd>
<p>
Cette variable n&#8217;est nécessaire que si les clients n&#8217;ont pas accès à un serveur DNS. Cette variable multiligne est ajoutée à /etc/hosts dans le nfsroot. Ensuite, les clients d&#8217;installation peuvent accéder à ces hôtes par leur nom sans utiliser DNS.
</p>
</dd>
</dl></div>
<div class="paragraph"><p>Le contenu de <em>/etc/fai/apt/sources.list</em> est utilisé par le serveur d&#8217;installation et par les clients. Si votre serveur d&#8217;installation a plusieurs cartes réseau et différents noms d&#8217;hôte pour chaque carte (comme pour un serveur Beowulf), utilisez le nom du serveur d&#8217;installation qui est connu des clients d&#8217;installation.</p></div>
<div class="paragraph"><p>Si vous avez des problèmes lors de l&#8217;exécution de <code>fai-setup</code>, ils proviennent habituellement de <code>fai-make-nfsroot(8)</code> qui est appelé par la commande précédente. L&#8217;ajout de <em>-v</em> vous donne une sortie plus détaillée qui vous aide à repérer l&#8217;erreur. La sortie est écrite dans <em>/var/log/fai/fai-make-nfsroot.log</em>. <span class="footnote"><br />[Pour le débogage, il peut être utile d&#8217;entrer l&#8217;environnement chroot manuellement à l&#8217;aide de cette commande. <em>faiserver# chroot /srv/fai/nfsroot bash</em>]<br /></span></p></div>
<div class="paragraph"><p>L&#8217;installation crée également le compte fai (défini par <code>$LOGUSER</code>) s&#8217;il n&#8217;est pas déjà disponible. Vous pouvez donc ajouter un utilisateur avant d&#8217;appeler <code>fai-setup(8)</code> à l&#8217;aide de la commande <code>adduser(8)</code> et utiliser ce compte local pour enregistrer des fichiers journaux. Les fichiers journaux de tous les clients d&#8217;installation sont enregistrés dans le répertoire de base de ce compte. Vous devriez changer le groupe principal de ce compte, donc ce compte a des droits d'écriture sur <em>/srv/tftp/fai</em> pour appeler fai-chboot pour créer la configuration PXE pour les hôtes.</p></div>
<div class="paragraph"><p>Lorsque vous apportez des modifications à <em>fai.conf</em>, <em>nfsroot.conf</em>, le nfsroot doit être reconstruit en appelant <code>fai-make-nfsroot(8)</code>. Si vous souhaitez uniquement installer un nouveau paquet kernel sur nfsroot, ajoutez les flags <em>-k</em> ou <em>-K</em> à <code>fai-make-nfsroot</code>. Cela ne recréera pas votre nfsroot, mais ne mettra à jour que vos noyaux et les modules du noyau dans le nfsroot ou ajoutera des paquets supplémentaires dans le nfsroot.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_cdboot_a_création_d_8217_un_cd_fai_ou_d_8217_une_clé_usb"><a id="cdboot"></a>Création d&#8217;un CD FAI ou d&#8217;une clé USB</h3>
<div class="paragraph"><p>Vous pouvez facilement créer un CD d&#8217;installation (ou clé USB) pour votre installation réseau. Cela permettra d&#8217;effectuer la même installation et la même configuration à partir du CD sans avoir besoin du serveur d&#8217;installation. Par conséquent, vous devez créer un miroir partiel de tous les paquets Debian nécessaires à vos classes FAI (à l&#8217;aide de <code>fai-mirror(1)</code>). Ensuite, la commande <code>fai-cd(8)</code> mettra ce miroir, le nfsroot et l&#8217;espace de configuration sur un CD amorçable. C&#8217;est tout!</p></div>
<div class="paragraph"><p>Ce CD d&#8217;installation contient toutes les données nécessaires à l&#8217;installation. La commande <code>fai-cd(8)</code> place le nfsroot, l&#8217;espace de configuration et un sous-ensemble du miroir Debian sur un CD-ROM. Un miroir de paquets partiel est créé à l&#8217;aide de la commande <code>fai-mirror(1)</code> qui contient tous les paquetages utilisés par les classes utilisées dans votre espace de configuration. Un échantillon d&#8217;image ISO est disponible à l&#8217;adresse <a href="http://fai-project.org/fai-cd">http://fai-project.org/fai-cd</a>.</p></div>
<div class="paragraph"><p>Avec la commande <code>dd(1)</code>, vous pouvez également créer une clé USB bootable en écrivant simplement le contenu du fichier ISO sur votre clé USB (ici le stick est <em>/dev/sdf</em>).</p></div>
<div class="listingblock">
<div class="content">
<pre><code> faiserver# dd if=fai-cd.iso of=/dev/sdf bs=1M</code></pre>
</div></div>
<div class="paragraph"><p>Il ne s&#8217;agit pas d&#8217;un live CD du serveur d&#8217;installation.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_diskimage_a_création_d_8217_images_de_disque_vm_à_l_8217_aide_de_fai"><a id="diskimage"></a>Création d&#8217;images de disque VM à l&#8217;aide de FAI</h3>
<div class="paragraph"><p>En utilisant la commande <code>fai-diskimage(8)</code>, vous pouvez créer des images de disques de machines Linux qui peuvent être utilisées avec une machine virtuelle comme KVM, VMware, VirtualBox ou un service cloud comme OpenStack, GCE, EC2 et autres. Le processus d&#8217;installation exécute les tâches FAI normales sur une image de disque brut. Après l&#8217;installation, vous pouvez démarrer l&#8217;image disque et avoir un système en cours d&#8217;exécution. L&#8217;image disque peut également être convertie au format qcow2.</p></div>
<div class="listingblock">
<div class="content">
<pre><code> faiserver# export FAI_BASEFILEURL=http://fai-project.org/download/basefiles/
 faiserver# fai-diskimage -u cloud3 -S 2G -cDEBIAN,JESSIE64,AMD64,FAIBASE,GRUB_PC,CLOUD,GCE disk.raw</code></pre>
</div></div>
<div class="paragraph"><p>Crée le fichier disk.raw pour un hôte appelé cloud3, avec un petit ensemble de progiciels.</p></div>
<div class="listingblock">
<div class="content">
<pre><code> # export FAI_BASEFILEURL=http://fai-project.org/download/basefiles/
 # cl=DEFAULT,DHCPC,DEBIAN,AMD64,FAIBASE,GRUB_PC,UBUNTU,XENIAL,XENIAL64,XORG
 # fai-diskimage -v -u foobar -S5G -c$cl ubuntu.qcow2</code></pre>
</div></div>
<div class="paragraph"><p>Crée une image de disque appelée ubuntu.qcow2 pour un bureau Ubuntu 16.04 avec un nom d&#8217;hôte défini sur foobar.</p></div>
<div class="paragraph"><p>Vous ne devez pas configurer le nfsroot lorsque vous utilisez uniquement fai-diskimage. Mais vous avez besoin d&#8217;un fichier de base dans votre espace de configuration. Vous pouvez télécharger une image de base Debian à partir de <a href="http://fai-project.org/download/basefile">http://fai-project.org/download/basefile</a> et copier ceci dans votre espace de configuration. Si vous avez déjà configuré le nfsroot, vous pouvez copier le fichier de base Debian depuis le nfsroot dans votre espace de configuration à l&#8217;aide de cette commande:</p></div>
<div class="listingblock">
<div class="content">
<pre><code> $ cp /srv/fai/nfsroot/var/tmp/base.tar.xz
 $ /srv/fai/config/basefiles/JESSIE64.tar.xz</code></pre>
</div></div>
</div>
<div class="sect2">
<h3 id="_a_id_sysinfo_a_système_de_sauvetage_fai"><a id="sysinfo"></a>Système de sauvetage FAI</h3>
<div class="paragraph"><p>Si vous définissez la variable <code>$FAI_ACTION</code> sur sysinfo (par exemple en utilisant <code>fai-chboot -S</code>), le client n&#8217;installera pas de nouveau système, mais collectera beaucoup d&#8217;informations système. Si vous définissez <code>$FAI_ACTION</code> sur <em>inventory</em>, vous ne recevrez que quelques informations sur le matériel. Les deux actions peuvent être utilisées pour FAI comme un système de sauvetage.</p></div>
<div class="paragraph"><p>Tapez <em>ctrl-c</em> pour obtenir un shell ou utilisez <em>Alt-F2</em> ou <em>Alt-F3</em> et vous obtiendrez un autre terminal de console, si vous avez ajouté <em>createvt</em> à <code>$FAI_FLAGS</code>.</p></div>
<div class="paragraph"><p>Vous avez maintenant un système Linux en cours d&#8217;exécution sur le client d&#8217;installation sans utiliser le disque dur local. Utilisez-le comme système de secours si votre disque local est endommagé ou si l&#8217;ordinateur ne peut pas démarrer correctement à partir du disque dur. Vous obtiendrez un shell et vous pouvez exécuter diverses commandes (<code>dmesg</code>, <code>lsmod</code>, <code>df</code>, <code>lspci</code>, &#8230;). Regardez le fichier journal dans <code>/tmp/fai</code>. Vous y trouverez de nombreuses informations sur le processus d&#8217;amorçage.</p></div>
<div class="paragraph"><p>FAI monte tous les systèmes de fichiers qu&#8217;il trouve sur les disques locaux en lecture seule. Il vous indique également sur quelle partition un fichier <em>/etc/fstab</em> existe. Lorsqu&#8217;une seule table de système de fichiers est trouvée, les partitions sont montées selon ces informations. Voici un exemple:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>demohost:~# df
Filesystem      1K-blocks      Used Available Use% Mounted on
rootfs            4099064    414088   3645296  11% /
192.168.33.250:/srv/fai/nfsroot
                  3905600    410976   3454944  11% /live/image
tmpfs              193464      3112    190352   2% /live/cow
aufs              4099064    414088   3645296  11% /

192.168.33.250:/srv/fai/config
                  3905600    410976   3454944  11% /var/lib/fai/config
/dev/sda1          241116     74519    154149  33% /target
/dev/sda9         4364212    139888   4179988   4% /target/home
/dev/sda7          553376     16840    536536   4% /target/tmp
/dev/sda8         2221628    275936   1832840  14% /target/usr
/dev/sda6          577096    172924    374856  32% /target/var</code></pre>
</div></div>
<div class="paragraph"><p><strong>Cette méthode peut être utilisée comme un environnement de secours!</strong> Si vous avez besoin d&#8217;un système de fichiers avec accès en lecture/écriture, utilisez la commande <code>rwmount</code>:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>demohost# rwmount /target/home</code></pre>
</div></div>
</div>
<div class="sect2">
<h3 id="_a_id_nonfs_a_fai_sans_nfs"><a id="nonfs"></a>FAI sans NFS</h3>
<div class="paragraph"><p>Pour démarrer dans FAI et commencer la séquence d&#8217;installation sans utiliser le protocole NFS. Vous démarrez la machine cliente en utilisant PXE comme d&#8217;habitude, puis récupérez une image contenant le nfsroot via http.</p></div>
<div class="paragraph"><p>Pour créer une image, utilisez l&#8217;argument -S de fai-cd</p></div>
<div class="listingblock">
<div class="content">
<pre><code>faiserver# fai-cd -S squash.img</code></pre>
</div></div>
<div class="paragraph"><p>Déplacez cette image vers un répertoire à partir duquel elle peut être demandée via http (généralement un répertoire desservi par le serveur web)</p></div>
<div class="paragraph"><p>Pour demander maintenant l&#8217;image squashfs, ajoutez ce qui suit à votre ligne de commande du noyau, p. Dans votre fichier de configuration pxelinux pour le client.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>root=live:http://faiserver/cskoeln/squash.img</code></pre>
</div></div>
<div class="paragraph"><p>Remplacez faiserver par le nom de domaine ou IP de la machine à laquelle votre image de squash est servie.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_otherdists_a_installation_d_8217_autres_distributions_à_l_8217_aide_d_8217_un_nfsroot_debian"><a id="otherdists"></a>Installation d&#8217;autres distributions à l&#8217;aide d&#8217;un nfsroot Debian</h3>
<div class="paragraph"><p>Vous pouvez installer toutes sortes de distributions Linux à partir d&#8217;un seul nfsroot Debian. Par conséquent, vous devez créer un fichier base.tar.xz de la distribution que vous souhaitez installer et le placer dans le répertoire <code>basefiles</code>. Puis nommez-le UBUNTU1404.tar.xz par exemple. Un client d&#8217;installation appartenant à la classe UBUNTU1404 extrait ensuite ce fichier de base dans son système de fichiers vide. De plus, vous devez ajuster les sources.list ou les fichiers de configuration similaires nécessaires pour spécifier l&#8217;emplacement du référentiel de paquets.</p></div>
<div class="paragraph"><p>L&#8217;outils <code>rinse(8)</code> est utilisé pour créer des fichiers de base pour la distribution comme CentOS, openSUSE, Scientific Linux Cern ou Fedora. Certains fichiers de base peuvent être téléchargés à partir de <a href="http://fai-project.org/download/basefiles/">http://fai-project.org/download/basefiles/</a>.</p></div>
<div class="paragraph"><p>Le script <code>mk-basefile</code> dans <em>/usr/share/doc/fai-doc/examples/simple/basefiles/</em>' aide à créer ces fichiers de base.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_dirinstall_a_création_d_8217_environnements_chrooter_et_virtualiser"><a id="dirinstall"></a>Création d&#8217;environnements chrooter et virtualiser</h3>
<div class="paragraph"><p>Si vous devez créer certains environnements chroot, ou un environnement de virtualisation où vous ne pouvez ni ne voulez exécuter un programme d&#8217;installation Debian normal pour accéder à un système opérationnel (par exemple, les domaines hôtes Xen), il ya l&#8217;action FAI <em>dirinstall</em>.
En appelant</p></div>
<div class="listingblock">
<div class="content">
<pre><code>faiserver# fai &lt;options&gt; dirinstall &lt;target-directory&gt;</code></pre>
</div></div>
<div class="paragraph"><p>Et en utilisant l&#8217;option <em>-c &lt;classes&gt;</em> ou <em>-N</em> vous obtenez une installation FAI, sans l&#8217;action de partitionnement, directement dans le répertoire cible. Le nom d&#8217;hôte de l&#8217;installation cible peut être spécifié à l&#8217;aide de <em>-u &lt;host-name&gt;</em></p></div>
<div class="paragraph"><p>Ceci, par exemple, peut être utilisé pour combiner FAI avec l&#8217;outil <em>xen-tools</em>, qui vous aide à construire des domaines invités Xen. <em>xen-tools</em> est très agréable pour générer des fichiers de configuration et bloquer des périphériques pour de nouveaux invités basés sur des commandes simples et/ou des fichiers de configuration, mais ils ne peuvent assigner qu&#8217;un seul rôle par installation pour la personnalisation. Les FAI-utilisateurs ont besoin et veulent plus, car ils sont utilisés pour avoir le système de classe. Ils les obtiennent même dans les installations xen-tools, en utilisant le code suivant en tant que rôle xen-tools script:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>#!/bin/sh
TARGET=$1
CMD="fai -N  -v -u ${hostname} dirinstall $TARGET"
echo running $CMD
$CMD</code></pre>
</div></div>
<div class="paragraph"><p>Ensuite, vous voulez définir la variable <em>install=0</em> de la configuration xen-tools pour cet hôte.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_softupdate_a_utilisation_de_fai_pour_les_mises_à_jour"><a id="softupdate"></a>Utilisation de FAI pour les mises à jour</h3>
<div class="paragraph"><p>FAI peut également effectuer des mises à jour de systèmes déjà en cours d&#8217;exécution, sans réinstallation à partir de zéro. C&#8217;est ce qu&#8217;on appelle softupdate. Un FAI softupdate ignore les tâches qui ne sont pas adaptées à la mise à jour d&#8217;un système en cours d&#8217;exécution, comme le partitionnement des disques durs et la création de systèmes de fichiers. Au lieu de cela, il exécute uniquement les tâches de mise à jour et d&#8217;installation des progiciels et de l&#8217;appel des scripts de personnalisation.</p></div>
<div class="paragraph"><p>Pour exécuter un appel softupdate:</p></div>
<div class="listingblock">
<div class="content">
<pre><code># fai -v -s nfs://faiserver/srv/fai/config softupdate</code></pre>
</div></div>
<div class="paragraph"><p>Par défaut, un softupdate utilise la liste des classes définies lors de l&#8217;installation initiale. Assurez-vous de définir la variable <code>$LOGSERVER</code> (effectuée dans un fichier <em>class/*.var</em>) si FAI doit enregistrer les fichiers journaux sur une machine distante.</p></div>
<div class="paragraph"><p>C&#8217;est à vous, comment démarrer un softupdate sur un plus grand nombre d&#8217;hôtes. Vous pouvez faire le softupdate sur une base régulière via cron ou vous pouvez utiliser des outils comme <code>clusterssh(1)</code> pour démarrer un softupdate via un push sur une liste d&#8217;hôtes.</p></div>
<div class="paragraph"><p>Gardez à l&#8217;esprit que les scripts de personnalisation sont exécutés chaque fois que vous faites un softupdate. Cela signifie qu&#8217;ils doivent être <strong>idempotents</strong>, c&#8217;est-à-dire que le résultat de leur fonctionnement doit toujours produire le même résultat, même lorsqu&#8217;ils fonctionnent plus d&#8217;une fois.</p></div>
<div class="paragraph"><p>Par exemple, l&#8217;ajout d&#8217;une ligne à un fichier ne doit pas se faire via ce code:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>$ echo "some strings" &gt;&gt; /etc/fstab</code></pre>
</div></div>
<div class="paragraph"><p>Utilisez plutôt la commande <code>ainsl(1)</code> dans un script shell ou utilisez la fonction <em>AppendIfNoSuchLine</em> de cfengine.</p></div>
<div class="paragraph"><p>Toutes les commandes du script de personnalisation doivent être capables de modifier le système de fichiers cible s&#8217;il est disponible dans <em>/target</em> lors de l&#8217;installation initiale ou si c&#8217;est le système de fichiers normal relatif à <em>/</em> pendant le softtupdate.</p></div>
<div class="paragraph"><p>Voici quelques variables qui aident à écrire ces scripts:</p></div>
<div class="dlist"><dl>
<dt class="hdlist1">
<code>$target</code>
</dt>
<dd>
<p>
Pointe vers le répertoire racine du client, qui est <em>/target</em> pendant l&#8217;installation et <em>/</em> pendant un softupdate.
</p>
</dd>
<dt class="hdlist1">
<code>$FAI_ROOT</code>
</dt>
<dd>
<p>
C&#8217;est la même valeur que <code>$target</code>. Pour des raisons historiques, nous avons ces deux variables dans FAI.
</p>
</dd>
<dt class="hdlist1">
<code>$ROOTCMD</code>
</dt>
<dd>
<p>
Dans le cas de l&#8217;installation, il s&#8217;agit d&#8217;un alias pour <em>chroot $target</em> en cas de softupdate c&#8217;est juste vide. Vous pouvez ajouter ceci aux commandes si vous avez besoin d&#8217;exécuter une commande dans le système de fichiers cible des clients via chroot.
</p>
</dd>
<dt class="hdlist1">
<code>$FAI_ACTION</code>
</dt>
<dd>
<p>
Si vous devez appeler le code en fonction de l&#8217;action FAI effectuée, vous pouvez utiliser cette variable. Il contient l&#8217;action actuellement exécutée: <em>install</em>, <em>softupdate</em>, <em>dirinstall</em>, <em>sysinfo</em>, <em>inventory</em> ou votre propre action définie.
</p>
</dd>
</dl></div>
</div>
<div class="sect2">
<h3 id="_a_id_archcross_a_comment_installer_un_système_d_8217_exploitation_32_bits_à_partir_d_8217_un_système_d_8217_exploitation_64_bits"><a id="archcross"></a>Comment installer un système d&#8217;exploitation 32 bits à partir d&#8217;un système d&#8217;exploitation 64 bits</h3>
<div class="paragraph"><p>Pour installer un ordinateur avec un système d&#8217;exploitation 32 bits, vous avez besoin d&#8217;un nfsroot i386. La création de cette nfsroot 32 bits sur un serveur d&#8217;installation exécutant amd64 est assez simple. Installez et configurez les paquets FAI. Copiez ensuite vos fichiers de configuration FAI dans un nouveau sous-répertoire.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>faiserver# cp -a /etc/fai /etc/fai-i386</code></pre>
</div></div>
<div class="paragraph"><p>Modifiez la variable <code>$FAI_DEBOOTSTRAP_OPTS</code> dans <em>/etc/fai-i386/nfsroot.conf</em> et ajoutez l&#8217;option <code>--arch i386</code>. Choisissez également un répertoire différent pour votre nouveau nfsroot. Voici les deux lignes après l'édition.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>NFSROOT=/srv/fai/nfsroot-i386
FAI_DEBOOTSTRAP_OPTS="--arch i386 --exclude=info --include=aptitude""</code></pre>
</div></div>
<div class="paragraph"><p>Appelez maintenant fai-make-nfsroot qui crée le nfsroot 32 bits dans <em>/srv/fai/nfsroot-i386</em></p></div>
<div class="listingblock">
<div class="content">
<pre><code>faiserver# fai-make-nfsroot -v -C/etc/fai-i386</code></pre>
</div></div>
<div class="paragraph"><p>La création d&#8217;un miroir partiel utilisant <code>fai-mirror(1)</code> nécessaire à un CD amorçable ou une clé USB est également possible sur une architecture différente. Vous devez spécifier l&#8217;architecture lors de l&#8217;appel de fai-mirror.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>$ fai-mirror -m800 -B -a i386 -v -cDEFAULT,DEBIAN,FAIBASE,I386 /srv/mirror-i386</code></pre>
</div></div>
<div class="paragraph"><p>C&#8217;est tout!</p></div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_a_id_hints_a_divers_conseils_et_détails"><a id="hints"></a>Divers conseils et détails</h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_a_id_tasks_a_la_liste_des_tâches"><a id="tasks"></a>La liste des tâches</h3>
<div class="paragraph"><p>La plupart des tâches de l&#8217;installation sont définies comme des sous-routines qui sont définies dans <em>/usr/lib/fai/subroutines</em> (par exemple <code>task_instsoft</code>). Certains sont des scripts shell externes situés dans <em>/usr/lib/fai/</em>. Ils sont appelés via un sous-programme supérieur appelé <em>task</em>. Ce sous-programme appelle les hooks si disponibles, puis appelle la tâche (définie comme <em>task</em>&lt;name&gt;_). Une tâche et ses hooks peuvent être ignorés à la demande en utilisant la commande <em>skiptask()</em>.</p></div>
<div class="paragraph"><p>Suit maintenant la description de toutes les tâches, énumérées dans l&#8217;ordre dans lequel elles sont exécutées.</p></div>
<div class="dlist"><dl>
<dt class="hdlist1">
confdir
</dt>
<dd>
<p>
Les paramètres ajoutés au noyau peuvent définir des variables, le démon syslog est démarré. La liste des périphériques réseau est stockée dans <code>$netdevices</code>. Ensuite, des paramètres supplémentaires sont extraits d&#8217;un serveur DHCP. Le fichier de configuration du résolveur DNS est créé.
</p>
<div class="paragraph"><p>L&#8217;emplacement de l&#8217;espace de configuration est défini par la variable <code>$FAI_CONFIG_SRC</code>.</p></div>
<div class="paragraph"><p>Ensuite, le fichier <em>$FAI/hooks/subroutines</em> est sourcé s&#8217;il existe. En utilisant ce fichier, vous pouvez définir vos propres sous-programmes ou remplacer la définition des sous-programmes FAI.</p></div>
</dd>
<dt class="hdlist1">
setup
</dt>
<dd>
<p>
Cette tâche définit l&#8217;heure du système, tous les <code>$FAI_FLAGS</code> sont définis et deux terminaux virtuels supplémentaires sont ouverts à la demande. Un démon de shell sécurisé est lancé à la demande pour les connexions à distance.
</p>
</dd>
<dt class="hdlist1">
defclass
</dt>
<dd>
<p>
Appellez <code>fai-class(1)</code> pour définir des classes à l&#8217;aide de scripts et de fichiers dans <em>$FAI/class</em> et classes de <em>/tmp/fai/additional-classes</em> et la variable <code>$ADDCLASSES</code>. La liste de toutes les classes définies est stockée dans la variable <code>$classes</code> et enregistrée dans <em>/tmp/fai/FAI_CLASSES</em>.
</p>
</dd>
<dt class="hdlist1">
defvar
</dt>
<dd>
<p>
Sourcez tous les fichiers <em>$FAI/class/*.var</em> pour chaque classe définie. Si un hook a écrit quelques définitions de variables dans le fichier <em>$LOGDIR/additional.var</em>, ce fichier est également sourcé.
</p>
</dd>
<dt class="hdlist1">
action
</dt>
<dd>
<p>
En fonction de la valeur de <code>$FAI_ACTION</code>, ce sous-programme décide de l&#8217;action FAI à exécuter. Les actions disponibles par défaut sont: <em>sysinfo</em>, <em>install</em>, <em>inventory</em>, <em>dirinstall</em> et <em>softupdate</em>. Si <code>$FAI_ACTION</code> a une autre valeur, une action définie par l&#8217;utilisateur est appelée si un fichier <em>$FAI/hooks/$FAI_ACTION</em> existe. Ainsi, vous pouvez facilement définir vos propres actions.
</p>
</dd>
<dt class="hdlist1">
sysinfo
</dt>
<dd>
<p>
Appelée lorsque aucune installation n&#8217;est effectuée mais que l&#8217;action est <em>sysinfo</em>. Il affiche des informations sur le matériel détecté et monte les disques durs locaux en lecture uniquement sur <em>/target/<code>partitionname</code></em> ou en regard d&#8217;un fichier <em>fstab</em> trouvé à l&#8217;intérieur d&#8217;une partition. Les fichiers journaux sont stockés sur le serveur d&#8217;installation.
</p>
</dd>
<dt class="hdlist1">
inventory
</dt>
<dd>
<p>
Une courte liste des informations système est imprimée.
</p>
</dd>
<dt class="hdlist1">
install
</dt>
<dd>
<p>
Cette tâche contrôle la séquence d&#8217;installation. Vous entendrez trois bips avant le début de l&#8217;installation. Le travail principal consiste à appeler d&#8217;autres tâches et à enregistrer la sortie dans <em>/tmp/fai/fai.log</em>. Si vous avez des problèmes pendant l&#8217;installation, regardez tous les fichiers dans <em>/tmp/fai/</em>. Vous trouverez des exemples de fichiers journaux à l&#8217;adresse <a href="http://fai-project.org/logs/">http://fai-project.org/logs/</a>.
</p>
</dd>
<dt class="hdlist1">
dirinstall
</dt>
<dd>
<p>
Installez dans un répertoire, et non pas sur un disque local. Utilisez-le pour créer des environnements chrootés.
</p>
</dd>
<dt class="hdlist1">
softupdate
</dt>
<dd>
<p>
Cette tâche, exécutée à l&#8217;intérieur d&#8217;un système en cours d&#8217;exécution via l&#8217;interface de ligne de commande <code>fai(8)</code>, effectue un softupdate. Voir le chapitre <a href="#softupdate">[softupdate]</a> pour plus de détails.
</p>
</dd>
<dt class="hdlist1">
partition
</dt>
<dd>
<p>
Appelle <code>setup-storage(8)</code> pour partitionner les disques durs et créer des systèmes de fichiers. La tâche écrit des définitions de variables pour la partition et le périphérique racine et de démarrage (<code>$ROOT_PARTITION, $BOOT_PARTITION, $BOOT_DEVICE</code>) dans <em>/tmp/fai/disk_var.sh</em> et crée un fichier <em>fstab</em> pour le nouveau système.
</p>
</dd>
<dt class="hdlist1">
mountdisks
</dt>
<dd>
<p>
Montez les partitions créées en fonction du fichier <em>/tmp/fai/fstab</em> créé par rapport à <code>$FAI_ROOT</code>.
</p>
</dd>
<dt class="hdlist1">
extrbase
</dt>
<dd>
<p>
Extrait un système minimal après lequel un chroot peut y être introduit. Par défaut, le fichier tar base <em>/var/tmp/base.tar.xz</em> sera extrait. Les fichiers correspondant à un nom de classe dans <em>$FAI/basefiles/</em> sont également utilisés pour décompresser un autre fichier tar selon les classes définies. Cela peut être utilisé pour installer des distributions Linux différentes de celles utilisées pour créer le nfsroot. Le fichier par défaut <em>base.tar.xz</em> est un instantané d&#8217;un système Debian de base créé par <code>debootstrap(8)</code> Cette tâche utilise la variable <code>FAI_BASEFILEURL</code> pour extraire le fichier de base via FTP ou HTTP si elle est définie.
</p>
</dd>
<dt class="hdlist1">
debconf
</dt>
<dd>
<p>
Appelle <code>fai-debconf(1)</code> pour définir les valeurs de la base de données de préconfiguration de debconf.
</p>
</dd>
<dt class="hdlist1">
repository
</dt>
<dd>
<p>
Préparez l&#8217;accès au référentiel de paquets en préparant la configuration apt. Cela peut également ajouter des clés de référentiel via <code>apt-key(8)</code> en classe à partir de fichiers comme <em>CLASSNAME.asc</em> dans le répertoire <em>package_config</em>.
</p>
</dd>
<dt class="hdlist1">
updatebase
</dt>
<dd>
<p>
Met à jour les paquets de base du nouveau système et met à jour la liste des paquets disponibles. Il falsifie également certaines commandes (appelées diversions) à l&#8217;intérieur du nouveau système installé à l&#8217;aide de <code>dpkg-divert(8)</code>, de sorte qu&#8217;aucun démon ne sera démarré pendant l&#8217;installation.
</p>
</dd>
<dt class="hdlist1">
instsoft
</dt>
<dd>
<p>
Installe les progiciels souhaités en utilisant des fichiers de classe dans <em>$FAI/package_config/</em>.
</p>
</dd>
<dt class="hdlist1">
configure
</dt>
<dd>
<p>
Appelle les scripts dans <em>$FAI/scripts/</em> et ses sous-répertoires pour chaque classe définie.
</p>
</dd>
<dt class="hdlist1">
tests
</dt>
<dd>
<p>
Appelle les scripts de test dans <em>$FAI/tests/</em> et ses sous-répertoires pour chaque classe définie.
</p>
</dd>
<dt class="hdlist1">
finish
</dt>
<dd>
<p>
Démonte tous les systèmes de fichiers dans le nouveau système installé et supprime les diversions de fichiers à l&#8217;aide de la commande <code>fai-divert</code>.
</p>
</dd>
<dt class="hdlist1">
chboot
</dt>
<dd>
<p>
Modifie la configuration PXE d&#8217;un hôte sur le serveur d&#8217;installation qui indique quelle configuration PXELINUX doit être chargée lors de la prochaine initialisation à partir de la carte réseau via TFTP. Par conséquent, la commande <code>fai-chboot(8)</code> est exécutée à distance sur le serveur d&#8217;installation.
</p>
</dd>
<dt class="hdlist1">
savelog
</dt>
<dd>
<p>
Enregistre les fichiers journaux sur le disque local et sur le compte <code>$LOGUSER</code> sur <code>$LOGSERVER</code> (par défaut sur le serveur d&#8217;installation).
</p>
</dd>
<dt class="hdlist1">
faiend
</dt>
<dd>
<p>
Attendez que les travaux en arrière-plan se terminent (par exemple, emacs compile des fichiers lisp) et redémarre automatiquement les clients d&#8217;installation ou attend la saisie manuelle avant le redémarrage.
</p>
</dd>
</dl></div>
</div>
<div class="sect2">
<h3 id="_a_id_itests_a_tests_automatisés"><a id="itests"></a>Tests automatisés</h3>
<div class="paragraph"><p>Après l&#8217;exécution des scripts de personnalisation, FAI exécutera certains tests si disponibles. En utilisant ces tests, vous pouvez vérifier les erreurs de l&#8217;installation. Les scripts de test sont appelés via <code>fai-do-scripts(1)</code> et doivent ajouter leurs messages à <em>$LOGDIR/test.log</em>. Un module Perl comprenant des sous-routines utiles peut être trouvé dans <em>Faitest.pm</em>. Un test peut également définir une nouvelle classe pour exécuter d&#8217;autres tests lors du prochain démarrage via la variable <code>$ADDCLASSES</code>.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_autodiscover_a_découvrir_automatiquement"><a id="autodiscover"></a> Découvrir automatiquement</h3>
<div class="paragraph"><p>Dans FAI 5.0, nous avons publié une fonctionnalité qui permet aux clients de rechercher le faiserver dans leur sous-réseau respectif. Cela soulève la nécessité de récupérer l&#8217;adresse MAC de chaque client et de configurer le démon DHCP.</p></div>
<div class="paragraph"><p>Cela se fait en démarrant à partir d&#8217;une petite autodiscover FAI bootmedium (CD, USB, etc.), qui peut être créée via la commande:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>faiserver# fai-cd -A autodiscover.iso</code></pre>
</div></div>
<div class="paragraph"><p>L&#8217;image a une taille d&#8217;environ 25 Mo et analyse le sous-réseau d&#8217;un serveur FAI. Par défaut, il affiche un menu avec tous les profils disponibles dans l&#8217;espace de configuration de la même manière que le drapeau de menu. Dans ce menu, vous pouvez sélectionner le type d&#8217;installation que vous souhaitez effectuer.</p></div>
<div class="paragraph"><p>Pour que les clients puissent trouver le faiserver, le faiserver doit exécuter fai-monitor.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_changeboot_a_modification_du_périphérique_d_8217_amorçage"><a id="changeboot"></a>Modification du périphérique d&#8217;amorçage</h3>
<div class="paragraph"><p>La modification de la séquence d&#8217;amorçage s&#8217;effectue normalement dans la configuration du BIOS. Mais vous ne pouvez pas changer le BIOS d&#8217;un système Linux en cours d&#8217;exécution.</p></div>
<div class="paragraph"><p>Ainsi, la séquence d&#8217;amorçage du BIOS restera inchangée et votre ordinateur devrait toujours démarrer en premier à partir de sa carte réseau et le deuxième périphérique d&#8217;amorçage devrait être le disque local. Ensuite, vous pouvez changer le périphérique d&#8217;amorçage du client en créant différentes configurations PXELINUX. Cela définira si une installation doit être effectuée, ou si le client doit démarrer à partir du disque local. Cela se fait à l&#8217;aide de <code>fai-chboot(8)</code>.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_debian_mirror_a_comment_créer_un_miroir_debian_local"><a id="debian-mirror"></a>Comment créer un miroir Debian local</h3>
<div class="paragraph"><p>Le script <code>mkdebmirror</code> <span class="footnote"><br />[Vous pouvez trouver le script dans <em>/usr/share/doc/fai-doc/examples/utils/</em> Version 5.3]<br /></span> peut être utilisé pour créer votre propre miroir Debian local. Ce script utilise la commande <code>debmirror(1)</code>. Un miroir Debian partiel pour l&#8217;architecture i386 et amd64 pour Debian 8.0 (aka jessie) sans les paquets source nécessite environ 56Go d&#8217;espace disque. L&#8217;accès au miroir via HTTP sera la méthode par défaut dans la plupart des cas. Pour afficher plus de résultats à partir du script, appelez <code>mkdebmirror -v</code>. Un compte root n&#8217;est pas nécessaire pour créer et maintenir le miroir Debian.</p></div>
<div class="paragraph"><p>Pour utiliser l&#8217;accès HTTP au miroir Debian local, installez un serveur Web et créez un lien symbolique vers le répertoire local où se trouve votre miroir:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>faiserver# apt-get install apache2
faiserver# ln -s /files/scratch/debmirror /var/www/html/debmirror</code></pre>
</div></div>
<div class="paragraph"><p>Créez un fichier <code>sources.list(5)</code> dans <em>/etc/fai/apt</em> qui donne accès à votre miroir Debian. Ajoutez également l&#8217;adresse IP du serveur HTTP à la variable <code>$NFSROOT_ETC_HOSTS</code> dans <em>nfsroot.conf</em> si les clients d&#8217;installation n&#8217;ont pas de résolution DNS.</p></div>
</div>
<div class="sect2">
<h3 id="_petits_conseils">Petits conseils</h3>
<div class="ulist"><ul>
<li>
<p>
Lorsque vous utilisez l&#8217;accès HTTP à un miroir Debian, la partition locale <em>/var</em> sur tous les clients d&#8217;installation doit être suffisamment grande pour conserver les paquets Debian téléchargés. N&#8217;essayez pas avec moins de 250 Moctets à moins que vous sachiez pourquoi. Vous pouvez limiter le nombre de paquets installés à la fois avec la variable <code>$MAXPACKAGES</code>.
</p>
</li>
<li>
<p>
Vous pouvez supprimer le logo rouge sur le client d&#8217;installation en appelant simplement une fois <code>reset</code>. Il ne s&#8217;affichera pas si vous créez un fichier à l&#8217;aide de cette commande sur le serveur d&#8217;installation:
</p>
</li>
</ul></div>
<div class="listingblock">
<div class="content">
<pre><code>touch /srv/fai/nfsroot/.nocolorlogo</code></pre>
</div></div>
<div class="ulist"><ul>
<li>
<p>
Une liste des variables utilisées par FAI peut être trouvée à <a href="http://wiki.fai-project.org/wiki/Variables">http://wiki.fai-project.org/wiki/Variables</a>.
</p>
</li>
<li>
<p>
Vous pouvez raccourcir certains scripts de personnalisation en utilisant une seule commande fcopy <em>fcopy -r /</em>.
</p>
</li>
<li>
<p>
Si vous reconstruisez le nfsroot, vous allez créer une nouvelle clé hôte ssh dans le nfsroot. La connexion à un client d&#8217;installation peut échouer, car la clé hôte change. Vous pouvez utiliser ceci:
</p>
</li>
</ul></div>
<div class="listingblock">
<div class="content">
<pre><code>$ ssh -o StrictHostKeyChecking=no root@installclient</code></pre>
</div></div>
<div class="ulist"><ul>
<li>
<p>
Vous pouvez également supprimer l&#8217;entrée hôte de votre client d&#8217;installation dans votre fichier <em>~/.ssh/known_hosts</em> à l&#8217;aide de la commande <em>ssh-keygen -R</em>.
</p>
</li>
<li>
<p>
Dans les tâches chboot et savelog, une connexion utilisant un shell sécurisé est ouverte au serveur FAI (voir <a href="#isavelog">[isavelog]</a>). Pour garantir que cela fonctionne de manière non interactive, une entrée appropriée dans <em>NFSROOT/root/.ssh/known_hosts</em> doit être créée. Lors de l&#8217;utilisation de fai-setup, cela se fait automatiquement, mais il peut s&#8217;avérer nécessaire de l'éditer manuellement si le nom de votre serveur FAI n&#8217;a pas été correctement déterminé. Si vous trébuchez sur des connexions ssh qui nécessitent de taper "yes" pour accepter la clé hôte pendant l&#8217;installation, vérifiez le contenu de votre fichier <em>NFSROOT/root/.ssh/known_hosts</em>
</p>
</li>
<li>
<p>
Une liste de tous les disques durs locaux est stockée dans <code>$disklist</code>. Il est défini après l&#8217;appel de <code>set_disk_info</code>.
</p>
</li>
<li>
<p>
Utilisez <code>fai-divert -a</code> si un script postinst appelle un programme de configuration, par exemple Le script postinst pour package apache appelle apacheconfig, qui nécessite une entrée manuelle. Vous pouvez fausser le programme de configuration pour que l&#8217;installation puisse être entièrement automatique.
</p>
</li>
<li>
<p>
Parfois, l&#8217;installation semble s&#8217;arrêter, mais souvent il ya seulement un script postinstall d&#8217;un logiciel qui nécessite une entrée manuelle de la console. Passez à un autre terminal virtuel et regardez quel processus fonctionne avec des outils comme <code>top(1)</code> et <code>pstree(1)</code>. Vous pouvez ajouter <em>debug</em> à <em>FAI_FLAGS</em> pour faire en sorte que le processus d&#8217;installation affiche toutes les sorties des scripts postinst sur la console et obtenir son entrée aussi à partir de la console.
</p>
</li>
<li>
<p>
Comment puis-je définir des classes sur la ligne de commande du noyau?
</p>
<div class="paragraph"><p>Lisez la page de manuel de <code>fai-class(8)</code>. Si vous souhaitez définir des classes supplémentaires (par exemple A, B, C) sur la ligne de commande du noyau, ajoutez ceci: <em>ADDCLASSES=A,B,C</em></p></div>
</li>
<li>
<p>
Comment utiliser un noyau personnalisé dans le nfsroot?
</p>
<div class="paragraph"><p>Construisez votre noyau personnalisé en construisant un paquet kernel à l&#8217;aide de <code>make-kpkg(8)</code> et utilisez l&#8217;option <code>--initrd</code>. Copiez ce paquet Debian dans un référentiel local et ajoutez-le à /etc/fai/sources.list. Ajoutez le nom de votre package à /etc/fai/NFSROOT. Ensuite appeler</p></div>
<div class="listingblock">
<div class="content">
<pre><code># fai-make-nfsroot -k</code></pre>
</div></div>
</li>
<li>
<p>
Puis-je utiliser un noyau 4.X?
</p>
<div class="paragraph"><p>Oui. L&#8217;utilisation de FAI 5.1 et dracut 044+150-1 overlayfs (au lieu d&#8217;aufs) est prise en charge, de même que le noyau 4.x. Lorsque vous utilisez Debian jessie, vous pouvez utiliser un noyau de backports ou consulter <a href="https://lists.uni-koeln.de/pipermail/linux-fai/2016-March/011283.html">https://lists.uni-koeln.de/pipermail/linux-fai/2016-March/011283.html</a></p></div>
</li>
<li>
<p>
Comment utiliser le nfsroot comme système pour les clients sans disque?
</p>
<div class="paragraph"><p><a href="http://wiki.fai-project.org/wiki/Use_nfsroot_for_diskless_clients">http://wiki.fai-project.org/wiki/Use_nfsroot_for_diskless_clients</a></p></div>
</li>
<li>
<p>
Comment faire pour servir plusieurs arborescence nfsroot sur un serveur FAI?
</p>
<div class="paragraph"><p>Si vous souhaitez diffuser plusieurs répertoires nfsroot, vous devez créer des répertoires de configuration spécifiques dans <em>/etc</em> pour FAI, comme <em>/etc/fai-jessie</em> et <em>/etc/fai-stretch</em>. Ensuite, vous devez définir les variables <code>$NFSROOT</code> dans différents répertoires et exécuter</p></div>
</li>
</ul></div>
<div class="listingblock">
<div class="content">
<pre><code>faiserver#fai-make-nfsroot -c /etc/fai-jessie</code></pre>
</div></div>
</div>
<div class="sect2">
<h3 id="_flag_reboot_fai_flags">flag_reboot (FAI_FLAGS)</h3>
<div class="paragraph"><p>Si flag_reboot est défini, en ajoutant "reboot" à <code>$FAI_FLAGS</code>, votre ordinateur client redémarrera après la fin de la tâche. Ceci est vrai pour les installations de réseau ainsi que pour les installations de bootmedium.</p></div>
</div>
<div class="sect2">
<h3 id="_centos_reboot">CentOS reboot</h3>
<div class="paragraph"><p>Après l&#8217;installation, CentOS nécessite habituellement un redémarrage supplémentaire, en raison des correctifs de sécurité SELinux qui sont appliqués après l&#8217;installation.</p></div>
</div>
<div class="sect2">
<h3 id="_a_id_logfiles_a_fichiers_journaux"><a id="logfiles"></a>Fichiers journaux</h3>
<div class="paragraph"><p>FAI crée plusieurs fichiers journaux. Pendant l&#8217;installation, ils sont stockés dans <em>/tmp/fai</em> sur le client d&#8217;installation lui-même. A la fin de l&#8217;installation, ils seront copiés sur le serveur d&#8217;installation (voir <a href="#isavelog">[isavelog]</a>). Une fois le client d&#8217;installation redémarré dans son système nouvellement installé, vous pouvez trouver les journaux FAI dans <em>/var/log/fai</em>. Les fichiers journaux sont également créés lors de l&#8217;action softupdate ou dirinstall.</p></div>
<div class="paragraph"><p>Sur le faiserver, vous pouvez trouver les fichiers journaux (distants) sous le répertoire ~fai.</p></div>
<div class="paragraph"><p>Les exemples de fichiers journaux des ordinateurs installés avec succès sont disponibles sur <a href="http://fai-project.org/logs">http://fai-project.org/logs</a>. Ce sont quelques fichiers journaux qui sont créés par FAI.</p></div>
<div class="dlist"><dl>
<dt class="hdlist1">
FAI_CLASSES
</dt>
<dd>
<p>
Contient une liste de toutes les classes définies.
</p>
</dd>
<dt class="hdlist1">
dmesg.log
</dt>
<dd>
<p>
La sortie de la commande <code>dmesg</code>. Contient des messages utiles de la mémoire tampon du noyau.
</p>
</dd>
<dt class="hdlist1">
fai.log
</dt>
<dd>
<p>
Le fichier journal principal. Contient toutes les informations importantes. Vous devez <strong>toujours</strong> lire ce fichier.
</p>
</dd>
<dt class="hdlist1">
boot.log
</dt>
<dd>
<p>
Une liste de variables de paramètres de réseau, principalement définis par le démon DHCP.
</p>
</dd>
<dt class="hdlist1">
format.log
</dt>
<dd>
<p>
Sortie de l&#8217;outil de partition <code>setup-storage(8)</code>.
</p>
</dd>
<dt class="hdlist1">
shell.log
</dt>
<dd>
<p>
La sortie de tous les scripts shell, utilisés pour la personnalisation.
</p>
</dd>
<dt class="hdlist1">
variables.log
</dt>
<dd>
<p>
Une liste de toutes les variables shell qui sont disponibles au cours d&#8217;une installation.
</p>
</dd>
<dt class="hdlist1">
error.log
</dt>
<dd>
<p>
Résumé des erreurs possibles dans tous les fichiers journaux.
</p>
</dd>
<dt class="hdlist1">
disk_var.sh
</dt>
<dd>
<p>
Une liste des variables contenant des informations sur les périphériques et les partitions à partir desquelles la partition racine et une liste de périphériques de swap. Ces informations sont utilisées par certains scripts de personnalisation (par exemple <em>GRUB_PC/10-setup</em>).
</p>
</dd>
</dl></div>
<div class="paragraph"><p>Si le processus d&#8217;installation se termine, le hook <em>savelog.LAST.sh</em> recherche tous les fichiers journaux pour les erreurs courantes et les écrit dans le fichier <em>error.log</em>. Donc, vous devriez d&#8217;abord regarder dans ce fichier pour les erreurs. Le fichier <em>status.log</em> vous donne également le code de sortie de la dernière commande exécutée dans un script. Pour être sûr, vous devriez rechercher plus de détails dans tous les fichiers journaux.</p></div>
</div>
<div class="sect2">
<h3 id="_comment_utiliser_http_pour_le_démarrage_pxe">Comment utiliser HTTP pour le démarrage PXE</h3>
<div class="listingblock">
<div class="content">
<pre><code>cp /usr/lib/PXELINUX/lpxelinux.0 /srv/tftp/fai/pxelinux.0</code></pre>
</div></div>
<div class="paragraph"><p>Activer l&#8217;accès HTTP au répertoire tftp:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>cd /var/www/html
ln -s /srv/tftp/fai</code></pre>
</div></div>
<div class="paragraph"><p>Ajoutez <em>-U URL</em> à l&#8217;appel <em>fai-chboot</em>. Par exemple:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>fai-chboot -U http://faiserver/fai -IFv .......</code></pre>
</div></div>
</div>
</div>
</div>
<div class="sect1">
<h2 id="_a_id_troubleshoot_a_dépannage"><a id="troubleshoot"></a>Dépannage</h2>
<div class="sectionbody">
<div class="sect2">
<h3 id="_a_id_booterror_a_erreurs_d_8217_amorçage"><a id="booterror"></a>Erreurs d&#8217;amorçage</h3>
<div class="paragraph"><p>Le message d&#8217;erreur suivant indique que votre client d&#8217;installation n&#8217;obtient pas de réponse d&#8217;un serveur DHCP. Vérifiez vos câbles ou démarrez le démon <code>dhcpd(8)</code> avec le debug flag activé.</p></div>
<div class="quoteblock">
<div class="content">
<div class="paragraph"><p>PXE-E51: No DHCP or BOOTP offers received
Network boot aborted</p></div>
</div>
<div class="attribution">
</div></div>
<div class="paragraph"><p>Si vous ne voyez pas le message suivant, le noyau d&#8217;installation n&#8217;a pas pu détecter votre carte réseau, par exemple en raison d&#8217;un pilote manquant:</p></div>
<div class="listingblock">
<div class="content">
<pre><code>Starting dhcp for interface eth0
dhcp: PREINIT eth0 up
dhcp: BOND setting eth</code></pre>
</div></div>
<div class="paragraph"><p>Vérifiez l&#8217;initrd dans le nfsroot (<code>lsinird</code>) si le pilote du noyau de votre carte réseau est inclus et vérifiez si vous souhaitez ajouter le paquet <em>firmware-linux-nonfree</em> dans <code>/etc/fai/NFSROOT</code> et reconstruisez l&#8217;initrd en appelant <code>fai-make-nfsroot -k</code>. Vous pouvez également ajouter un pilote à <code>/srv/fai/nfsroot/etc/dracut.conf</code> dans la ligne <code>add_drivers</code>+<code>=</code>.</p></div>
<div class="paragraph"><p>C&#8217;est le message d&#8217;erreur que vous verrez, lorsque votre carte réseau fonctionne, mais le serveur d&#8217;installation n&#8217;exporte pas le répertoire nfsroot vers les clients d&#8217;installation. Cela est souvent dû aux permissions NFS manquantes du côté serveur.</p></div>
<div class="listingblock">
<div class="content">
<pre><code>Starting dhcp for interface eth0
dhcp: PREINIT eth0 up
dhcp: BOND setting eth
mount.nfs: access denied by server while mounting 192.168.33.250:/srv/fai/nfsroot
.
.
dracut Warning: Could not boot
.
Dropping to debug shell
dracut:/#</code></pre>
</div></div>
<div class="paragraph"><p>Maintenant, vous êtes à l&#8217;intérieur du shell d&#8217;urgence de l&#8217;initrd qui a été créé par <em>dracut(8)</em>. Vous obtiendrez une invite du shell et pourrez consulter les fichiers journaux. Pour plus d&#8217;informations sur le débogage du processus de démarrage précoce à l&#8217;aide de dracut, consultez <code>dracut.cmdline(7)</code></p></div>
<div class="paragraph"><p>Utilisez la commande suivante sur le serveur d&#8217;installation pour voir quels répertoires sont exportés à partir du serveur d&#8217;installation (nommé faiserver):</p></div>
<div class="listingblock">
<div class="content">
<pre><code>$ showmount -e faiserver</code></pre>
</div></div>
</div>
</div>
</div>
</div>
<div id="footnotes"><hr /></div>
<div id="footer">
<div id="footer-text">
Version 5.3<br />
Last updated
 2017-04-26 23:45:58 CEST
</div>
</div>
</body>
</html>
