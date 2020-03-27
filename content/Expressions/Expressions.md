<!-- Created with the Wolfram Language for Students - Personal Use Only : www.wolfram.com -->

<html xmlns="http://www.w3.org/1999/xhtml">
<head>
 <title>
  Expressions (the Wolfram Language for Students - Personal Use Only : www.wolfram.com)
 </title>
 <link href="HTMLFiles/Expressions.css" rel="stylesheet" type="text/css" />
  <style>
 .Input {
  border-style: inset;
}
 </style>
</head>

<body>

<p class="Section">
 What exactly are expressions?
</p>



<p class="Text">
 Expressions are built by <span style='font-weight: bold;'>combining more basic</span> expressions into more complicated expressions
</p>



<p class="Text">
 e.g.
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_1.png" alt="Expressions_1.png" width="30" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_2.png" alt="Expressions_2.png" width="30" height="17" style="vertical-align:middle" />
</p>

<p class='Text' style='font-style: italic;'>
 <span style='font-style: normal;'>can be thought of as being made up of expressions for </span>a<span style='font-style: normal;'>, </span>b<span style='font-style: normal;'>, and +</span>
</p>



<p class="Text">
 So a complicated expression can be broken down into simpler expressions
</p>



<p class="Text">
 At a certain point, we obtain simple, <span style='font-weight: bold;'>irreducible</span> expressions that cannot be broken down anymore
</p>



<p class="Text">
 These irreducible expressions are called <span style='font-weight: bold;'>atoms</span>
</p>



<p class="Text">
 There are three main kinds of atoms:
</p>



<p class="Item">
 Numbers
</p>



<p class="Item">
 Strings
</p>



<p class="Item">
 Symbols
</p>



<p class="Text">
 We have seen many examples of numbers: these can be integers or inexact (floating point) numbers
</p>



<p class="Text">
 Strings are more-or-less self-explanatory:
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_3.png" alt="Expressions_3.png" width="142" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_4.png" alt="Expressions_4.png" width="126" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 <span style='font-weight: bold;'>Symbols</span> are what distinguish Mathematica from other kinds of languages
</p>



<p class="Text">
 In the example above, <span style='font-style: italic;'>a</span> and <span style='font-style: italic;'>b</span> are symbols
</p>



<p class="Text">
 The + sign is also a notation for the Plus symbol
</p>



<p class="Text">
 We can decompose an expression into its atoms using FullForm
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_5.png" alt="Expressions_5.png" width="108" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_6.png" alt="Expressions_6.png" width="76" height="17" style="vertical-align:middle" />
</p>

<p class="Section">
 Variables and expressions
</p>



<p class="Text">
 Here we begin to see what makes Mathematica different
</p>



<p class="Text">
 <span style='font-weight: bold;'>Unlike in Julia,</span> variables may be used <span style='font-weight: bold;'>before</span> they are assigned a value
</p>



<p class="Text">
 Mathematica will manipulate the expression with variables held in an unevaluated form
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_7.gif" alt="Expressions_7.gif" width="613" height="409" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_8.gif" alt="Expressions_8.gif" width="613" height="409" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_9.png" alt="Expressions_9.png" width="30" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_10.png" alt="Expressions_10.png" width="19" height="17" style="vertical-align:middle" />
</p>

<p class="Section">
 Mathematical expressions
</p>



<p class="Text">
 Using variables in this way lets us manipulate mathematical objects such as equations and polynomials
</p>



<p class="Text">
 <span style='font-weight: bold;'>Note: </span>using some shortcuts, you can use &ldquo;fancy&rdquo; notation in input cells (e.g. superscripts for powers, fractions for division, etc.)
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_11.png" alt="Expressions_11.png" width="112" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_12.png" alt="Expressions_12.png" width="81" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_13.png" alt="Expressions_13.png" width="81" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_14.png" alt="Expressions_14.png" width="81" height="17" style="vertical-align:middle" />
</p>

<p class="Section">
 Creating and assigning variables
</p>



<p class="Text">
 Variables are assigned using the equal sign = (Set)
</p>



<p class="Text">
 lhs = rhs
</p>



<p class="Text">
 will evaluate the expression &lsquo;rhs&rsquo; and assign the result to &lsquo;lhs&rsquo;. The right-hand side can be any Mathematica expression
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_15.png" alt="Expressions_15.png" width="47" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_16.png" alt="Expressions_16.png" width="15" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_17.png" alt="Expressions_17.png" width="32" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_18.png" alt="Expressions_18.png" width="47" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_19.png" alt="Expressions_19.png" width="48" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_20.png" alt="Expressions_20.png" width="55" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Variables can be unset using Clear
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_21.png" alt="Expressions_21.png" width="63" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_22.png" alt="Expressions_22.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_23.png" alt="Expressions_23.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Section">
 Brackets
</p>



<p class="Text">
 There are four kinds of bracketing in Mathematica:
</p>



<p class="Item">
 (Parentheses) for grouping mathematical expressions
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_24.png" alt="Expressions_24.png" width="50" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_25.png" alt="Expressions_25.png" width="16" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_26.png" alt="Expressions_26.png" width="66" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_27.png" alt="Expressions_27.png" width="16" height="17" style="vertical-align:middle" />
</p>

<p class="Item">
 [Square brackets] for functions calls
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_28.png" alt="Expressions_28.png" width="55" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_29.png" alt="Expressions_29.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Item">
 {Braces} for lists
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_30.png" alt="Expressions_30.png" width="66" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_31.png" alt="Expressions_31.png" width="66" height="17" style="vertical-align:middle" />
</p>

<p class="Item">
 [[Double brackets]] for indexing
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_32.png" alt="Expressions_32.png" width="106" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_33.png" alt="Expressions_33.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Section">
 Algebraic manipulation and simplification
</p>



<p class="Text">
 This is one of the most powerful features of Mathematica
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_34.png" alt="Expressions_34.png" width="133" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_35.png" alt="Expressions_35.png" width="53" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_36.png" alt="Expressions_36.png" width="149" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_37.png" alt="Expressions_37.png" width="710" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 In particular, <span style='font-weight: bold;'>Simplify</span> is one of the most useful single functions
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_38.png" alt="Expressions_38.png" width="200" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_39.png" alt="Expressions_39.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Sometimes <span style='font-weight: bold;'>FullSimplify</span> can simplify more complicated expressions (using an expanded set of rules)
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_40.png" alt="Expressions_40.png" width="229" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_41.png" alt="Expressions_41.png" width="151" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_42.png" alt="Expressions_42.png" width="261" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_43.png" alt="Expressions_43.png" width="69" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_44.png" alt="Expressions_44.png" width="321" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_45.png" alt="Expressions_45.png" width="116" height="40" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_46.png" alt="Expressions_46.png" width="102" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_47.png" alt="Expressions_47.png" width="250" height="37" style="vertical-align:middle" />
</p>

<p class="Text">
 The percent symbol can be used as a shortcut for the output of the last expression
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_48.png" alt="Expressions_48.png" width="86" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_49.png" alt="Expressions_49.png" width="116" height="40" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_50.png" alt="Expressions_50.png" width="71" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_51.png" alt="Expressions_51.png" width="116" height="40" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_52.png" alt="Expressions_52.png" width="94" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_53.png" alt="Expressions_53.png" width="373" height="38" style="vertical-align:middle" />
</p>

<p class="Section">
 Substitution rules
</p>



<p class="Text">
 Given an expression such as:
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_54.png" alt="Expressions_54.png" width="175" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_55.png" alt="Expressions_55.png" width="81" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 We can evaluate this expression with the variables replaced by numbers (or <span style='font-weight: bold;'>any</span> other expressions) using <span style='font-weight: bold;'>substitution rules</span>
</p>



<p class="Text">
 The <span style='font-weight: bold;'>replacement operator</span> is typed slash-dot, and rules are typed -&gt;
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_56.png" alt="Expressions_56.png" width="104" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_57.png" alt="Expressions_57.png" width="74" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Multiple substitutions can be made at once using lists of rules
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_58.png" alt="Expressions_58.png" width="258" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_59.png" alt="Expressions_59.png" width="16" height="17" style="vertical-align:middle" />
</p>

<p class="Section">
 More algebraic manipulations
</p>



<p class="Text">
 Simplify tends not to make assumptions about the variables
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_60.png" alt="Expressions_60.png" width="140" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_61.png" alt="Expressions_61.png" width="30" height="19" style="vertical-align:middle" />
</p>

<p class="Text">
 Assumptions can be provided as a second argument to Simplify:
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_62.png" alt="Expressions_62.png" width="185" height="20" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_63.png" alt="Expressions_63.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Algebraic expressions can be analyzed programmatically:
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_64.png" alt="Expressions_64.png" width="256" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_65.png" alt="Expressions_65.png" width="228" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_66.png" alt="Expressions_66.png" width="170" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_67.png" alt="Expressions_67.png" width="56" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_68.png" alt="Expressions_68.png" width="146" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_69.png" alt="Expressions_69.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_70.png" alt="Expressions_70.png" width="71" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_71.png" alt="Expressions_71.png" width="26" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_72.png" alt="Expressions_72.png" width="155" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_73.png" alt="Expressions_73.png" width="62" height="36" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_74.png" alt="Expressions_74.png" width="94" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_75.png" alt="Expressions_75.png" width="30" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_76.png" alt="Expressions_76.png" width="110" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_77.png" alt="Expressions_77.png" width="57" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_78.png" alt="Expressions_78.png" width="27" height="17" style="vertical-align:middle" />
</p>

<p class="Section">
 Example: binomial theorem
</p>



<p class="Text">
 Recall the binomial theorem:
</p>



<p class="Text">
 <span><span><img src="HTMLFiles/Expressions_79.png" alt="Expressions_79.png" width="688" height="38" style="vertical-align:middle" /></span></span>
</p>



<p class="Text">
 Mathematica immediately simplifies using this identity:
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_80.png" alt="Expressions_80.png" width="328" height="21" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_81.png" alt="Expressions_81.png" width="53" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 We can evaluate for a specific n using a replacement rule
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_82.png" alt="Expressions_82.png" width="104" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_83.png" alt="Expressions_83.png" width="58" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_84.png" alt="Expressions_84.png" width="79" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_85.png" alt="Expressions_85.png" width="669" height="17" style="vertical-align:middle" />
</p>

<p class="Section">
 Equations
</p>



<p class="Text">
 Just like in Julia, equality is tested with ==
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_86.png" alt="Expressions_86.png" width="32" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_87.png" alt="Expressions_87.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_88.png" alt="Expressions_88.png" width="34" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_89.png" alt="Expressions_89.png" width="39" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_90.png" alt="Expressions_90.png" width="34" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_91.png" alt="Expressions_91.png" width="31" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_92.png" alt="Expressions_92.png" width="63" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Equations are themselves Mathematica expressions
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_93.png" alt="Expressions_93.png" width="162" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_94.png" alt="Expressions_94.png" width="107" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 Equations can be solved using Solve
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_95.png" alt="Expressions_95.png" width="115" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_96.png" alt="Expressions_96.png" width="330" height="39" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_97.png" alt="Expressions_97.png" width="185" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_98.png" alt="Expressions_98.png" width="240" height="21" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_99.png" alt="Expressions_99.png" width="32" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_100.png" alt="Expressions_100.png" width="230" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 NSolve (for &ldquo;numeric solve&rdquo;) will look for numeric rather than symbolic solutions
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_101.png" alt="Expressions_101.png" width="193" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_102.png" alt="Expressions_102.png" width="230" height="17" style="vertical-align:middle" />
</p>

<p class="Text">
 For linear, quadratic, cubic, and quartic polynomials, Mathematica will always give a closed-form solution
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_103.png" alt="Expressions_103.png" width="205" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_104.png" alt="Expressions_104.png" width="681" height="36" style="vertical-align:middle" />
</p>

<p class="Text">
 Some equations do not admit closed-form solutions
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_105.png" alt="Expressions_105.png" width="185" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_106.png" alt="Expressions_106.png" width="664" height="43" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_107.png" alt="Expressions_107.png" width="193" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_108.png" alt="Expressions_108.png" width="426" height="39" style="vertical-align:middle" />
</p>

<p class="Text">
 You can also solve for simultaneous systems of equations
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_109.png" alt="Expressions_109.png" width="325" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_110.png" alt="Expressions_110.png" width="250" height="35" style="vertical-align:middle" />
</p>

<p class="Section">
 Set and SetDelayed
</p>



<p class="Text">
 Up until now, we have assigned expressions to variables using =, which is called Set
</p>



<p class="Text">
 Whenever we write lhs = rhs, the rhs is evaluated immediately
</p>



<p class="Text">
 Sometimes we don&rsquo;t want to evaluate the rhs immediately. Instead, we want to wait until we encounter lhs somewhere else in our program. When we encounter lhs, it is replaced by rhs and <span style='font-weight: bold;'>only then</span> evaluated
</p>



<p class="Text">
 This is denoted SetDelayed, and is written :=
</p>



<p class="Text">
 <span style='font-weight: bold;'>For example, </span>we will use <span style='font-weight: bold;'>Set</span> for x, and <span style='font-weight: bold;'>SetDelayed</span> for y
</p>



<p class="Input">
 <img src="HTMLFiles/Expressions_111.gif" alt="Expressions_111.gif" width="95" height="39" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_112.png" alt="Expressions_112.png" width="62" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_113.png" alt="Expressions_113.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_114.png" alt="Expressions_114.png" width="62" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_115.png" alt="Expressions_115.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_116.png" alt="Expressions_116.png" width="62" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_117.png" alt="Expressions_117.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_118.png" alt="Expressions_118.png" width="62" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_119.png" alt="Expressions_119.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_120.png" alt="Expressions_120.png" width="62" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_121.png" alt="Expressions_121.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_122.png" alt="Expressions_122.png" width="62" height="17" style="vertical-align:middle" />
</p>

<p class="Input">
 <img src="HTMLFiles/Expressions_123.png" alt="Expressions_123.png" width="8" height="17" style="vertical-align:middle" />
</p>

<p class="Output">
 <img src="HTMLFiles/Expressions_124.png" alt="Expressions_124.png" width="70" height="17" style="vertical-align:middle" />
</p>




<div style="font-family:Helvetica; font-size:11px; width:100%; border:1px none #999999; border-top-style:solid; padding-top:2px; margin-top:20px;">
 <a href="http://www.wolfram.com/language/" style="color:#000; text-decoration:none;">
  <span style="color:#555555">Created with the Wolfram Language</span> 
 </a>
</div>
</body>

</html>
