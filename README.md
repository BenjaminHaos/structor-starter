### Structor React App Starter

# Run on Cloud9

## Run Structor on Cloud9

#### *Prerequisites:*
* An account on [Cloud9](https://c9.io/) (it's free.)

#### Step 1

Create a basic Virtual Machine. **Make sure the privacy is set to public**.

![alt text][logo]

![alt text][test](step2.jpg)

[logo]: ./docs/img/step1.jpg

[test]: ./docs/img/

#### Step 2

Just to be safe, update npm and node:

```
npm i npm -g
nvm install 6
nvm alias default 6
```

#### Step 3

Clone the ```structor-starter``` repo, install modules, and install structor,

```bash
# Clone the repo,
git clone https://github.com/ipselon/structor-starter.git

# dwitch to the cloned directory,
cd structor-starter/

# install Node modules,
npm install

# and install Structor!
npm install structor
```

#### Step 3.5

During the install, you will need to choose a directory, or simply press return,

#### Step 4

Once the above is completed, modify the ```package.json``` changing **one** line from this,

```json
(...)
  "scripts": {
    (...)
    "structor": "structor"
  },
(...)
```
to this,

```json
(...)
  "scripts": {
    (...)
    "structor": "structor -v -p 8080"
  },
(...)
```
*Note* - The ```-v``` switch is optional but the ```-p <port>``` is [needed to run on Cloud9](https://docs.c9.io/docs/multiple-ports). (8080, 8081, 8082 are available at the time this was documented) 

#### Step 5

Run the command ```npm run structor``` in the same directory,

click the link displayed in the console,

choose ```open```,

and

### You Are Ready to Go!

Please create an issue if the above does not work for you. You should now be able to follow along with the the documentation and get to building some UI!