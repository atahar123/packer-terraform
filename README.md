# Node App Environment

## Prerequisites:
- Vagrant
- VirtualBox
- All other dependencies are installed from the provisions, you don't need anything else.

## How to clone this repo:
In your terminal, please type in the following:
```
git clone git@github.com:atahar123/DevEnv.git
```

### To run the app:
- On the directory:
```
vagrant up
vagrant ssh app
cd ..
cd ubuntu/
cd app
cd seeds
node seed.js
cd ..
npm start
```

### After starting, you should see the following:
"Your app is ready and listening on port 3000"


### To view the app:
- Go to your chosen browser
- type in the following:
```
development.local
```
You should see the Sparta Global logo. This means it is working.

- To see the posts, type in:
```
development.local/posts
```
