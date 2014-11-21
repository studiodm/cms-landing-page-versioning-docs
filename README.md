<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%'>The
following is the instructional guide to adding a new set of landing pages into
CMS and versioning them on to the marketing servers. The pages include city and
state navigation for search optimization along with city data. These are
additional include files that read XML files built from CMS and display onto
the landing pages.<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%'>This is an
example site structure as it resides on the server
(windstreamauthorizeddeals.com)<span class=GramE>:</span><br>
<b style='mso-bidi-font-weight:normal'>Example File Structure:</b><o:p></o:p></span></p>

<p class=MsoNormal><!--[if gte vml 1]><v:shapetype id="_x0000_t75" coordsize="21600,21600"
 o:spt="75" o:preferrelative="t" path="m@4@5l@4@11@9@11@9@5xe" filled="f"
 stroked="f">
 <v:stroke joinstyle="miter"/>
 <v:formulas>
  <v:f eqn="if lineDrawn pixelLineWidth 0"/>
  <v:f eqn="sum @0 1 0"/>
  <v:f eqn="sum 0 0 @1"/>
  <v:f eqn="prod @2 1 2"/>
  <v:f eqn="prod @3 21600 pixelWidth"/>
  <v:f eqn="prod @3 21600 pixelHeight"/>
  <v:f eqn="sum @0 0 1"/>
  <v:f eqn="prod @6 1 2"/>
  <v:f eqn="prod @7 21600 pixelWidth"/>
  <v:f eqn="sum @8 21600 0"/>
  <v:f eqn="prod @7 21600 pixelHeight"/>
  <v:f eqn="sum @10 21600 0"/>
 </v:formulas>
 <v:path o:extrusionok="f" gradientshapeok="t" o:connecttype="rect"/>
 <o:lock v:ext="edit" aspectratio="t"/>
</v:shapetype><v:shape id="Picture_x0020_1" o:spid="_x0000_s1026" type="#_x0000_t75"
 style='position:absolute;margin-left:0;margin-top:0;width:272.2pt;height:148.45pt;
 z-index:251658240;visibility:visible;mso-wrap-style:square;
 mso-wrap-distance-left:9pt;mso-wrap-distance-top:0;mso-wrap-distance-right:9pt;
 mso-wrap-distance-bottom:0;mso-position-horizontal:left;
 mso-position-horizontal-relative:text;mso-position-vertical:top;
 mso-position-vertical-relative:text'>
 <v:imagedata src="CMS%20-%20%20Adding%20and%20Versioning%20Landing%20Pages_files/image001.png"
  o:title=""/>
 <w:wrap type="square"/>
</v:shape><![endif]--><![if !vml]><img width=363 height=198
src="CMS%20-%20%20Adding%20and%20Versioning%20Landing%20Pages_files/image001.png"
align=left hspace=12 v:shapes="Picture_x0020_1"><![endif]><span
style='font-size:12.0pt;line-height:115%'><br clear=all style='mso-special-character:
line-break'>
<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%'>The <span
class=SpellE>php</span> files displayed are the standard for versioning and <span
class=SpellE>main.php</span> being a configuration file for the entire
versioned pages and connection to CMS. Inside the <span class=SpellE>php</span>
files is the <span class=SpellE>siteid</span> which is configured inside the
CMS. These must match. The <span class=SpellE>php</span> content also has a
pointer to each corresponding HTML file inside each versioned set of landing
pages. Example, <span class=SpellE>index.php</span>:<o:p></o:p></span></p>

<p class=MsoNormal><span style='mso-no-proof:yes'><!--[if gte vml 1]><v:shape
 id="Picture_x0020_3" o:spid="_x0000_i1027" type="#_x0000_t75" style='width:468pt;
 height:59.25pt;visibility:visible;mso-wrap-style:square'>
 <v:imagedata src="CMS%20-%20%20Adding%20and%20Versioning%20Landing%20Pages_files/image002.png"
  o:title=""/>
</v:shape><![endif]--><![if !vml]><img width=624 height=79
src="CMS%20-%20%20Adding%20and%20Versioning%20Landing%20Pages_files/image003.png"
v:shapes="Picture_x0020_3"><![endif]></span><span style='font-size:12.0pt;
line-height:115%'><o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%'>Inside the
versions directory resides each version and within each version reside the HTML
files and page assets as shown below:<br>
</span><span style='mso-no-proof:yes'><!--[if gte vml 1]><v:shape id="Picture_x0020_2"
 o:spid="_x0000_i1026" type="#_x0000_t75" style='width:208.5pt;height:146.25pt;
 visibility:visible;mso-wrap-style:square'>
 <v:imagedata src="CMS%20-%20%20Adding%20and%20Versioning%20Landing%20Pages_files/image004.png"
  o:title=""/>
</v:shape><![endif]--><![if !vml]><img width=278 height=195
src="CMS%20-%20%20Adding%20and%20Versioning%20Landing%20Pages_files/image004.png"
v:shapes="Picture_x0020_2"><![endif]></span><span style='font-size:12.0pt;
line-height:115%'><o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%'><o:p>&nbsp;</o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%'>Inside the <span
class=SpellE>cms_include</span> directory reside all the include files which
must be attached or plugged into each HTML page. Directory structure shown
below:<o:p></o:p></span></p>

<p class=MsoNormal><span style='mso-no-proof:yes'><!--[if gte vml 1]><v:shape
 id="Picture_x0020_4" o:spid="_x0000_i1025" type="#_x0000_t75" style='width:270pt;
 height:150pt;visibility:visible;mso-wrap-style:square'>
 <v:imagedata src="CMS%20-%20%20Adding%20and%20Versioning%20Landing%20Pages_files/image005.png"
  o:title=""/>
</v:shape><![endif]--><![if !vml]><img width=360 height=200
src="CMS%20-%20%20Adding%20and%20Versioning%20Landing%20Pages_files/image005.png"
v:shapes="Picture_x0020_4"><![endif]></span><span style='font-size:12.0pt;
line-height:115%'><o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%'><o:p>&nbsp;</o:p></span></p>

<p class=MsoListParagraph style='margin-left:.25in;mso-add-space:auto;
text-indent:-.25in;mso-list:l2 level1 lfo3'><![if !supportLists]><b
style='mso-bidi-font-weight:normal'><span style='font-size:12.0pt;line-height:
115%;mso-bidi-font-family:Calibri;mso-bidi-theme-font:minor-latin'><span
style='mso-list:Ignore'>2.<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span></span></b><![endif]><b style='mso-bidi-font-weight:normal'><span
style='font-size:12.0pt;line-height:115%'>Versioning <o:p></o:p></span></b></p>

<p class=MsoNormal><b style='mso-bidi-font-weight:normal'><span
style='font-size:12.0pt;line-height:115%'>The first step in creating a new
version</span></b><span style='font-size:12.0pt;line-height:115%'> is to create
a new numeric directory with in the versions directory. Example, if the last
version is 1.3 the next version would be 1.4 and so on.<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%'>Inside the
new version you will add the new HTML files and page assets.<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%'>You will
need to edit each HTML file and thus plug in the include files.<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%'><br
style='mso-special-character:line-break'>
<![if !supportLineBreakNewLine]><br style='mso-special-character:line-break'>
<![endif]><b style='mso-bidi-font-weight:normal'><o:p></o:p></b></span></p>

<p class=MsoNormal><b style='mso-bidi-font-weight:normal'><span
style='font-size:12.0pt;line-height:115%'><o:p>&nbsp;</o:p></span></b></p>

<p class=MsoListParagraph style='margin-left:.25in;mso-add-space:auto;
text-indent:-.25in;mso-list:l2 level1 lfo3'><![if !supportLists]><span
style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:Calibri;
mso-bidi-theme-font:minor-latin'><span style='mso-list:Ignore'>3.<span
style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span></span></span><![endif]><b
style='mso-bidi-font-weight:normal'><span style='font-size:12.0pt;line-height:
115%'>Adding Include Files<br>
<br>
Starting with the top of the HTML file or the Head</span></b><span
style='font-size:12.0pt;line-height:115%'> you will add the following include
files (example snippet from HTML file):<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-family:"Courier New";color:red'><o:p>&nbsp;</o:p></span></p>

<p class=MsoNormal><span style='font-family:"Courier New";color:red'>&lt;?<span
class=SpellE>php</span> include &quot;<span class=SpellE>cms_include</span>/<span
class=SpellE>curlConnXml.php</span>&quot;; ?&gt;</span><span style='font-family:
"Courier New"'><br>
&lt;!DOCTYPE HTML&gt;<br>
&lt;html&gt;<br>
&lt;head&gt;<br>
&lt;meta charset=&quot;utf-8&quot;&gt;<br>
<span style='color:red'>&lt;?<span class=SpellE>php</span> include &quot;<span
class=SpellE>cms_include</span>/<span class=SpellE>metaData.php</span>&quot;;
?&gt;</span><br>
&lt;meta http-<span class=SpellE>equiv</span>=&quot;X-UA-Compatible&quot;
content=&quot;IE=edge&quot;&gt;<br>
&lt;meta name=&quot;viewport&quot; content=&quot;width=device-width,
initial-scale=1.0&quot;&gt;<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-family:"Courier New"'><o:p>&nbsp;</o:p></span></p>

<p class=MsoNormal><span class=SpellE><span style='font-size:12.0pt;line-height:
115%;mso-bidi-font-family:"Courier New"'>The</span></span><span
style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:"Courier New"'>
include filenames are descriptive of the will display in that area of HTML.<br>
The first being a connection string to the City State XML � <span class=SpellE><b
style='mso-bidi-font-weight:normal'>curlConnXml.php</b></span><b
style='mso-bidi-font-weight:normal'><br>
</b><span class=GramE>This</span> include file does NOT display any data<b
style='mso-bidi-font-weight:normal'><br>
</b>The second, <span class=SpellE><b style='mso-bidi-font-weight:normal'>metaData.php</b></span>
handles meta tags including site title. <br>
<b style='mso-bidi-font-weight:normal'>NOTE:</b> If the following HTML meta
tags are in place, � TITLE, META CONTENT-DESCRIPTION, META CONTENT-KEYWORD�,
remove them and replace with the include file.<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'><o:p>&nbsp;</o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'>The next set of edits will be versioning the assets.<br>
<span class=GramE>all</span> asset <span class=SpellE>src</span> files will
need to be replaced as shown below:<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'><br>
<b style='mso-bidi-font-weight:normal'>Original<br>
</b>&lt;link <span class=SpellE>href</span>=&quot; assets/<span class=SpellE>css</span>/bootstrap.css&quot;
<span class=SpellE>rel</span>=&quot;<span class=SpellE>stylesheet</span>&quot;&gt;<o:p></o:p></span></p>

<p class=MsoNormal><b style='mso-bidi-font-weight:normal'><span
style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:"Courier New"'>Updated<br>
</span></b><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'>&lt;link <span class=SpellE>href</span>=&quot;/versions/&lt;<span
class=GramE>?<span class=SpellE>php</span></span> echo $<span class=SpellE>pathVersion</span>;
?&gt;/assets/<span class=SpellE>css</span>/bootstrap.css&quot; <span
class=SpellE>rel</span>=&quot;<span class=SpellE>stylesheet</span>&quot;&gt;<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'>This includes ALL <b style='mso-bidi-font-weight:normal'>CSS, JS</b>,
and <b style='mso-bidi-font-weight:normal'>IMG</b> assets.<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'>After the opening body tag, where ever you would like to display
breadcrumbs you can include the breadcrumbs include<span class=GramE>:</span><br>
<span style='color:red'>&lt;?<span class=SpellE>php</span> include (&quot;<span
class=SpellE>cms_include</span>/<span class=SpellE>breadcrumbs.php</span>&quot;);
?&gt;<o:p></o:p></span></span></p>

<p class=MsoNormal><b style='mso-bidi-font-weight:normal'><span
style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:"Courier New"'><o:p>&nbsp;</o:p></span></b></p>

<p class=MsoNormal><b style='mso-bidi-font-weight:normal'><span
style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:"Courier New"'><o:p>&nbsp;</o:p></span></b></p>

<p class=MsoNormal><b style='mso-bidi-font-weight:normal'><span
style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:"Courier New"'><o:p>&nbsp;</o:p></span></b></p>

<p class=MsoListParagraph style='margin-left:.25in;mso-add-space:auto;
text-indent:-.25in;mso-list:l2 level1 lfo3'><![if !supportLists]><b
style='mso-bidi-font-weight:normal'><span style='font-size:12.0pt;line-height:
115%;mso-bidi-font-family:Calibri;mso-bidi-theme-font:minor-latin'><span
style='mso-list:Ignore'>4.<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span></span></b><![endif]><b style='mso-bidi-font-weight:normal'><span
style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:"Courier New"'>Navigation<o:p></o:p></span></b></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'>The navigation of pages via anchor tag is not <span class=GramE>an
include</span> but rather a place holder that renders from the <span
class=SpellE>main.php</span> or configuration file. They are appropriately
named for ease of implementation. Below is an example of navigation:<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'><o:p>&nbsp;</o:p></span></p>

<p class=MsoNormal><span style='font-family:"Courier New"'>&lt;<span
class=SpellE>ul</span> class=&quot;<span class=SpellE>nav</span> <span
class=SpellE>navbar-nav</span>&quot;&gt;<br>
&lt;li class=&quot;active&quot;&gt;&lt;a <span class=SpellE>href</span>=&quot;<span
style='color:red'>&lt;?<span class=SpellE>php</span> echo $<span class=SpellE>navBundles</span>;
?&gt;</span>&quot;&gt;Bundles&lt;/a&gt;&lt;/li&gt;<br>
&lt;li&gt;&lt;a <span class=SpellE>href</span>=&quot;<span style='color:red'>&lt;?<span
class=SpellE>php</span> echo $<span class=SpellE>navTv</span>; ?&gt;</span>&quot;&gt;TV&lt;/a&gt;&lt;/li&gt;<br>
&lt;li&gt;&lt;a <span class=SpellE>href</span>=&quot;<span style='color:red'>&lt;?<span
class=SpellE>php</span> echo $<span class=SpellE>navInternet</span>; ?&gt;</span>&quot;&gt;Internet&lt;/a&gt;&lt;/li&gt;<br>
&lt;li&gt;&lt;a <span class=SpellE>href</span>=&quot;<span style='color:red'>&lt;?<span
class=SpellE>php</span> echo $<span class=SpellE>navPhone</span>; ?&gt;</span>&quot;&gt;Digital
Phone&lt;/a&gt;&lt;/li&gt;<br>
&lt;li class=&quot;last&quot;&gt;&lt;a <span class=SpellE>href</span>=&quot;<span
style='color:red'>&lt;?<span class=SpellE>php</span> echo $<span class=SpellE>navPaquetes</span>;
?&gt;</span>&quot;&gt;<span class=SpellE>Espanol</span>&lt;/a&gt;&lt;/li&gt;<br>
<span style='mso-spacerun:yes'>�</span>&lt;/<span class=SpellE>ul</span>&gt;<span
style='mso-spacerun:yes'>� </span><o:p></o:p></span></p>

<p class=MsoNormal><span style='font-family:"Courier New"'><o:p>&nbsp;</o:p></span></p>

<p class=MsoNormal><span style='font-family:"Courier New"'><o:p>&nbsp;</o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'><o:p>&nbsp;</o:p></span></p>

<p class=MsoListParagraph style='margin-left:.25in;mso-add-space:auto;
text-indent:-.25in;mso-list:l2 level1 lfo3'><![if !supportLists]><b
style='mso-bidi-font-weight:normal'><span style='font-size:12.0pt;line-height:
115%;mso-bidi-font-family:Calibri;mso-bidi-theme-font:minor-latin'><span
style='mso-list:Ignore'>5.<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span></span></b><![endif]><b style='mso-bidi-font-weight:normal'><span
style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:"Courier New"'>States
Links<o:p></o:p></span></b></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'>The following include file displays the footprint via links to
each state with in that footprint.<br>
This reads from the XML file and is controlled by CMS. This can be placed,
usually near the bottom of the page before the footer. It may be placed
anywhere within the HTML page.<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'>&lt;!--GET STATES--&gt;<br>
<span style='color:red'>&lt;<span class=GramE>?<span class=SpellE>php</span></span>
include ('<span class=SpellE>cms_include</span>/<span class=SpellE>getState.php</span>');
?&gt;<br>
</span>&lt;!--GET STATES--&gt;<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'><o:p>&nbsp;</o:p></span></p>

<p class=MsoListParagraph style='margin-left:.25in;mso-add-space:auto;
text-indent:-.25in;mso-list:l2 level1 lfo3'><![if !supportLists]><b
style='mso-bidi-font-weight:normal'><span style='font-size:12.0pt;line-height:
115%;mso-bidi-font-family:Calibri;mso-bidi-theme-font:minor-latin'><span
style='mso-list:Ignore'>6.<span style='font:7.0pt "Times New Roman"'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</span></span></span></b><![endif]><b style='mso-bidi-font-weight:normal'><span
style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:"Courier New"'>City
Data<o:p></o:p></span></b></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'>The city data include file can be placed below the state links.
This reads the <span class=SpellE>CityData</span> XML controlled from CMS and
displays pertinent data from the city selected via city navigation:<o:p></o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'>&lt;!--City Data--&gt;<br>
<span style='color:red'>&lt;<span class=GramE>?<span class=SpellE>php</span></span>
include ('<span class=SpellE>cms_include</span>/<span class=SpellE>cityData.php</span>');
?&gt;</span><br>
&lt;!--City Data--&gt;<b style='mso-bidi-font-weight:normal'><o:p></o:p></b></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%;mso-bidi-font-family:
"Courier New"'><o:p>&nbsp;</o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%'><o:p>&nbsp;</o:p></span></p>

<p class=MsoNormal><span style='font-size:12.0pt;line-height:115%'><o:p>&nbsp;</o:p></span></p>

</div>



