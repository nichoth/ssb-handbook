<h1 align="center" style="font-size: 4em;">
  <img
    alt="Hermies the hermit crab"
    src="assets/hermies.png"
    width="256"
    height="256"
  />
  <br />
  Scuttlebutt
</h1>

<h2 align="center">
  a decent(ralised) secure gossip platform
</h2>

<h4 align="center">
  sea-slang for gossip - a scuttlebutt is basically a watercooler on a ship
</h4>

## contents

* [How To Get Started](#how-to-get-started)
* [Applications](applications.md)
* [Stories](stories/index.md)
  - [Design Challenge: Avoid Centralization and Singletons](stories/design-challenge-avoid-centralization-and-singletons.md)
  - [Design Challenge: Sybil Attacks](stories/design-challenge-sybil-attacks.md)
  - [Gossiping Securely is the new Email](stories/gossiping-securely-is-the-new-email.md)
  - [Scuttlebutt Genesis](stories/scuttlebutt-genesis.md)
  - [Using Trust in Open Networks](stories/using-trust-in-open-networks.md)
* [Talks](talks.md)
* [Contributing](contributing.md)

---

* [Principles](principles.md)
* [Concepts](concepts/index.md)
  - [Identity](concepts/identity.md)
  - [Stream](concepts/stream.md)
  - [Feed](concepts/feed.md)
  - [Message](concepts/message.md)
  - [Private Message](concepts/private-message.md)
  - [Link](concepts/link.md)
  - [Gossip](concepts/gossip.md)
  - [Local](concepts/local.md)
  - [Consensus](concepts/consensus.md)
  - [Pub](concepts/pub.md)
  - [Blob](concepts/blob.md)
  - [Cap](concepts/cap.md)
* [Guides](guides/index.md)
  - [First steps with sbot, a command line tool for Scuttlebutt](guides/cli-first-steps.md)
* [Modules](modules.md)
* [FAQ](faq/index.md)
  - [Basics](faq/basics/basics.md)
    - [What is the difference between Patchwork and Scuttlebutt?](faq/basics/patchwork-vs-scuttlebutt.md)
    - [What is a pub?](faq/basics/pub.md)
    - [Should I follow multiple pubs?](faq/basics/multiple-pubs.md)
    - [What do you mean SSB works through gossip?](faq/basics/gossip.md)
    - [Where does all my data live?](faq/basics/data-live.md)
    - [What ports does Scuttlebutt use?](faq/basics/port.md)
    - [How much space will scuttlebutt take up?](faq/basics/size.md)
    - [What happens if I delete everything?](faq/basics/delete.md) 
  - [Applications](faq/applications/applications.md)
    - [How do posts work across apps?](faq/applications/patchwork-and-patchbay.md)
    - [Can I switch apps easily?](faq/applications/moving-ssb-apps.md)
    - [Can I post  from different devices?](faq/applications/multiple-devices.md)
    - [Is there a markdown guide for Patchwork?](faq/applications/patchwork-markup.md)
  - [Channels](faq/channels/channels-index.md)
    - [What are channels?](faq/channels/channels.md)
    - [Are Channels sorted in any order?](faq/channels/channel-sort.md)
    - [How do channel descriptions work?](faq/channels/channel-messages.md)
    - [How do I find a channel?](faq/channels/channel-find.md)
  - [Misc.](faq/misc/concepts.md)
    - [This seems really cool?](faq/misc/cool.md)
    - [Who wrote this FAQ?](faq/misc/faq-credits.md)
    - [How can I help?](faq/misc/help.md)
* [Glossary](glossary.md)


{% vimeo %}236358264{% endvimeo %}

## How To Get Started

The easiest way to get started is using [patchwork](https://github.com/ssbc/patchwork), a classic social networking [application](./applications.md).

![screenshot of patchwork](./assets/patchwork.jpg)

### Easy path

1. [Download an Installer](https://github.com/ssbc/patchwork/releases) for Windows, macOS and Linux
2. Get a [pub invite code](https://github.com/ssbc/scuttlebot/wiki/Pub-Servers)  
3. Use the pub invite : in Patchwork click `+ Join Pub` and paste the invite code

Step 2 is important if you want to be able to find people further than your local network - it sets you up with a robot friend on the internet which helps you find and communicate with people.
Read more about Pubs and their role [here](./concepts/pub.md).


### Build from Source

This is more technical than the easy path, mainly useful if you're interested in developing Patchwork.

On Linux you'll need some more dependencies. On Debian:

```shell
sudo apt-get install libxext-dev libxtst-dev libxkbfile-dev g++ m4 automake libtool
```

With [node (>= 4) and npm (>= 2) installed](https://github.com/creationix/nvm):

```shell
$ git clone https://github.com/ssbc/patchwork
$ cd patchwork
$ npm install
$ npm start
```

Follow steps `2.` and `3.` above to connect to the network.


## Join The Community

Check out the following channels by typing their name (with #) in the search bar:
- **#new-people**: introduce yourself
- **#faq**: first impressions, what is confusing as a new user?
- **#patchwork**: report bugs, suggestions, etc
- **#scuttlebutt**: protocol related discussion

Here are some other favourites:
- **#boats**: people living on, hacking, and bulding boats
- **#cooking-channel**: nerds sharing recipes
- **#solarpunk**: step into the future
- **#gardening**: get some gardening on with your off-grid
- **#anarchitecture**: decentralise all the things

## Code of conduct

Please note that this project is released with a [Contributor Code of Conduct](code-of-conduct.md). By participating in this project you agree to abide by its terms.

