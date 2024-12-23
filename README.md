# Asterisk PBX Dial Plan

<h3>Project Overview</h3>
<p>This project contains the configuration for an Asterisk PBX system supporting both SIP and IAX2 subscribers. The setup is designed for testing and development in a virtualized environment.</p>

<h4>System Details:</h4>
<ul>
    <li><b>PBX Software:</b> AsteriskNOW</li>
    <li><b>Operating System:</b> CentOS (as a virtual machine)</li>
    <li><b>Virtualization Platform:</b> Oracle VM VirtualBox 7.0.14</li>
    <li><b>Softphones:</b>
        <ul>
            <li><b>MicroSIP:</b> Used for SIP protocol.</li>
            <li><b>ZoIPer:</b> Configured exclusively for IAX2 protocol.</li>
        </ul>
    </li>
</ul>

<h3>Subscribers</h3>
<h4>SIP Subscribers</h4>
<ul>
    <li>Phone number: <b>1331</b></li>
    <li>Phone number: <b>2331</b></li>
</ul>

<h4>IAX2 Subscribers</h4>
<ul>
    <li>Phone number: <b>3331</b></li>
    <li>Phone number: <b>4331</b></li>
</ul>

<h3>Functions</h3>
<h4>For IAX2 Phones</h4>
<ul>
    <li><b>VMAuthenticate:</b> Authenticate users based on <code>voicemail.conf</code>.</li>
    <li><b>VoiceMail:</b> Leave a voicemail message.</li>
    <li><b>VoiceMailMain:</b> Access the voicemail system.</li>
    <li><b>Authenticate:</b> Authenticate a user.</li>
</ul>

<h4>For SIP Phones</h4>
<ul>
    <li><b>SayAlpha:</b> Announce letters.</li>
    <li><b>SayDigits:</b> Announce digits.</li>
    <li><b>SayNumber:</b> Announce numbers.</li>
    <li><b>SayPhonetic:</b> Announce the phonetic representation.</li>
    <li><b>SayUnixTime:</b> Announce the date and/or time.</li>
</ul>

<h3>Configuration Files</h3>
<ul>
    <li><b>sip.conf:</b> Defines SIP subscribers with their respective phone numbers.</li>
    <li><b>iax.conf:</b> Defines IAX2 subscribers with their respective phone numbers.</li>
    <li><b>extensions.conf:</b> Implements the dial plan, linking SIP and IAX2 subscribers and enabling the described features.</li>
    <li><b>voicemail.conf:</b> Configures voicemail settings for the IAX2 subscribers.</li>
</ul>
