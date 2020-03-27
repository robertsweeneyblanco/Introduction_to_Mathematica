<!-- Created with the Wolfram Language for Students - Personal Use Only : www.wolfram.com -->

<html xmlns="http://www.w3.org/1999/xhtml">
<head>
 <title>
  Untitled (the Wolfram Language for Students - Personal Use Only : www.wolfram.com)
 </title>
 <link href="HTMLFiles/Compiling_and_Generating_Code.css" rel="stylesheet" type="text/css" />
 <style>
 .Input {
  border-style: inset;
}
 </style>
</head>

<body>

<p class="Section">
 Code compilation
</p>



<p class="Text">
 Mathematica code is by default interpreted by the Mathematica kernel
</p>



<p class="Text">
 The kernel can also <span style='font-weight: bold;'>compile</span> a subset of Mathematica code for better performance
</p>



<p class="Text">
 e.g. approximate &pi; numerically
</p>



<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_1.png" alt="Compiling_and_Generating_Code_1.png" width="218" height="38" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Compiling_and_Generating_Code_2.png" alt="Compiling_and_Generating_Code_2.png" width="13" height="30" style="vertical-align:middle" />
</p>

<p class="Text">
 Truncate this sum at <span style='font-style: italic;'>n</span> terms
</p>



<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_3.png" alt="Compiling_and_Generating_Code_3.png" width="309" height="39" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_4.png" alt="Compiling_and_Generating_Code_4.png" width="159" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Compiling_and_Generating_Code_5.png" alt="Compiling_and_Generating_Code_5.png" width="47" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_6.png" alt="Compiling_and_Generating_Code_6.png" width="252" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Compiling_and_Generating_Code_7.png" alt="Compiling_and_Generating_Code_7.png" width="123" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_8.png" alt="Compiling_and_Generating_Code_8.png" width="713" height="39" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Compiling_and_Generating_Code_9.gif" alt="Compiling_and_Generating_Code_9.gif" width="328" height="45" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_10.png" alt="Compiling_and_Generating_Code_10.png" width="206" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Compiling_and_Generating_Code_11.png" alt="Compiling_and_Generating_Code_11.png" width="138" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_12.png" alt="Compiling_and_Generating_Code_12.png" width="243" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_13.png" alt="Compiling_and_Generating_Code_13.png" width="126" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Compiling_and_Generating_Code_14.png" alt="Compiling_and_Generating_Code_14.png" width="289" height="753" style="vertical-align:middle" />
</p>

<p class="Section">
 Generating code
</p>



<p class="Text">
 
</p>



<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_15.png" alt="Compiling_and_Generating_Code_15.png" width="188" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_16.png" alt="Compiling_and_Generating_Code_16.png" width="528" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Compiling_and_Generating_Code_17.png" alt="Compiling_and_Generating_Code_17.png" width="654" height="1761" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_18.png" alt="Compiling_and_Generating_Code_18.png" width="513" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Compiling_and_Generating_Code_19.png" alt="Compiling_and_Generating_Code_19.png" width="713" height="690" style="vertical-align:middle" />
</p>

<p class="Section">
 JIT Compilation
</p>



<p class="Text">
 Suppose we want to roll our own JIT compilation
</p>



<p class="Text">
 We want to speed up Select, which returns those elements of a list that match a pattern
</p>



<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_20.png" alt="Compiling_and_Generating_Code_20.png" width="328" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_21.png" alt="Compiling_and_Generating_Code_21.png" width="317" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Compiling_and_Generating_Code_22.png" alt="Compiling_and_Generating_Code_22.png" width="62" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_23.png" alt="Compiling_and_Generating_Code_23.png" width="686" height="102" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_24.png" alt="Compiling_and_Generating_Code_24.png" width="340" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Compiling_and_Generating_Code_25.png" alt="Compiling_and_Generating_Code_25.png" width="62" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_26.png" alt="Compiling_and_Generating_Code_26.png" width="340" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Compiling_and_Generating_Code_27.png" alt="Compiling_and_Generating_Code_27.png" width="62" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_28.png" alt="Compiling_and_Generating_Code_28.png" width="348" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Compiling_and_Generating_Code_29.png" alt="Compiling_and_Generating_Code_29.png" width="62" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Compiling_and_Generating_Code_30.png" alt="Compiling_and_Generating_Code_30.png" width="348" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Compiling_and_Generating_Code_31.png" alt="Compiling_and_Generating_Code_31.png" width="62" height="17" style="vertical-align:middle" />
</p>




<div style="font-family:Helvetica; font-size:11px; width:100%; border:1px none #999999; border-top-style:solid; padding-top:2px; margin-top:20px;">
 <a href="http://www.wolfram.com/language/" style="color:#000; text-decoration:none;">
  <span style="color:#555555">Created with the Wolfram Language</span> 
 </a>
</div>
</body>

</html>
