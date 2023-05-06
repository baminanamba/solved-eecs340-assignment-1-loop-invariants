Download Link: https://assignmentchef.com/product/solved-eecs340-assignment-1-loop-invariants
<br>
Assignment 1: Loop Invariants

The greatest common divisor (GCD) of two integers <em>a </em>and <em>b </em>is defined as the largest integer that can divide both <em>a </em>and <em>b </em>without a remainder. For example, the GCD of 30 and 54 is 6, whereas the GCD of 7 and 5 is 1. The following procedure was developed by Euclid to compute the greatest common divisor of two positive integers <em>a </em>and <em>b</em>. In this exercise, we will prove the correctness of this algorithm.

<strong>procedure </strong>Euclidean(<em>a</em>, <em>b</em>)

<ul>

 <li><em>x </em>← <em>a</em></li>

 <li><em>y </em>← <em>b</em></li>

 <li><strong>while </strong><em>x </em>6= <em>y </em><strong>do</strong></li>

 <li><strong>if </strong><em>x &gt; y </em><strong>then</strong></li>

 <li><em>x </em>← <em>x</em>−<em>y</em></li>

 <li><strong>else</strong></li>

 <li><em>y </em>← <em>y </em>−<em>x</em></li>

 <li><strong>return </strong><em>x</em></li>

 <li>State the loop invariant for the while loop in this procedure.</li>

 <li>Prove the loop invariant.</li>

 <li>Prove that procedure Euclidean always terminates provided that <em>a </em>and <em>b </em>are positive integers.</li>

 <li>Using the termination property of your loop invariant, prove that procedure Euclidean computes and returns the greatest common divisor of <em>a </em>and <em>b</em>.</li>

</ul>

<h1>Problem 2</h1>

Let <em>A </em>and <em>B </em>be two arrays, each consisting of <em>n </em>numbers sorted in increasing order. We are also given a number <em>x </em>and would like to find and return <em>i </em>and <em>j </em>such that <em>A</em>[<em>i</em>] + <em>B</em>[<em>j</em>] = <em>x</em>. If no such pair exists, we would like to return FALSE. We would like to develop an algorithm to solve this problem in linear time.

<ul>

 <li>Using pseudo-code, describe an algorithm that correctly solves this problem in linear time.</li>

 <li>Explain graphically how your algorithm works.</li>

 <li>Using loop invariants, prove that your algorithm is correct.</li>

 <li>Show that the worst-case runtime of your algorithm is Θ(<em>n</em>).</li>

</ul>

<h1>Problem 3</h1>

Two species are sharing planet Kepler-442b: Pisidians and Lydians. Members of either species roam individually. They can run into each other only in pairs (randomly) and whenever any two individuals run into each other, they fight. Since Pisidians are stronger and Lydians have magical powers, the outcome of a fight is always the same:

<ul>

 <li>If two Lydians fight, one of the Lydians dies and the other survives.</li>

 <li>If two Pisidians fight, both Pisidians die and a new Lydian comes to existence.</li>

 <li>If a Pisidian and a Lydian fight, the Lydian dies and the Pisidian survives.</li>

</ul>

At the beginning of time, there were <em>m </em>Lydians and <em>n </em>Pisidians on Kepler-442b. Observing that there will be only one individual left on Kepler-442b at eternity, identify the species of the eternal individual as a function of <em>m </em>and/or <em>n</em>. (<em>Hint: </em>Describe the process using a loop and define a loop invariant.)