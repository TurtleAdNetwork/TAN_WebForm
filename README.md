<h1 align="center">
  <img src="https://www.turtleadnetwork.com/images/turtleadnetwork_logo.png" alt="TAN" width="200"/>
</h1>

# Turtle Ad Network - Web Form
Web Form for submitting Ads, utilizes the TurtleShell web extension, for Paying &amp; Sending the Advert.<br>

**Visit:** https://www.turtleadnetwork.com/ad/ <br>
**Plugin:** https://wordpress.org/plugins/turtle-ad-network <br>
**Note:** TurtleShell web extension will be required to Pay & Send the Ad. <a href="https://addons.mozilla.org/en-US/firefox/addon/turtleshell/">Download: TurtleShell on FireFox.</a>

**formsubmission.html:** Front-end html code, to create the form view.<br>
**process.js:** Javascript that does all the magic. Please make sure to insert 'process.js' in the same directory as the frontend html.<br>
**Inserting multiple websites:** Simply edit 'process.js' and include the details, as below, each new entry please increase the index value.

```
$(document).ready(function () {
    let websites = [{
        index: 0,
        website: 'TurtleNetwork.eu',
        address: '3Jqn2aKeYn59UNJue9qy9poHZH16HhZ6LFp',
        currency: 'TN',
        price: '100000000',
        assetId: 'TN',
        digits: '8',
        amountImpressions: '50'
    },
    {
        index: 1,
        website: 'RapydBlok.com',
        address: '3Jhhq39fSg6y44EDSf8xprHGWaKfdphBjbR',
        currency: 'TN',
        price: '100000000',
        assetId: 'TN',
        digits: '8',
        amountImpressions: '25'
    }
