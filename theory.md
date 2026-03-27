### Gray Code:
The Gray code is unweighted code. Gray code exhibits only a single bit change from one code word to the next in sequence. Due to this specific feature Gray code is important in applications such as shaft position encoders, where error susceptibility increases with the number of bit changes between adjacent numbers in a sequence.

<br/>

#### Let us design a 3-bit Gray to Binary code converter and implement using IC-74LS138.

#### The relation between these two codes can be understood from the following diagram and equations:


<center> 
<img src="./images/image0018.png">
<br/>

#### Fig. 1. Gray Code to Binary Conversion
<br/>

<img src="./images/image0023.png">
</center>

<p >From the truth table it is observed that the output B2 is HIGH for minterms m<sub>4</sub>, m<sub>5</sub>, m<sub>6</sub> and m<sub>7</sub>. Hence equation defining B2 output can be written as:<span> B2 = &Sigma; m (4, 5, 6, 7). The output B1 is HIGH for minterms </span><span>m<sub>2</sub> and m<sub>3</sub> m<sub>4</sub> &amp; m<sub>5</sub>. Hence equation defining B1 output can be written as:</span><span> B1 = &Sigma; m (2, 3, 4, 5). The output B0 is HIGH for minterms&nbsp; </span><span>m<sub>1, </sub>m<sub>2</sub>&nbsp; m<sub>4 </sub>m<sub>7</sub>. Hence equation defining B0 output can be written as:</span><span><span> B0 = &Sigma; m (1, 2, 4, 7). The Binary outputs for given 3 bit Gray code are summarized as follows:</span></span></p>

<p><span><span >B2 = &Sigma; m (4, 5, 6, 7)</span></span></p>

<p >B1 = &Sigma; m (2, 3, 4, 5)</p>

<span>B0 = &Sigma; m (1, 2, 4, 7)</span>

<p >These equations can be implemented by using IC74LS138 as a 3:8 decoder as shown in Fig.2. Every Binary output has 4-minterms each. Hence IC74LS20- four input NAND gate ICs are required to produce the final Binary equivalent.</p>




<center>
<img src="./images/image0019.png">
<br/>
<span>Fig.2. Implementation of Gray code to Binary Converter using IC 74LS138 Decoder</span><br/>
</center>
<b>Note:</b> The outputs of IC 74138 are active low.

<p><span>The logic diagram, connection diagram and function table for IC 74LS138 are given below:</span></p>

<center>
<img src="./images/image0020.png">
<br/>
<img src="./images/image0021.png">
<br/>
<img src="./images/image0022.png">
<br/>

<span >Fig.3. Logic Diagram, Connection Diagram &amp; Function Table of IC 74LS138.</span>
</center>

#### Numerical:

 <img src="./images/image001.png"><br/>  Outputs =&gt; <img src="./images/image002.png">
<br/><br/><br/>
<img src="./images/image003.png">
<br/>
<img src="./images/image004.png">
<br/>
<img src="./images/image005.png">
<br/>
<img src="./images/image006.png">
<br/>
<br/>
Ex-Or Operation Table:
<br/>


<img src="./images/image007.png">
<br/>
Truth table:
<center>
<img src="./images/image0024.png">
</center>

Examples: 
<ol>
	<li>
		Input &ldquo;011&rdquo;<br/>
		<img src="./images/image008.png">
		<br/>
		<br/><img src="./images/image009.png">
		<br/><img src="./images/image010.png">
		<br/><img src="./images/image011.png">
		<br/>Output &ldquo;010&rdquo;<br/><br/><br/>
	</li>
	<li>
		Input &ldquo;110&rdquo;<br/>
		<img src="./images/image012.png">
		<br/>
		<br/><img src="./images/image013.png">
		<br/><img src="./images/image014.png">
		<br/><img src="./images/image015.png">
		<br/>Output &ldquo;100&rdquo;<br/><br/><br/>
	</li>
	<li>
		Input &ldquo;111&rdquo;<br/>
		<img src="./images/image016.png">
		<br/>
		<br/><img src="./images/image013.png">
		<br/><img src="./images/image014.png">
		<br/><img src="./images/image017.png">
		<br/>Output &ldquo;101&rdquo;<br/><br/><br/>
	</li>
</ol>
<script type="text/javascript" id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"> </script>