<a href="/1.3/README.md">Back to the Table of Contents</a>&nbsp;&nbsp;|&nbsp;&nbsp;<a href="API_METHODS.md">Back to API Methods</a>
<h2>getMmsIds</h2>
<p><strong>Synopsis:</strong><br />
This API function returns a list of comma separated MMSIDS for that account.</p>
<div><strong>Request: XML</strong></div>
<pre>&lt;REQUEST&gt;
    &lt;ACTION&gt;getMmsIds&lt;/ACTION&gt;
    &lt;API_KEY&gt;apiKey&lt;/API_KEY&gt;
&lt;/REQUEST&gt;</pre>
<div><strong>Request: GET</strong></div>
<pre>API_URL?action=getmmsids&amp;api_key=apiKey</pre>
<div><strong>Request Parameters:</strong></div>
<pre><strong>Mandatory:</strong>
action, apikey
<strong>Optional:</strong>
--
</pre>

<strong>Response Parameters:</strong><br />
status, mmsids, Errorcode, Errorinfo

<strong>Related Errorcodes: </strong><br />
E200
<div><strong>Request Examples</strong></div>
XML:
<pre>&lt;REQUEST&gt;
    &lt;ACTION&gt;getmmsids&lt;/ACTION&gt;
    &lt;API_KEY&gt;qTFkykO9JTfahCOqJ0V2Wf5Cg1t8iWlZ&lt;/API_KEY&gt;    
&lt;/REQUEST&gt;</pre>
GET:
<pre>https://secure.sumotext.com/API/wxml/1.3/index.php?action=getmmsids&api_key=qTFkykO9JTfahCOqJ0V2Wf5Cg1t8iWlZ</pre>
<div><strong>Response Example: Success</strong></div>
<pre>&lt;RESPONSE&gt;
    &lt;STATUS&gt;Success&lt;/STATUS&gt;
    &lt;MMSIDS&gt;10011,10234,10634&lt;/MMSIDS&gt;
&lt;/RESPONSE&gt;</pre>
<div><strong>Response Example: Failure</strong></div>
<pre>&lt;RESPONSE&gt;
    &lt;STATUS&gt;Failure&lt;/STATUS&gt;
    &lt;ERRORCODE&gt;E200&lt;/ERRORCODE&gt;
    &lt;ERRORINFO&gt;No MMS Templates were created in this account.&lt;/ERRORINFO&gt;
&lt;/RESPONSE&gt;</pre>
