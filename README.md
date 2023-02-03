# The Best Way to Host & Deploy a React Application To Netlify
# Deploy Manually :
## Steps
### 1 - Create a folder with your app name (for me "demo-app")

then run command :  `npx create-react-app  demo-app`  
it will create another folder named "demo-app" inside our initial "demo-app" folder

so instead run the command below to create the app directly inside our initial "demo-app" folder
`npx create-react-app ./`

### 2  - Building process

Run `npm start` to run the app on browser
Run `npm run build` to build (production mode or to minify) the app manually
After running above command a new folder will be created named **"build"**

### 3 - Manual Deployment Process

To deploy the app manually to netlify we just have to _drag and drop_ the build folder to netlify and that's it.

## *Disadvantage of manual deployment

In this deployment method , we can't do regular updates to the deployed app.


# Deploy from GitHub :
## Steps
### 1 - First, make a repo on GitHub Web 

### 2 - Then, remote add the app to GitHub Web
- git init => for initialize git
- git add . => for staging all the files to git
- git commit -m "first commit" => for commit to git with a commit message
- git branch -M main => to change the branch name to "main" which in initially "master" as GitHub officially changed name of branch from `master` to `main`.
- git remote add origin [git repo url] => for adding local repo to GitHub Web
- git push -u origin main => to push local repo to remote repo

### 3 - Deployment Process from GitHub
Go to netlify and just click _New site from Git_ and follow the process ahead.

>Notes : In this deployment process, we don't have to build the app to production mode (or to minify) , netlify will handle the build process on its own. Here all regular updates will be reflected to app after pushing to GitHub.
