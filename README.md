# Beaker Starter Kit

Building smart contracts with TEAL, an assembly language, and PyTeal could be challenging and unfamiliar to beginner Algorand smart contract developers. Beaker aims to address the problem by making smart contract development both simpler and familiar to web2 developers.

This is a Beaker starter kit that covers all of the components of Beaker and a complete RSVP Application example that utilizes Beaker.

Beaker repo: <https://github.com/algorand-devrel/beaker>
Beaker Documentation: <https://algorand-devrel.github.io/beaker/html/index.html>

## How to Learn

This is a recommendation only.

1. Clone and set up your development environment (instruction below) to code what you learn by yourself.
2. Have Beaker Github repo and Beaker documentation opened while learning.
3. Try filling in blanks in files under `starter-kit` folder and make the file run. If you are stuck, refer [code examples](https://github.com/algorand-devrel/beaker/tree/master/examples) provided in the Beaker github repo or search in the Beaker doc for guidance. Recommended learning route is:
   - contract_basic/application.py
   - contract_basic/state.py
   - contract_basic/decorator.py
   - interact_basic/use_sandbox.py
   - interact_basic/use_app_client.py
4. After completing all of the files above, Try building your own RSVP Application with what you learned. Try to fail as much as possible as you will learn from making mistakes, debugging, and diving into the Beaker source code to find answers.

After completing these steps, you will be a Beaker master! :clap::clap:

Now go innovate and build your own application with Beaker :grin:

## Contents

📦**complete_code** - *Directory containing complete code for demonstration* </br>
┣ 📂**contract_basic** - *Directory containing Beaker contract components code examples* </br>
┃ ┣ 📜**application.py** - *Code example showcasing application class* </br>
┃ ┣ 📜**decorator.py** - *Code example showcasing Beaker decorators* </br>
┃ ┗ 📜**state.py** - *Code example showcasing Beaker States* </br>
┣ 📂**interact_basic** - *Directory containing Beaker deploy/call, testing components code examples* </br>
┃ ┣ 📜**use_app_client.py** - *Code example showcasing Beaker application client* </br>
┃ ┗ 📜**use_sandbox.py** - *Code example showcasing Beaker sandbox module* </br>
┗ 📂**rsvp** - *Directory containing full RSVP App code examples* </br>
┃ ┣ 📜**approval.teal** - *autogenerated RSVP TEAL approval program* </br>
┃ ┣ 📜**clear.teal** - *autogenerated RSVP TEAL clear program* </br>
┃ ┣ 📜**contract.json** - *A JSON file describing the interface of the contract to be read by SDK clients* </br>
┃ ┣ 📜**interact_rsvp.py** - *Code example showcasing how to deploy / call RSVP app using Beaker sandbox module and Application client* </br>
┃ ┗ 📜**rsvp.py** - *RSVP application built with Beaker* </br>
📦**starter_kit** - *Directory containing all of the files above but with "fill in the blank" type of files for you to learn by coding by yourself* </br>

## Development Environment

### Install Sandbox

Install the [sandbox](https://github.com/algorand/sandbox) to start a local private node and start it with the `dev` configuration.

If you're in the sandbox directory run:

```bash
./sandbox up dev
```

### Clone repository

Next, clone this repository and cd to the root directory.

### Setup Virtual Environment

Create a virtual environment inside the project directory.

```bash
python3 -m venv venv
```

Activate virtual environment.

```bash
source ./venv/bin/activate
```

requirements.txt file contains all of the required dependencies and packages. Install them in your virtual environment by running:

```bash
pip install -r requirements.txt
```

Check all dependencies and packages install in your virtual environment by running:

```bash
pip list
```
