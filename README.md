# Banking Bot

This application uses the following services:
1) Conversation Service
2) Natural Language Understanding
3) Tone Analyzer
4) discovery

# Before you begin

<li>You must have a Bluemix account, and your account must have available space for at least 1 application and 2 services. 
To register for a Bluemix account, go to https://console.ng.bluemix.net/registration/. 
Your Bluemix console shows your available space.</li>


<li> You must also have the following prerequisites installed:</li>
        1) The Node.js runtime (including the npm package manager)</br>
        2) The Cloud Foundry command-line client
        
     
# Getting the files.
Clone the bankingBot locally. In a terminal, run:

<pre> <code> $ git clone https://github.com/monicaNadyH/bankingBot</code></pre>

We’ll be using the file <a href="https://github.com/monicaNadyH/bankingBot/blob/master/data/conversation/workspaces/banking%20bot.json"><code>data/conversation/workspaces/banking bot.json</code></a>
 
# Create Watson Services with IBM Cloud

<ul>

<li><a href="https://console.ng.bluemix.net/catalog/services/conversation" rel="nofollow"><strong>Watson Conversation</strong></a></li>
<li><a href="https://console.ng.bluemix.net/catalog/services/discovery" rel="nofollow"><strong>Watson Discovery</strong></a></li>
<li><a href="https://console.ng.bluemix.net/catalog/services/tone-analyzer" rel="nofollow"><strong>Watson Tone Analyzer</strong></a></li>
<li><a href="https://console.ng.bluemix.net/catalog/services/natural-language-understanding" rel="nofollow"><strong>Watson Natural Language Understanding</strong></a></li>

</ul>


# Import the workspace JSON file.

Launch the <b>Watson Conversation tool</b> . Use the import icon button on the right
<p>
Find the local version of <a href="href="https://github.com/monicaNadyH/bankingBot/blob/master/data/conversation/workspaces/banking%20bot.json"><code>data/conversation/workspaces/banking bot.json</code></a> and select
<strong>Import</strong>. Find the <strong>Workspace ID</strong> by clicking on the context menu of the new
workspace and select <strong>View details</strong>. Save this ID for later.
</p>
   
 # Load the Discovery documents.
 
 Launch the <b>Watson Discovery tool</b>. Create a new data collection and give the data collection a unique name.
 
 Under Add data to this collection use Drag and drop your documents here or browse from computer to seed the content with the five documents in <code>data/discovery/docs</code>.
 
  # Configure credentials:
  
  The credentials for IBM Cloud services (Conversation, Discovery, Tone Analyzer and Natural Language Understanding), can be found in the Services menu in IBM Cloud, by selecting the Service Credentials option for each service
  
  Copy the env.sample to .env.<br>
  
   <code>
   $ cp env.sample .env
    </code>
  <br>
   
   Edit the .env file with the necessary settings.
   
    # Run the application
    
    1. Install Node.js runtime or NPM.
    2. Start the app by running npm install, followed by npm start.
    3. Use the chatbot at localhost:3000.


