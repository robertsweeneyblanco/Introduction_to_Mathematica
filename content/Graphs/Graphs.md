<!-- Created with the Wolfram Language for Students - Personal Use Only : www.wolfram.com -->

<html xmlns="http://www.w3.org/1999/xhtml">
<head>
 <title>
  Untitled (the Wolfram Language for Students - Personal Use Only : www.wolfram.com)
 </title>
 <link href="HTMLFiles/Graphs.css" rel="stylesheet" type="text/css" />
 <style>
 .Input {
  border-style: inset;
}
 </style>
</head>

<body>

<p class="Section">
 Graph algorithms
</p>



<p class="Text">
 There is sophisticated built-in support for graphs and graph algorithms
</p>



<p class="Text">
 There are lots of built-in graphs obtainable using GraphData, e.g.
</p>



<p class="Input">
 <img src="HTMLFiles/Graphs_1.png" alt="Graphs_1.png" width="86" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Graphs_2.png" alt="Graphs_2.png" width="606" height="188" style="vertical-align:middle;" usemap="#map_2" />
<map name="map_2">
<area shape="rect" coords="13,178,72,168" title="Dynamic[FEPrivate`FrontEndResource[FEStrings, sizeExplanation]]" nohref="" />
</map>
</p>

<p class="Input">
 <img src="HTMLFiles/Graphs_3.png" alt="Graphs_3.png" width="284" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Graphs_4.gif" alt="Graphs_4.gif" width="360" height="165" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Graphs_5.png" alt="Graphs_5.png" width="257" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Graphs_6.gif" alt="Graphs_6.gif" width="360" height="170" style="vertical-align:middle" />
</p>

<p class="Text">
 Let&rsquo;s perform a <span style='font-weight: bold;'>depth-first search </span>on this tree
</p>



<p class="Text">
 We start with the root node (33) in our case, and visit each node in the graph by first visiting all the children of a given node before visiting any of its siblings
</p>



<p class="Input">
 <img src="HTMLFiles/Graphs_7.png" alt="Graphs_7.png" width="102" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 We will need to find the neighbors of a given node:
</p>



<p class="Input">
 <img src="HTMLFiles/Graphs_8.png" alt="Graphs_8.png" width="200" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Graphs_9.png" alt="Graphs_9.png" width="103" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 We also don&rsquo;t want to visit our parent, so we will use Cases and Except to skip items
</p>



<p class="Input">
 <img src="HTMLFiles/Graphs_10.png" alt="Graphs_10.png" width="146" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Graphs_11.png" alt="Graphs_11.png" width="53" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Graphs_12.png" alt="Graphs_12.png" width="293" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Graphs_13.png" alt="Graphs_13.png" width="24" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Graphs_14.gif" alt="Graphs_14.gif" width="449" height="123" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Graphs_15.png" alt="Graphs_15.png" width="131" height="17" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_16.png" alt="Graphs_16.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_17.png" alt="Graphs_17.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_18.png" alt="Graphs_18.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_19.png" alt="Graphs_19.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_20.png" alt="Graphs_20.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_21.png" alt="Graphs_21.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_22.png" alt="Graphs_22.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_23.png" alt="Graphs_23.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_24.png" alt="Graphs_24.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_25.png" alt="Graphs_25.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_26.png" alt="Graphs_26.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_27.png" alt="Graphs_27.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_28.png" alt="Graphs_28.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_29.png" alt="Graphs_29.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_30.png" alt="Graphs_30.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_31.png" alt="Graphs_31.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_32.png" alt="Graphs_32.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_33.png" alt="Graphs_33.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_34.png" alt="Graphs_34.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_35.png" alt="Graphs_35.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_36.png" alt="Graphs_36.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_37.png" alt="Graphs_37.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_38.png" alt="Graphs_38.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_39.png" alt="Graphs_39.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_40.png" alt="Graphs_40.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_41.png" alt="Graphs_41.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_42.png" alt="Graphs_42.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_43.png" alt="Graphs_43.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_44.png" alt="Graphs_44.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_45.png" alt="Graphs_45.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_46.png" alt="Graphs_46.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_47.png" alt="Graphs_47.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_48.png" alt="Graphs_48.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Graphs_49.png" alt="Graphs_49.png" width="532" height="17" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_50.png" alt="Graphs_50.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_51.png" alt="Graphs_51.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_52.png" alt="Graphs_52.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_53.png" alt="Graphs_53.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_54.png" alt="Graphs_54.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_55.png" alt="Graphs_55.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_56.png" alt="Graphs_56.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_57.png" alt="Graphs_57.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_58.png" alt="Graphs_58.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_59.png" alt="Graphs_59.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_60.png" alt="Graphs_60.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_61.png" alt="Graphs_61.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_62.png" alt="Graphs_62.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_63.png" alt="Graphs_63.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_64.png" alt="Graphs_64.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_65.png" alt="Graphs_65.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_66.png" alt="Graphs_66.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_67.png" alt="Graphs_67.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_68.png" alt="Graphs_68.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_69.png" alt="Graphs_69.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_70.png" alt="Graphs_70.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_71.png" alt="Graphs_71.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_72.png" alt="Graphs_72.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_73.png" alt="Graphs_73.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_74.png" alt="Graphs_74.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_75.png" alt="Graphs_75.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_76.png" alt="Graphs_76.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_77.png" alt="Graphs_77.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_78.png" alt="Graphs_78.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_79.png" alt="Graphs_79.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_80.png" alt="Graphs_80.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_81.png" alt="Graphs_81.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_82.png" alt="Graphs_82.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Graphs_83.png" alt="Graphs_83.png" width="548" height="17" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_84.png" alt="Graphs_84.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_85.png" alt="Graphs_85.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_86.png" alt="Graphs_86.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_87.png" alt="Graphs_87.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_88.png" alt="Graphs_88.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_89.png" alt="Graphs_89.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_90.png" alt="Graphs_90.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_91.png" alt="Graphs_91.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_92.png" alt="Graphs_92.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_93.png" alt="Graphs_93.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_94.png" alt="Graphs_94.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_95.png" alt="Graphs_95.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_96.png" alt="Graphs_96.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_97.png" alt="Graphs_97.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_98.png" alt="Graphs_98.png" width="72" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_99.png" alt="Graphs_99.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_100.png" alt="Graphs_100.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_101.png" alt="Graphs_101.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_102.png" alt="Graphs_102.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_103.png" alt="Graphs_103.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_104.png" alt="Graphs_104.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_105.png" alt="Graphs_105.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_106.png" alt="Graphs_106.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_107.png" alt="Graphs_107.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_108.png" alt="Graphs_108.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_109.png" alt="Graphs_109.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_110.png" alt="Graphs_110.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_111.png" alt="Graphs_111.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_112.png" alt="Graphs_112.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_113.png" alt="Graphs_113.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_114.png" alt="Graphs_114.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_115.png" alt="Graphs_115.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Graphs_116.png" alt="Graphs_116.png" width="79" height="16" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Graphs_117.png" alt="Graphs_117.png" width="199" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Graphs_118.png" alt="Graphs_118.png" width="182" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Graphs_119.png" alt="Graphs_119.png" width="638" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Graphs_120.gif" alt="Graphs_120.gif" width="360" height="345" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Graphs_121.png" alt="Graphs_121.png" width="219" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Graphs_122.png" alt="Graphs_122.png" width="511" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Graphs_123.png" alt="Graphs_123.png" width="467" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Graphs_124.gif" alt="Graphs_124.gif" width="360" height="275" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Graphs_125.png" alt="Graphs_125.png" width="382" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Graphs_126.png" alt="Graphs_126.png" width="601" height="60" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Graphs_127.png" alt="Graphs_127.png" width="503" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Graphs_128.gif" alt="Graphs_128.gif" width="360" height="343" style="vertical-align:middle" />
</p>




<div style="font-family:Helvetica; font-size:11px; width:100%; border:1px none #999999; border-top-style:solid; padding-top:2px; margin-top:20px;">
 <a href="http://www.wolfram.com/language/" style="color:#000; text-decoration:none;">
  <span style="color:#555555">Created with the Wolfram Language</span> 
 </a>
</div>
</body>

</html>
