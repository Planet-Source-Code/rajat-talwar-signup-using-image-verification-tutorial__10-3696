<div align="center">

## Signup using Image Verification Tutorial


</div>

### Description

All Major Websites dealing with secure content, administrative rights and user privacy use image verification. an image is provided with a random string embossed on it and before registering the string has to be entered in the provided textbox. This can be easily seen at Yahoo. COM, gmail, planet source code (yes our very own PSC will ask you for this when you vote for me).
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[rajat talwar](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/rajat-talwar.md)
**Level**          |Beginner
**User Rating**    |4.6 (176 globes from 38 users)
**Compatibility**  |VB\.NET, ASP\.NET
**Category**       |[Validation/ Processing](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/validation-processing__10-16.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/rajat-talwar-signup-using-image-verification-tutorial__10-3696/archive/master.zip)





### Source Code

<html xmlns:o="urn:schemas-microsoft-com:office:office"
xmlns:w="urn:schemas-microsoft-com:office:word"
xmlns="http://www.w3.org/TR/REC-html40">
<head>
<meta http-equiv=Content-Type content="text/html; charset=windows-1252">
<meta name=ProgId content=FrontPage.Editor.Document>
<meta name=Generator content="Microsoft FrontPage 6.0">
<meta name=Originator content="Microsoft Word 11">
<title>Imports System</title>
<style>
<!--
 /* Font Definitions */
 @font-face
	{font-family:CourierNew;
	panose-1:0 0 0 0 0 0 0 0 0 0;
	mso-font-charset:0;
	mso-generic-font-family:roman;
	mso-font-format:other;
	mso-font-pitch:auto;
	mso-font-signature:3 0 0 0 1 0;}
@font-face
	{font-family:"Arial Black";
	panose-1:2 11 10 4 2 1 2 2 2 4;
	mso-font-charset:0;
	mso-generic-font-family:swiss;
	mso-font-pitch:variable;
	mso-font-signature:647 0 0 0 159 0;}
 /* Style Definitions */
 p.MsoNormal, li.MsoNormal, div.MsoNormal
	{mso-style-parent:"";
	margin:0in;
	margin-bottom:.0001pt;
	mso-pagination:widow-orphan;
	font-size:12.0pt;
	font-family:"Times New Roman";
	mso-fareast-font-family:"Times New Roman";}
h1
	{mso-style-next:Normal;
	margin-top:12.0pt;
	margin-right:0in;
	margin-bottom:3.0pt;
	margin-left:0in;
	mso-pagination:widow-orphan;
	page-break-after:avoid;
	mso-outline-level:1;
	font-size:16.0pt;
	font-family:Arial;
	mso-font-kerning:16.0pt;
	font-weight:bold;}
h2
	{mso-style-next:Normal;
	margin-top:12.0pt;
	margin-right:0in;
	margin-bottom:3.0pt;
	margin-left:0in;
	mso-pagination:widow-orphan;
	page-break-after:avoid;
	mso-outline-level:2;
	font-size:14.0pt;
	font-family:Arial;
	font-weight:bold;
	font-style:italic;}
p.MsoList, li.MsoList, div.MsoList
	{margin-top:0in;
	margin-right:0in;
	margin-bottom:0in;
	margin-left:.25in;
	margin-bottom:.0001pt;
	text-indent:-.25in;
	mso-pagination:widow-orphan;
	font-size:12.0pt;
	font-family:"Times New Roman";
	mso-fareast-font-family:"Times New Roman";}
p.MsoBodyText, li.MsoBodyText, div.MsoBodyText
	{margin-top:0in;
	margin-right:0in;
	margin-bottom:6.0pt;
	margin-left:0in;
	mso-pagination:widow-orphan;
	font-size:12.0pt;
	font-family:"Times New Roman";
	mso-fareast-font-family:"Times New Roman";}
p
	{font-size:12.0pt;
	font-family:"Times New Roman";
	mso-fareast-font-family:"Times New Roman";}
span.grame
	{mso-style-name:grame;}
span.SpellE
	{mso-style-name:"";
	mso-spl-e:yes;}
span.GramE
	{mso-style-name:"";
	mso-gram-e:yes;}
@page Section1
	{size:8.5in 11.0in;
	margin:1.0in 1.25in 1.0in 1.25in;
	mso-header-margin:.5in;
	mso-footer-margin:.5in;
	mso-paper-source:0;}
div.Section1
	{page:Section1;}
-->
</style>
</head>
<div class=Section1>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><b
style='mso-bidi-font-weight:normal'><span style='font-size:14.0pt;font-family:
"Arial Black"'>Signup using Image Verification Tutorial<o:p></o:p></span></b></p>
<p>All Major Websites dealing with secure content, administrative rights and
user privacy use image verification. an image is provided with a random string embossed
on it and before registering the string has to be entered in the provided
textbox. This can be easily seen at Yahoo. COM, gmail, planet source code (yes
our very own PSC will ask you for this when you vote for me). </p>
<p>Lets try and work
at producing such a random image so that it can be easily embedded in any of
professional website. I prefer working with classes so let’s develop a
verification class.</p>
<p>First we will import the required namespaces.</p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Imports
</span><span class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>System.Drawing.Text</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'> </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'for
font<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Imports
</span><span class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>System.Drawing.Imaging</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'> </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'for
saving the gif<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Imports
</span><span class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>System.Security.Cryptography</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'> </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'for
creating random String<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Public
Class </span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>Verification<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'>&nbsp;</p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'>
<span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Public
Function </span><span class=SpellE><span class=GramE><span style='font-family:
CourierNew;mso-bidi-font-family:CourierNew;color:black'>CreateImage</span></span></span><span
class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>(</span></span><span class=SpellE><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:blue'>ByVal</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'> </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>path
</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:blue'>As String</span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>, </span><span class=SpellE><span style='font-family:
CourierNew;mso-bidi-font-family:CourierNew;color:blue'>ByVal</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'> </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>height
</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:blue'>As Integer</span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>, </span><span class=SpellE><span style='font-family:
CourierNew;mso-bidi-font-family:CourierNew;color:blue'>ByVal</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'> </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>width<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>As
Integer</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>) </span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:blue'>As String<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'Creates
a Random Gif file of provided width and height<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'<span
class=GramE>the</span> string on the gif file is rotated randomly<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'<span
class=GramE>returns</span> the random string painted<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Dim </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>r </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>As
New </span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>Random </span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:#008100'>'to generate a random angle<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Dim </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>salt
</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:blue'>As String </span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>= <span class=SpellE><span class=GramE>CreateSalt</span></span><span
class=GramE>(</span>4) </span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:#008100'>'generates a random string<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Dim </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>bmp </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>As
New </span><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>Bitmap(</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'>width, height,
PixelFormat.Format24bppRgb) </span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:#008100'>'creates a<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>24bit
bitmap in memory<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Dim </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>g </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>As </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>Graphics
= <span class=SpellE><span class=GramE>Graphics.FromImage</span></span><span
class=GramE>(</span>bmp)<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>g.TextRenderingHint</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'> = <span class=SpellE>TextRenderingHint.AntiAlias</span>
</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:#008100'>'this will <span class=SpellE>smoothen</span> the Font<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>g.Clear</span></span></span><span class=GramE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>(</span></span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>Color.Black</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'>) </span><span style='font-family:
CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'this clears the
background and paints specified color<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>g.DrawRectangle</span></span></span><span class=GramE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>(</span></span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>Pens.White</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'>, 1, 1, width - 3, height - 3)<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>g.DrawRectangle</span></span></span><span class=GramE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>(</span></span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>Pens.Black</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'>, 0, 0, width, height)<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Dim </span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>mymat</span></span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'> </span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:blue'>As New </span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'>System.Drawing.Drawing2D.Matrix </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'matrix
used for rotation<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:#008100'>transformation</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:#008100'><o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Dim </span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>i</span></span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'> </span><span class=GramE><span style='font-family:
CourierNew;mso-bidi-font-family:CourierNew;color:blue'>As</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>
Integer<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>For </span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>i</span></span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'> = 0 </span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:blue'>To </span><span class=GramE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>Len(</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>salt)
- 1 </span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:#008100'>'we will rotate each literal at a specified angle<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>mymat.Reset</span></span></span><span class=GramE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>()</span></span><o:p><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>&nbsp;&nbsp;&nbsp; </span>
<font color="#FF0000">
<span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;'>' matrix should
be initialized to identity matrix</span></font></o:p></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>mymat.RotateAt</span></span></span><span class=GramE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>(</span></span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>r.Next</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'>(-30, 0), </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>New </span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>PointF</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'>(width * (0.12 * <span
class=SpellE>i</span>), height * 0.5))<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'<span
class=GramE>rotate</span> at any angle b/w -30 and 0</span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>g.Transform</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'> = <span class=SpellE>mymat</span>
</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:#008100'>'apply the transform<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>g.DrawString</span></span></span><span class=GramE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>(</span></span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>salt.Chars</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'>(<span class=SpellE>i</span>), </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>New </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>Font(&quot;Comic
Sans MS&quot;, 10, <span class=SpellE>FontStyle.Italic</span>),<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>SystemBrushes.ActiveCaptionText</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>,
width * (0.12 * <span class=SpellE>i</span>), height * 0.5) </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'draw
the text on<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:#008100'>our</span></span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:#008100'> image<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>g.ResetTransform</span></span></span><span class=GramE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>()</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'><o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Next<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>bmp.Save</span></span></span><span class=GramE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>(</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>path,
<span class=SpellE>ImageFormat.Gif</span>) </span><span style='font-family:
CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'save the gif at
specified path and name<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>g.Dispose</span></span></span><span class=GramE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>(</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>) </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'clean
up<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>bmp.Dispose</span></span></span><span class=GramE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>(</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>) </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'ok
the mess is over<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Return
</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>salt </span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:#008100'>'return the string painted for verification<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>End
Function</span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'>&nbsp;</p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Public
Function </span><span class=SpellE><span class=GramE><span style='font-family:
CourierNew;mso-bidi-font-family:CourierNew;color:black'>CreateSalt</span></span></span><span
class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>(</span></span><span class=SpellE><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:blue'>ByVal</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'> </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>size
</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:blue'>As Integer</span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>) </span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:blue'>As String<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:#008100'>' Generate</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:#008100'> a cryptographic random number
using the cryptographic<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:#008100'>' service</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:#008100'> provider<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Dim </span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>rng</span></span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'> </span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:blue'>As New </span><span class=SpellE><span style='font-family:
CourierNew;mso-bidi-font-family:CourierNew;color:black'>RNGCryptoServiceProvider</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'><o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Dim </span><span
class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>buff(</span></span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>size) </span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:blue'>As Byte<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>rng.GetBytes</span></span></span><span class=GramE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>(</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>buff)<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:#008100'>' Return</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:#008100'> a Base64 string representation
of the random number<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Return
</span><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>Convert.ToBase64String(</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>buff)<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>End
Function<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>End
Class</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'><o:p></o:p></span></p>
<p class=MsoNormal><span style='font-size:10.0pt'><o:p>&nbsp;</o:p></span></p>
<p>Here I have used a single font. You may use different fonts for each
literal. This can be easily done by storing different font family names in an
array</p>
<p>Now let’s get on with “How to use the class”. Drop an image box, label,
textbox and a button from the toolbox to an aspx page use image box ‘id=image
height=100, width=200; button id=btnRegister; textbox id=textbox1; label id=<span
class=SpellE>lblMessage</span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Private
Sub </span><span class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>Page_<span class=GramE>Load</span></span></span><span
class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>(</span></span><span class=SpellE><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:blue'>ByVal</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'> </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>sender
</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:blue'>As </span><span class=SpellE><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'>System.Object</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>, </span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:blue'>ByVal</span></span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:blue'> </span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>e </span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:blue'>As </span><span class=SpellE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>System.EventArgs</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>)<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Handles
<span class=SpellE>MyBase<span style='color:black'>.Load</span></span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'><o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:#008100'>'Put
user code to initialize the page here<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>If
Not </span><span class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>Page.IsPostBack</span></span><span style='font-family:
CourierNew;mso-bidi-font-family:CourierNew;color:black'> </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Then<o:p>&nbsp;&nbsp;&nbsp; </o:p></span><o:p>
<font color="#FF0000">
<span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;'>'we do not want
picture to be created when page is postback</span></font></o:p></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'>
<font color="#FF0000">'postback happens when asp.net fires it's control's event</font></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Dim </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>verify
</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:blue'>As New </span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>Verification<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Dim </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>salt
</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:blue'>As String </span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>= <span class=SpellE><span class=GramE>verify.CreateImage</span></span><span
class=GramE>(</span><span class=SpellE>Server.MapPath</span>(&quot;.\<span
class=SpellE>Random.gif</span>&quot;), 100,<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>200)<o:p>&nbsp;&nbsp;&nbsp; </o:p></span><o:p>
<font color="#FF0000">
<span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;'>'I have created
a file named Random.gif in the same directory as my web page size 100,200</span></font></o:p></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>Image.ImageUrl</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'> = <span class=SpellE><span
class=GramE>Server.MapPath</span></span><span class=GramE>(</span>&quot;.\<span
class=SpellE>Random.gif</span>&quot;)<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>Session.Add</span></span></span><span class=GramE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>(</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>&quot;salt&quot;,
salt)<o:p>&nbsp;&nbsp;&nbsp; </o:p></span><o:p>
<span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;'>
<font color="#FF0000">'Add our salt to session for verification so that we can
check on postback</font></span></o:p></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Dim </span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>params</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'> </span><span style='font-family:
CourierNew;mso-bidi-font-family:CourierNew;color:blue'>As </span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>System.Collections.Specialized.NameValueCollection</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'><o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>params</span></span></span><span style='font-family:
CourierNew;mso-bidi-font-family:CourierNew;color:black'> = <span class=SpellE>Request.QueryString</span>()<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>If </span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>params.Count</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'> &gt; 0 </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Then </span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>lblMessage.Text</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'> = <span class=SpellE><span
class=GramE>params.Item</span></span><span class=GramE>(</span>&quot;reason&quot;)<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>End
If<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>End
Sub</span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'>&nbsp;</p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Private
Sub </span><span class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>btnRegister_<span class=GramE>Click</span></span></span><span
class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>(</span></span><span class=SpellE><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:blue'>ByVal</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'> </span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>sender
</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:blue'>As </span><span class=SpellE><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'>System.Object</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>, </span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:blue'>ByVal</span></span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:blue'> </span><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>e </span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:blue'>As </span><span style='font-family:
CourierNew;mso-bidi-font-family:CourierNew;color:black'>System.<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>EventArgs</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'>) </span><span style='font-family:
CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Handles </span><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>btnRegister.Click</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'><o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>If
Not </span><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>TextBox1.Text.Equals(</span></span><span class=SpellE><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>Session.Item</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>(&quot;salt&quot;))
</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:blue'>Then<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:
CourierNew;color:black'>Response.Redirect</span></span></span><span
class=GramE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'>(</span></span><span class=SpellE><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:black'>Request.Url.ToString</span></span><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:black'>
&amp; &quot;?reason=The Strings did not match&quot;)<o:p>&nbsp;&nbsp;&nbsp; </o:p></span><o:p>
<span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;'>
<font color="#FF0000">'if we donot do it page will be considered a postback</font></span></o:p></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>Else<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
class=SpellE><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:blue'>lblMessage.text</span></span><span style='font-family:CourierNew;
mso-bidi-font-family:CourierNew;color:blue'>=”Good Boy”<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>End
If<o:p></o:p></span></p>
<p class=MsoNormal style='mso-layout-grid-align:none;text-autospace:none'><span
style='font-family:CourierNew;mso-bidi-font-family:CourierNew;color:blue'>End
Sub</span><span style='font-family:CourierNew;mso-bidi-font-family:CourierNew;
color:black'><o:p></o:p></span></p>
<p class=MsoNormal><span style='font-size:10.0pt'><o:p>&nbsp;</o:p></span></p>
<p>I have used sessions here. U can also use encrypted cookies or encrypted <span
class=SpellE><span class=GramE><span class=grame>url</span></span></span>
passing. <o:p></o:p></p>
<p>Keep in mind size of proportion b/w size of your image box and size of image
you are creating. This affects your image’s clarity and also font may go out of
bounds<o:p></o:p></p>
<p>Plz vote for me and you can request working demo at my email id<o:p></o:p></p>
<p>&nbsp;<o:p></o:p></p>
<p><o:p>&nbsp;</o:p></p>
<p>&nbsp;</p>
</div>
</html>

