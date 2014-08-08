Welcome to _OmnicoinJ_, a Java implementation of the Omnicoin protocol

Omnicoin is an experiment in the creation, implementation, and integration of a cryptocurrency with MyBB community software in mind. 
Originally created by a member of HackForums.net it's grown beyond that initial ideal and has moved into a wider realm of possibility. 
With a new launch of version 2 (OMCv2), a new team, and renewed focus Omnicoin promises to gain ground which no other crypto currency has tread.

Check out http://www.omnicoin.org/ for more info.

![alt tag](https://encrypted-tbn3.gstatic.com/images?q=tbn:ANd9GcT5cGH94w6MbLPaBojOdBAVmPM9pbqJm3LIn2gNd4tPKd1F8qbgmg)

To get started, ensure you have the latest JDK installed, and download Maven from:

  http://maven.apache.org/

Then run "mvn clean package" to compile the software. You can also run "mvn site:site" to generate a website with
useful information like JavaDocs. The outputs are under the target/ directory.

Alternatively, just import the project using your IDE. IntelliJ has Maven integration once you tell it where to
find your unzipped Maven install directory.

Now try running one of the example apps:

  cd examples
  mvn exec:java -Dexec.mainClass=com.google.bitcoin.examples.ForwardingService -Dexec.args="<insert a bitcoin address here>"

It will download the block chain and eventually print a Bitcoin address. If you send coins to it,
it will forward them on to the address you specified. Note that this example app does not use
checkpointing, so the initial chain sync will be pretty slow. You can make an app that starts up and
does the initial sync much faster by including a checkpoints file; see the documentation for
more info on this.

Now you are ready to follow the tutorial:

   https://code.google.com/p/bitcoinj/wiki/GettingStarted 


Things that still need updating:
* omnicoinj\core\src\main\java\com\google\bitcoin\core\CoinDefinition.java
* NetworkParamters.java
* Developer information in AUTHORS
* omnicoinj\core\src\main\java\com\google\bitcoin\core\Peer.java ?

Developed by MeshCollider. See AUTHORS for credits.