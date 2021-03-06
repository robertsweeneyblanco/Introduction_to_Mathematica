<!-- Created with the Wolfram Language for Students - Personal Use Only : www.wolfram.com -->

<html xmlns="http://www.w3.org/1999/xhtml">
<head>
 <title>
  Untitled (the Wolfram Language for Students - Personal Use Only : www.wolfram.com)
 </title>
 <link href="HTMLFiles/Functional_Programming.css" rel="stylesheet" type="text/css" />
 <style>
 .Input {
  border-style: inset;
}
 </style>
</head>

<body>

<p class="Section">
 Defining functions
</p>



<p class="Text">
 Functions are just another type of expression in Mathematica
</p>



<p class="Text">
 Their argument lists take the form of <span style='font-weight: bold;'>patterns. </span>We will discuss patterns in more depth in the next lecture
</p>



<p class="Text">
 For now, we will make use of one kind of pattern: <span style='font-style: italic;font-weight: bold;'>x_<br /></span>which matches any expression and calls it <span style='font-style: italic;'>x.<br /></span><span style='font-weight: bold;'>For example:</span>
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_1.png" alt="Functional_Programming_1.png" width="134" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 This function can be called with any kind of argument. That argument will be called <span style='font-style: italic;'>x</span> in the body of the function, which gives a result by adding one
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_2.png" alt="Functional_Programming_2.png" width="71" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_3.png" alt="Functional_Programming_3.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_4.png" alt="Functional_Programming_4.png" width="129" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_5.png" alt="Functional_Programming_5.png" width="66" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 There are much more sophisticated patterns than just &ldquo;match any expression.&rdquo; We will cover these later.
</p>



<p class="Text">
 Suppose we want to recursively compute the factorial<br />Base case: fac(0) = 1<br />Recursive definition: fac(n) = n*fac(n-1)
</p>



<p class="Text">
 This is simple to define in Mathematica.<br />We begin with the base case
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_6.png" alt="Functional_Programming_6.png" width="79" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Now, fac[0] will evaluate to 1
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_7.png" alt="Functional_Programming_7.png" width="47" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_8.png" alt="Functional_Programming_8.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 We don&rsquo;t have a rule for the general case, so fac[n] will remain unevaluated:
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_9.png" alt="Functional_Programming_9.png" width="47" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_10.png" alt="Functional_Programming_10.png" width="47" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Defining the general case:
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_11.png" alt="Functional_Programming_11.png" width="170" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_12.png" alt="Functional_Programming_12.png" width="47" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_13.png" alt="Functional_Programming_13.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_14.png" alt="Functional_Programming_14.png" width="55" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_15.png" alt="Functional_Programming_15.png" width="59" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_16.png" alt="Functional_Programming_16.png" width="26" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_17.png" alt="Functional_Programming_17.png" width="59" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Let&rsquo;s do a similar exercise with the Fibonacci sequence:<br /><span><span><img src="HTMLFiles/Functional_Programming_18.gif" alt="Functional_Programming_18.gif" width="88" height="68" style="vertical-align:middle" /></span></span>
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_19.gif" alt="Functional_Programming_19.gif" width="233" height="60" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_20.png" alt="Functional_Programming_20.png" width="55" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_21.png" alt="Functional_Programming_21.png" width="16" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Of course, Mathematica also has this built in, so we can check our work...
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_22.png" alt="Functional_Programming_22.png" width="102" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_23.png" alt="Functional_Programming_23.png" width="16" height="17" style="vertical-align:middle" />
</p>

<p class="Section">
 Solving recurrence relations
</p>



<p class="Text">
 Suppose we have the recurrence relation
</p>



<p class="Text">
 <span><span><img src="HTMLFiles/Functional_Programming_24.png" alt="Functional_Programming_24.png" width="688" height="72" style="vertical-align:middle" /></span></span>
</p>



<p class="Text">
 We can easily create a function to recursively evaluate this sequence
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_25.gif" alt="Functional_Programming_25.gif" width="218" height="60" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_26.png" alt="Functional_Programming_26.png" width="40" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_27.png" alt="Functional_Programming_27.png" width="68" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 What if we want to know a general (non-recursive formula)?<br />First, concentrate on the recursive definition <span><span><img src="HTMLFiles/Functional_Programming_28.png" alt="Functional_Programming_28.png" width="117" height="19" style="vertical-align:middle" /></span></span> (ignoring boundary conditions)<br />We can solve this recurrence by making the ansatz that <span><span><img src="HTMLFiles/Functional_Programming_29.png" alt="Functional_Programming_29.png" width="15" height="19" style="vertical-align:middle" /></span></span>is given by <span><span><img src="HTMLFiles/Functional_Programming_30.png" alt="Functional_Programming_30.png" width="13" height="19" style="vertical-align:middle" /></span></span> for some <span style='font-style: italic;'>r<br /></span>In that case,
</p>



<p class="Text">
 <span><span><img src="HTMLFiles/Functional_Programming_31.png" alt="Functional_Programming_31.png" width="688" height="23" style="vertical-align:middle" /></span></span>
</p>



<p class="Text">
 So, we look for solutions to this equation.
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_32.png" alt="Functional_Programming_32.png" width="141" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_33.png" alt="Functional_Programming_33.png" width="113" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 So, <span><em>r</em><em>=</em><em>5</em></span> and <span><em>r</em><em>=</em><em>2</em></span> satisfy this relationship.<br />The general solution will be given by <span><span><img src="HTMLFiles/Functional_Programming_34.png" alt="Functional_Programming_34.png" width="106" height="19" style="vertical-align:middle" /></span></span>
</p>



<p class="Text">
 We can easily solve the system of equations to find the values of <span style='font-style: italic;'>c</span> and <span style='font-style: italic;'>d</span>.<br />But we can also let Mathematica help...
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_35.gif" alt="Functional_Programming_35.gif" width="143" height="60" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_36.png" alt="Functional_Programming_36.png" width="66" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_37.png" alt="Functional_Programming_37.png" width="30" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_38.png" alt="Functional_Programming_38.png" width="52" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_39.png" alt="Functional_Programming_39.png" width="319" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_40.png" alt="Functional_Programming_40.png" width="130" height="34" style="vertical-align:middle" />
</p>

<p class="Text">
 Let&rsquo;s check our formula
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_41.png" alt="Functional_Programming_41.png" width="110" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_42.png" alt="Functional_Programming_42.png" width="74" height="36" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_43.png" alt="Functional_Programming_43.png" width="252" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_44.png" alt="Functional_Programming_44.png" width="31" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 ClearAll deletes all the definitions we made for a
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_45.png" alt="Functional_Programming_45.png" width="86" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Mathematica can also solve the recurrence directly using RSolve
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_46.png" alt="Functional_Programming_46.png" width="471" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_47.png" alt="Functional_Programming_47.png" width="268" height="34" style="vertical-align:middle" />
</p>

<p class="Section">
 More complicated functions and local variables
</p>



<p class="Text">
 Sometimes we want to introduce local variables in a function for intermediate values in long calculations
</p>



<p class="Text">
 This can be achieved using Module
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_48.png" alt="Functional_Programming_48.png" width="66" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_49.png" alt="Functional_Programming_49.png" width="174" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_50.png" alt="Functional_Programming_50.png" width="354" height="207" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_51.png" alt="Functional_Programming_51.png" width="57" height="16" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_52.png" alt="Functional_Programming_52.png" width="121" height="17" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_53.png" alt="Functional_Programming_53.png" width="166" height="16" style="vertical-align:middle" />
</p>

<p class="Text">
 Mathematica also has other <span style='font-weight: bold;'>scoping mechanisms</span> (i.e. for creating variables with local scope)<br />See e.g. Block, With
</p>



<p class="Text">
 For our uses, Module is sufficient
</p>



<p class="Section">
 Functional style programming
</p>



<p class="Text">
 Mathematica is a <span style='font-weight: bold;'>multi-paradigm</span> programming language
</p>



<p class="Text">
 It supports both functional and imperative programming, but functional constructs are often very natural
</p>



<p class="Text">
 For example, applying a function f to a list is known as mapping f over the list
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_54.png" alt="Functional_Programming_54.png" width="220" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_55.png" alt="Functional_Programming_55.png" width="276" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_56.png" alt="Functional_Programming_56.png" width="130" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_57.png" alt="Functional_Programming_57.png" width="221" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Map is considered so important in Mathematica it has its own syntax
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_58.png" alt="Functional_Programming_58.png" width="100" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_59.png" alt="Functional_Programming_59.png" width="221" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 We can define more complicated functions if we want
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_60.png" alt="Functional_Programming_60.png" width="201" height="20" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_61.png" alt="Functional_Programming_61.png" width="107" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_62.png" alt="Functional_Programming_62.png" width="580" height="43" style="vertical-align:middle" />
</p>

<p class="Text">
 Sometimes we want to create an <span style='font-weight: bold;'>anonymous function </span>so that we don&rsquo;t need to name it
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_63.png" alt="Functional_Programming_63.png" width="248" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_64.png" alt="Functional_Programming_64.png" width="580" height="43" style="vertical-align:middle" />
</p>

<p class="Text">
 Here # indicates the argument, and &amp; tells Mathematica that the preceding expression is a function
</p>



<p class="Text">
 This notation can easily become hard to read, so be careful
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_65.png" alt="Functional_Programming_65.png" width="218" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_66.png" alt="Functional_Programming_66.png" width="580" height="43" style="vertical-align:middle" />
</p>

<p class="Section">
 More functional programming
</p>



<p class="Text">
 Recall our list
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_67.png" alt="Functional_Programming_67.png" width="47" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_68.png" alt="Functional_Programming_68.png" width="276" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 We can apply filters to the list using Select
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_69.png" alt="Functional_Programming_69.png" width="162" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_70.png" alt="Functional_Programming_70.png" width="147" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 We can combine this with anonymous functions
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_71.png" alt="Functional_Programming_71.png" width="176" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_72.png" alt="Functional_Programming_72.png" width="184" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Sometimes we want to apply a function to a list for its side-effect rather than its return-value
</p>



<p class="Text">
 For this we have Scan
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_73.png" alt="Functional_Programming_73.png" width="230" height="17" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_74.png" alt="Functional_Programming_74.png" width="7" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_75.png" alt="Functional_Programming_75.png" width="7" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_76.png" alt="Functional_Programming_76.png" width="7" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_77.png" alt="Functional_Programming_77.png" width="7" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_78.png" alt="Functional_Programming_78.png" width="7" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_79.png" alt="Functional_Programming_79.png" width="7" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_80.png" alt="Functional_Programming_80.png" width="7" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_81.png" alt="Functional_Programming_81.png" width="7" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_82.png" alt="Functional_Programming_82.png" width="7" height="16" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_83.png" alt="Functional_Programming_83.png" width="14" height="16" style="vertical-align:middle" />
</p>

<p class="Text">
 There are a ton more functional programming facilities in Mathematica
</p>



<p class="Text">
 See e.g. Nest, Fold, Apply
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_84.png" alt="Functional_Programming_84.png" width="262" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_85.png" alt="Functional_Programming_85.png" width="559" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Can we get the sum of all of these entries?
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_86.png" alt="Functional_Programming_86.png" width="94" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_87.png" alt="Functional_Programming_87.png" width="559" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_88.png" alt="Functional_Programming_88.png" width="113" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_89.png" alt="Functional_Programming_89.png" width="66" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_90.png" alt="Functional_Programming_90.png" width="97" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_91.png" alt="Functional_Programming_91.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_92.png" alt="Functional_Programming_92.png" width="146" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_93.png" alt="Functional_Programming_93.png" width="23" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_94.png" alt="Functional_Programming_94.png" width="102" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_95.png" alt="Functional_Programming_95.png" width="23" height="17" style="vertical-align:middle" />
</p>

<p class="Section">
 Patterns
</p>



<p class="Text">
 We have seen one type of pattern before: <span style='font-style: italic;'>x_</span>
</p>



<p class="Text">
 The underscore will match any expression, and then the result will be called <span style='font-style: italic;'>x</span>
</p>



<p class="Text">
 We can test if a pattern matches an expression using MatchQ
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_96.png" alt="Functional_Programming_96.png" width="100" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_97.png" alt="Functional_Programming_97.png" width="31" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_98.png" alt="Functional_Programming_98.png" width="374" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_99.png" alt="Functional_Programming_99.png" width="31" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 There are other kinds of patterns.
</p>



<p class="Text">
 Except will match anything except what&rsquo;s in the brackets
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_100.png" alt="Functional_Programming_100.png" width="155" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_101.png" alt="Functional_Programming_101.png" width="31" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_102.png" alt="Functional_Programming_102.png" width="155" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_103.png" alt="Functional_Programming_103.png" width="39" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 You can match for specific <span style='font-weight: bold;'>heads</span> of expressions with _h
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_104.png" alt="Functional_Programming_104.png" width="154" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_105.png" alt="Functional_Programming_105.png" width="31" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_106.png" alt="Functional_Programming_106.png" width="174" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_107.png" alt="Functional_Programming_107.png" width="39" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Conditions can be added to a pattern with /;
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_108.png" alt="Functional_Programming_108.png" width="181" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_109.png" alt="Functional_Programming_109.png" width="31" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_110.png" alt="Functional_Programming_110.png" width="157" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_111.png" alt="Functional_Programming_111.png" width="39" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Boolean functions can also be added with the ? operator
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_112.png" alt="Functional_Programming_112.png" width="151" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_113.png" alt="Functional_Programming_113.png" width="31" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_114.png" alt="Functional_Programming_114.png" width="151" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_115.png" alt="Functional_Programming_115.png" width="39" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Patterns can be combined using | for or
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_116.png" alt="Functional_Programming_116.png" width="165" height="19" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_117.png" alt="Functional_Programming_117.png" width="31" height="17" style="vertical-align:middle" />
</p>

<p class="Section">
 Type checking
</p>



<p class="Text">
 Checking for specific heads allows us to perform type checking
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_118.gif" alt="Functional_Programming_118.gif" width="455" height="81" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_119.png" alt="Functional_Programming_119.png" width="117" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_120.png" alt="Functional_Programming_120.png" width="552" height="60" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_121.png" alt="Functional_Programming_121.png" width="47" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_122.png" alt="Functional_Programming_122.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_123.png" alt="Functional_Programming_123.png" width="67" height="17" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_124.png" alt="Functional_Programming_124.png" width="287" height="16" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_125.png" alt="Functional_Programming_125.png" width="56" height="17" style="vertical-align:middle" />
</p>

<p class="Message">
 <img src="HTMLFiles/Functional_Programming_126.png" alt="Functional_Programming_126.png" width="486" height="16" style="vertical-align:middle;" usemap="#map_126" />
<map name="map_126">
<area shape="rect" coords="0,15,20,1" title="Dynamic[RawBoxes[FEPrivate`FrontEndResource[FEStrings, messageMenuTooltip]]]" nohref="" />
</map>
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_127.png" alt="Functional_Programming_127.png" width="217" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Let&rsquo;s get rid of our old (overly-general) rule
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_128.png" alt="Functional_Programming_128.png" width="129" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 We want to add a condition to the pattern: only match non-negative integers
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_129.gif" alt="Functional_Programming_129.gif" width="556" height="39" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_130.png" alt="Functional_Programming_130.png" width="56" height="17" style="vertical-align:middle" />
</p>

<p class="Print">
 <img src="HTMLFiles/Functional_Programming_131.png" alt="Functional_Programming_131.png" width="381" height="16" style="vertical-align:middle" />
</p>

<p class="Text">
 <span style='font-weight: bold;'>Another example</span>
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_132.gif" alt="Functional_Programming_132.gif" width="154" height="39" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_133.png" alt="Functional_Programming_133.png" width="55" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_134.png" alt="Functional_Programming_134.png" width="16" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_135.png" alt="Functional_Programming_135.png" width="64" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_136.png" alt="Functional_Programming_136.png" width="16" height="17" style="vertical-align:middle" />
</p>

<p class="Section">
 Example: defining our own derivative function
</p>



<p class="Text">
 We want to differentiate arbitrary expressions
</p>



<p class="Text">
 This can be achieved using the basic rules of differentiation:
</p>



<p class="Item">
 Linearity
</p>



<p class="Item">
 Product rule
</p>



<p class="Item">
 Chain rule
</p>



<p class="Text">
 We first need the concept of an expression being independent of another expression.<br />This is achieved using FreeQ
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_137.png" alt="Functional_Programming_137.png" width="91" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_138.png" alt="Functional_Programming_138.png" width="31" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_139.png" alt="Functional_Programming_139.png" width="104" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_140.png" alt="Functional_Programming_140.png" width="31" height="17" style="vertical-align:middle" />
</p>

<p class="Item">
 Some common base cases:
</p>



<p class='Input' style='border-left: 0px;border-right: 0px;border-top: 0px;border-bottom: 2px;border-style: solid;border-color: #000000;'>
 <img src="HTMLFiles/Functional_Programming_141.gif" alt="Functional_Programming_141.gif" width="234" height="39" style="vertical-align:middle" />
</p>

<p class="Item">
 Addition:
</p>



<p class='Input' style='border-left: 0px;border-right: 0px;border-top: 0px;border-bottom: 2px;border-style: solid;border-color: #000000;'>
 <img src="HTMLFiles/Functional_Programming_142.png" alt="Functional_Programming_142.png" width="317" height="17" style="vertical-align:middle" />
</p>

<p class="Item">
 Scalar multiplication:
</p>



<p class='Input' style='border-left: 0px;border-right: 0px;border-top: 0px;border-bottom: 2px;border-style: solid;border-color: #000000;'>
 <img src="HTMLFiles/Functional_Programming_143.png" alt="Functional_Programming_143.png" width="354" height="17" style="vertical-align:middle" />
</p>

<p class="Item">
 Product rule
</p>



<p class='Input' style='border-left: 0px;border-right: 0px;border-top: 0px;border-bottom: 2px;border-style: solid;border-color: #000000;'>
 <img src="HTMLFiles/Functional_Programming_144.png" alt="Functional_Programming_144.png" width="358" height="17" style="vertical-align:middle" />
</p>

<p class="Item">
 Chain rule
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_145.png" alt="Functional_Programming_145.png" width="471" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 (Have to be careful in the above not to match f[x] (so make sure g doesn&rsquo;t match x), otherwise have infinite recursion)
</p>



<p class='Input' style='border-left: 0px;border-right: 0px;border-top: 0px;border-bottom: 2px;border-style: solid;border-color: #000000;'>
 <img src="HTMLFiles/Functional_Programming_146.png" alt="Functional_Programming_146.png" width="435" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_147.png" alt="Functional_Programming_147.png" width="168" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_148.png" alt="Functional_Programming_148.png" width="55" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_149.png" alt="Functional_Programming_149.png" width="99" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_150.png" alt="Functional_Programming_150.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_151.png" alt="Functional_Programming_151.png" width="76" height="17" style="vertical-align:middle" />
</p>

<p class="Message">
 <img src="HTMLFiles/Functional_Programming_152.png" alt="Functional_Programming_152.png" width="310" height="16" style="vertical-align:middle;" usemap="#map_152" />
<map name="map_152">
<area shape="rect" coords="0,15,20,1" title="Dynamic[RawBoxes[FEPrivate`FrontEndResource[FEStrings, messageMenuTooltip]]]" nohref="" />
</map>
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_153.png" alt="Functional_Programming_153.png" width="110" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 If we encounter functions whose derivatives we don&rsquo;t know, it will leave them unevaluated:
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_154.png" alt="Functional_Programming_154.png" width="165" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_155.png" alt="Functional_Programming_155.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_156.png" alt="Functional_Programming_156.png" width="122" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_157.png" alt="Functional_Programming_157.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 We can easily add rules for trigonometric functions:
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_158.gif" alt="Functional_Programming_158.gif" width="212" height="39" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_159.png" alt="Functional_Programming_159.png" width="122" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_160.png" alt="Functional_Programming_160.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_161.png" alt="Functional_Programming_161.png" width="165" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_162.png" alt="Functional_Programming_162.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Our definitions will automatically work with function composition:
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_163.png" alt="Functional_Programming_163.png" width="179" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_164.png" alt="Functional_Programming_164.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_165.png" alt="Functional_Programming_165.png" width="234" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_166.png" alt="Functional_Programming_166.png" width="690" height="66" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_167.png" alt="Functional_Programming_167.png" width="156" height="20" style="vertical-align:middle" />
</p>

<p class="Message">
 <img src="HTMLFiles/Functional_Programming_168.png" alt="Functional_Programming_168.png" width="310" height="16" style="vertical-align:middle;" usemap="#map_168" />
<map name="map_168">
<area shape="rect" coords="0,15,20,1" title="Dynamic[RawBoxes[FEPrivate`FrontEndResource[FEStrings, messageMenuTooltip]]]" nohref="" />
</map>
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_169.png" alt="Functional_Programming_169.png" width="117" height="17" style="vertical-align:middle" />
</p>

<p class="Section">
 Speed: memoization
</p>



<p class="Text">
 Recall our Fibonacci sequence
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_170.gif" alt="Functional_Programming_170.gif" width="233" height="60" style="vertical-align:middle" />
</p>

<p class="Text">
 How fast (slow?) is it?
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_171.png" alt="Functional_Programming_171.png" width="118" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_172.png" alt="Functional_Programming_172.png" width="122" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_173.png" alt="Functional_Programming_173.png" width="118" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_174.png" alt="Functional_Programming_174.png" width="132" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_175.png" alt="Functional_Programming_175.png" width="118" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_176.png" alt="Functional_Programming_176.png" width="125" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_177.png" alt="Functional_Programming_177.png" width="347" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_178.png" alt="Functional_Programming_178.png" width="604" height="85" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_179.png" alt="Functional_Programming_179.png" width="450" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_180.gif" alt="Functional_Programming_180.gif" width="360" height="226" style="vertical-align:middle" />
</p>

<p class="Text">
 In fact, the runtime for the recursive algorithm satisfies
</p>



<p class="Text">
 <span><span><img src="HTMLFiles/Functional_Programming_181.png" alt="Functional_Programming_181.png" width="688" height="19" style="vertical-align:middle" /></span></span>
</p>



<p class="Text">
 and so the time to compute fib[n] is actually given by fib[n]
</p>



<p class="Text">
 We can easily find a closed form representation of the Fibonacci sequence (involving the golden ratio) using e.g. the characteristic polynomial
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_182.png" alt="Functional_Programming_182.png" width="444" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_183.png" alt="Functional_Programming_183.png" width="191" height="49" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_184.png" alt="Functional_Programming_184.png" width="284" height="20" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_185.png" alt="Functional_Programming_185.png" width="511" height="43" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_186.gif" alt="Functional_Programming_186.gif" width="360" height="222" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_187.png" alt="Functional_Programming_187.png" width="232" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_188.gif" alt="Functional_Programming_188.gif" width="360" height="226" style="vertical-align:middle" />
</p>

<p class="Text">
 We can try to optimize our recursive implementation using <span style='font-weight: bold;'>memoization</span>
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_189.png" alt="Functional_Programming_189.png" width="110" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_190.png" alt="Functional_Programming_190.png" width="717" height="2412" style="vertical-align:middle" />
</p>

<p class="Text">
 Look how many times fib[1] and fib[0] are evaluated! We can speed things up by <span style='font-weight: bold;'>storing</span> these values
</p>



<p class="Input">
 <img src="HTMLFiles/Functional_Programming_191.png" alt="Functional_Programming_191.png" width="297" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_192.png" alt="Functional_Programming_192.png" width="110" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_193.png" alt="Functional_Programming_193.png" width="717" height="2412" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_194.png" alt="Functional_Programming_194.png" width="110" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_195.png" alt="Functional_Programming_195.png" width="429" height="76" style="vertical-align:middle;" usemap="#map_195" />
<map name="map_195">
<area shape="rect" coords="13,66,72,56" title="Dynamic[FEPrivate`FrontEndResource[FEStrings, sizeExplanation]]" nohref="" />
</map>
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_196.png" alt="Functional_Programming_196.png" width="110" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_197.png" alt="Functional_Programming_197.png" width="717" height="2412" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_198.png" alt="Functional_Programming_198.png" width="390" height="102" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_199.png" alt="Functional_Programming_199.png" width="386" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_200.png" alt="Functional_Programming_200.png" width="604" height="81" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_201.png" alt="Functional_Programming_201.png" width="620" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_202.gif" alt="Functional_Programming_202.gif" width="360" height="212" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_203.png" alt="Functional_Programming_203.png" width="224" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_204.gif" alt="Functional_Programming_204.gif" width="360" height="226" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Functional_Programming_205.gif" alt="Functional_Programming_205.gif" width="440" height="39" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Functional_Programming_206.gif" alt="Functional_Programming_206.gif" width="360" height="217" style="vertical-align:middle" />
</p>

<p class="Text">
 We can see that the timings are linear, which is clear given the recurrence
</p>



<p class="Text">
 <span><span><img src="HTMLFiles/Functional_Programming_207.png" alt="Functional_Programming_207.png" width="688" height="19" style="vertical-align:middle" /></span></span>
</p>






<div style="font-family:Helvetica; font-size:11px; width:100%; border:1px none #999999; border-top-style:solid; padding-top:2px; margin-top:20px;">
 <a href="http://www.wolfram.com/language/" style="color:#000; text-decoration:none;">
  <span style="color:#555555">Created with the Wolfram Language</span> 
 </a>
</div>
</body>

</html>
