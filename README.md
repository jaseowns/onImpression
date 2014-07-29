onImpression
============

<h1>onImpression : A  jQuery plugin to trigger a function when an element is displayed on screen</h1>

<h3>For more information, visit <a href="http://www.jaseowns.com/solutions/onimpression">http://www.jaseowns.com/solutions/onimpression</a></h3>

<h3>Created by Jason Ramsey - 7/20/2014</h3>

<div class="panel panel-default">
        <div class="panel-heading">
            <h3 class="panel-title">A simple example of how to take advantage of <b>onImpression.js</b>:</h3>
        </div> 

        <div class="panel-body" id="content">                
    
            <p>Include the jquery.onImpression.js file</p>

    <pre class="prettyprint prettyprinted"><span class="pln">
    </span><span class="com">// Javascript</span><span class="pln">
    </span><span class="pun">&lt;</span><span class="pln">script src</span><span class="pun">=</span><span class="str">"http://www.jaseowns.com/public/jquery.onimpression.js"</span><span class="pln"> </span><span class="pun">/&gt;&lt;</span><span class="pln">script</span><span class="pun">/&gt;</span><span class="pln">
    </span></pre>
            
    <p>Select the elements you want to capture impressions on:</p>

    <pre class="prettyprint prettyprinted"><span class="pln">
    </span><span class="com">// Javascript</span><span class="pln">
    $</span><span class="pun">(</span><span class="kwd">function</span><span class="pln"> </span><span class="pun">()</span><span class="pln"> </span><span class="pun">{</span><span class="pln">
        $</span><span class="pun">(</span><span class="str">"li img"</span><span class="pun">).</span><span class="pln">onImpression</span><span class="pun">({</span><span class="pln">
            offset</span><span class="pun">:</span><span class="pln"> </span><span class="pun">-</span><span class="lit">50</span><span class="pun">,</span><span class="pln">
            callback</span><span class="pun">:</span><span class="pln"> </span><span class="typ">CustomCallBack</span><span class="pun">,</span><span class="pln">
        </span><span class="pun">});</span><span class="pln">
    </span><span class="pun">});</span><span class="pln">
    </span></pre>

            <p>The logic specific to your application will go within the <b>callback</b> function you create:</p>

    <pre class="prettyprint prettyprinted"><span class="pln">
    </span><span class="com">// Javascript</span><span class="pln">
    </span><span class="kwd">function</span><span class="pln"> </span><span class="typ">CustomCallBack</span><span class="pun">()</span><span class="pln"> </span><span class="pun">{</span><span class="pln">
        </span><span class="kwd">var</span><span class="pln"> imgDisplayed </span><span class="pun">=</span><span class="pln"> </span><span class="str">"&lt;img src='"</span><span class="pln"> </span><span class="pun">+</span><span class="pln"> $</span><span class="pun">(</span><span class="kwd">this</span><span class="pun">).</span><span class="pln">attr</span><span class="pun">(</span><span class="str">"src"</span><span class="pun">)</span><span class="pln"> </span><span class="pun">+</span><span class="pln"> </span><span class="str">"' /&gt;"</span><span class="pun">;</span><span class="pln">
        $</span><span class="pun">(</span><span class="str">"#displayedImages"</span><span class="pun">).</span><span class="pln">append</span><span class="pun">(</span><span class="pln">imgDisplayed</span><span class="pun">);</span><span class="pln">
    </span><span class="pun">}</span><span class="pln">
    </span></pre>

        </div>

    </div>