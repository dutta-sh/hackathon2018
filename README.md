# hackathon2018

#Steps to setup the Atlassian SDK:
https://developer.atlassian.com/server/framework/atlassian-sdk/set-up-the-atlassian-plugin-sdk-and-build-a-project/
Note that this comes with a packaged maven, and uses that by default when you invoke the atlas-run command.
You can override that with command line parameters though.

#You can start from scratch to create your own plugin
https://developer.atlassian.com/server/framework/atlassian-sdk/create-a-helloworld-plugin-project/

#OR Download the sample plugin:
https://developer.atlassian.com/server/bitbucket/tutorials-and-examples/pull-request-overview/
Extract the code on your local machine. Its mavenized and I prefer to use Intellij to open it up.
Feel free to use your preferred IDE.

#Bring up the bitbucket server by running atlas-run from the command line.
Make sure to navigate into the root of the project (where the pom.xml exists) before running this.

#It will take some time for the server to come up every time you do a restart (even more for the first time while it downloads from nexus)

#Every time you make a change to the plugin xml file, avoid restarting the server.
Do this by opening another command line and type in atlas-cli
Wait for the maven> prompt to show up and then type in pi

#You can find a sample of how a new tab could be added (bitbucket.pull-request.nav) and how that could be linked to a servlet here:
https://bitbucket.org/atlassian/bitbucket-example-plugin/src/a55cffe7744e8f50abcd2f092243b4f7e1d855b1/src/main/resources/atlassian-plugin.xml?at=master&fileviewer=file-view-default

Thanks to everyone (AN, AT, CC, TS, RX and YI) for making this work !!