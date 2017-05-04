[step1]: ./docs/img/step1.jpg
[step2]: ./docs/img/step2.jpg
[step3]: ./docs/img/step3.jpg
[step3p2]: ./docs/img/step3p2.jpg
[step4p1]: ./docs/img/step4p1.jpg
[step4p2]: ./docs/img/step4p2.jpg
[step5p1]: ./docs/img/step5p1.jpg
[step5p2]: ./docs/img/step5p2.jpg
[step5p3]: ./docs/img/step5p3.jpg
[step5p4]: ./docs/img/step5p4.jpg

### Structor React App Starter

# Run on Cloud9

## Run Structor on Cloud9

#### *Prerequisites:*
* An account on [Cloud9](https://c9.io/) (it's free.)

#### Step 1

Create a basic Virtual Machine. **Make sure the privacy is set to public**.

![alt text][step1]

#### Step 2

Just to be safe, update npm and node:

```
npm i npm -g
nvm install 6
nvm alias default 6
```

![alt text][step2]

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

![alt text][step3]

#### Step 3.5

During the install, you will need to choose a directory, or simply press return,

![alt text][step3p5]

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

![alt text][step4p1]

to this,

```json
(...)
  "scripts": {
    (...)
    "structor": "structor -v -p 8080"
  },
(...)
```

![alt text][step4p2]

*Note* - The ```-v``` switch is optional but the ```-p <port>``` is [needed to run on Cloud9](https://docs.c9.io/docs/multiple-ports). (8080, 8081, 8082 are available at the time this was documented) 

#### Step 5

Run the command ```npm run structor``` in the same directory,

![alt text][step5p1]

click the link displayed in the console,

![alt text][step5p2]

choose ```open```,

![alt text][step5p3]

and

![alt text][step5p4]

### You Are Ready to Go!

Please create an issue if the above does not work for you. You should now be able to follow along with the the documentation and get to building some UI!