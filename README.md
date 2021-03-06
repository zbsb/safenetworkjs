[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](https://github.com/standard/standard)

# What's This?

SafenetworkJs is a library for implementing web, desktop and command line apps for use with the SAFE Network. It aims to be a pretty comprehensive library.

## Supports:
- Web apps running in SAFE Browser
- Desktop and command line apps on Windows, Mac OS and Linux
- NodeJs including cross platform packaged CLI apps (e.g. [safe-cli-boilerplate](https://github.com/theWebalyst/safe-cli-boilerplate) and [SAFE FUSE](https://github.com/theWebalyst/safenetwork-fuse/))

## Provides APIs:
- authorisation with SAFE Network (via SAFE Browser)
- Json API for accessing files (e.g. `listFolder(), readFile(), makeFolder(), safeFile()` etc.)
- Json API for accessing public names (e.g. listing `_publicNames` their services and files)
- creation of public names and services
- access to SAFE network via RESTful interface in web, desktop and CLI applications via `fetch()`

## Status
This NodeJs library is under development but already in use in [SAFE FUSE](https://github.com/theWebalyst/safenetwork-fuse/) which mounts files, public names (DNS) and services on your local drive. SAFE FUSE is a command line application which targets Windows, Mac OS and Linux. It uses SafenetworkJs for all interactions with SAFE Network including authorisation, and access to SAFE storage via a file system API, and for access to SAFE public names (DNS) and services.

SafenetworkJs incorporates the code from a discontinuted web library: [safenetwork-web](https://github.com/theWebalyst/safenetwork-web) that added RESTful services for SAFE Network (implemented in the client) and was used to demonstrate a [Solid](https://solid.mit.edu/) web app runnning on SAFE Network (Safe Plume blog). That code needs some refactoring for the update SAFE NodeJs API (v0.9.x) but has been proven with the earlier SAFE NodeJs API (v0.8). The demonstration which used these features is documented in a video presentation which shows how a web app can access SAFE Network as if it was a RESTful web server. Presentation slides and video: [Supercharging the SAFE Network with Project Solid](https://safenetforum.org/t/devcon-talk-supercharging-the-safe-network-with-project-solid/23081?u=happybeing), (SAFE Network DevCon, April 2018, Troon Scotland).

You can use SafenetworkJs APIs directly, or to emulate RESTful interfaces which access SAFE Network from web, desktop and command line applications. Extra RESTful interfaces can be supported by adding a new class.

## About SAFE Network
The [SAFE Network](https://safenetwork.tech/) is a truly autonomous, decentralised internet. This **Secure Access For Everyone Network** (SAFE) tackles the increasing risks to individuals, business and nation states arising from over centralisation: domination by commercial monopolies, security risks from malware, hacking, surveillance and so on. It's a new and truly open internet aligned with the original vision held by its creators and early users, with security, net neutrality and unmediated open access baked in.

The following are currently all unique to the SAFE Network (2018):

- all services are secure and decentralised, including a human readable DNS
- highly censorship resistant to DDoS, deep packet inspection and nation state filters
- truly autonomous network
- data is guaranteed to be stored and available, forever with no ongoing fees (pay once to store)
- truly decentralised 'proof of resource' (farming), and not 'proof of work' or 'proof of stake'
- scalable non-blockchain based storage not just of hashes of data, but the data itself
- scalable non-blockchain cryptographically secured currency (Safecoin) with zero transaction fees

SAFE Network operates using the resources of anonymous 'farmers' who are rewarded with Safecoin, which they can sell or use to purchase storage and other services on the network. Safecoin is efficent and scalable (non-blockchain based) secure and anonymous digital cash.

SAFE is an open source project of @maidsafe, a private company which is majority owned by a Scottish charity, both based in Scotland but which is decentralised with employees and contributors based around the globe.

# Development

If you wish to develop with or improve this library, please see the instructions on set-up and debugging in the [SAFE FUSE repository](https://github.com/theWebalyst/safenetwork-fuse/#development).

Pull requests are welcome for outstanding issues and feature requests. Please note that contributions are subject to the LICENSE (see below).

**IMPORTANT:** By submitting a pull request, you will be offering code under the LICENSE (below).

## Please Use Standard.js

Before submitting your code please consider using `Standard.js` formatting. You may also find it helps to use an editor with support for Standard.js when developing and testing. An easy way is just to use [Atom IDE](https://atom.io/packages/atom-ide-ui) with the package [ide-standardjs] (and optionally [standard-formatter](https://atom.io/packages/standard-formatter)). Or you can install NodeJS [Standard.js](https://standardjs.com/).

[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/standard/standard)

# LICENSE
This project is made available under the [GPL-3.0 LICENSE](https://opensource.org/licenses/GPL-3.0) except for individual files which contain their own license so long as that file license is compatible with GPL-3.0.

The responsibility for checking this licensing is valid and that your use of this code complies lies with any person and organisation making any use of it.
