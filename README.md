# greyhatgt.github.io
Georgia Tech's cyber security student organization, website created with [Hexo](https://hexo.io/)

*this is a note to self*
## deploy to [greyhat.gatech.edu](http://greyhat.gatech.edu) 
*must be on GT internet/vpn*
1. login at https://hosting.gatech.edu/login (you may need access from a current admin)
2. click on GreyHat site
3. Click "Login to site" (this brings you to cPanel)
4. Click "Deploy from Git" and then "Pull now" to pull the latest changes from GitHub
<img width="1492" height="581" alt="how-to-deploy" src="https://github.com/user-attachments/assets/e91bdf17-ddf0-42fc-af8f-8251b8be338e" />


## deploy to GitHub sites:
```shell
# prerequisites: npm

# installation
$ npm install hexo-cli -g
$ cd /path/to/greyhatgt.github.io/  # NOT the GitHub.com repo!
$ npm install

# usage
# deployment one-liner
$ hexo clean && hexo generate && cp README.md public/ && cp index.html public/ && hexo deploy
```

## Deployment

This site is automatically deployed to GitHub Pages when you push to the `master` branch.

### Manual Deployment
```bash
# Make changes to your site
# Add and commit changes
git add .
git commit -m "Your commit message"
git push origin master

# The site will automatically deploy via GitHub Actions
# Check the Actions tab in your GitHub repository for deployment status
```

### Local Development
```bash
# Install dependencies
npm install

# Serve locally
npm run dev
# or
npm start

# Site will be available at http://localhost:4000
```

### Site URL
🌐 **Live Site**: https://greyhatgeorgiatech.github.io
