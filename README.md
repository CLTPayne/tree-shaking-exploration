# Tree Shaking Exploration

An isolated environment to explore how tree shaking works with webpack 4. This was inspired by uncertainty and questions around implementing the best practises described here - https://developers.google.com/web/fundamentals/performance/optimizing-javascript/tree-shaking/. 

### Quickstart:
#### How to start a project:
1. Fork this project in the GitHub UI
2. Clone your forked copy ```git clone https://github.com/[YOUR-USERNAME]/tree-shaking-exploration```
3. Change into the directory ```cd react-playground```
4. Use node version 10.8.0 and have npm installed
5. Run ```npm install``` to add module dependencies

#### How to run the code:
1. Build the bundle in one terminal window with ```npm run build```
2. Open the server in a second terminal window with ```npm start```
3. Your default browser will open the application at localhost:8080
4. When finished with the application, close both process with ```^c```

#### Project Goals:
1. Understand how to set up a project correctly for webpack to tree shake the bundle. 
2. Know how lodash is a strange case and accomodate this to make sure the whole of lodash isn't included in the compiled code. 
3. Use bundle analyzer to look at the before and after state of a bundle
4. Add some commit tools to check that the size of the bundle does not dramatically increase in a commit. Potentially a pre commit hook if all commits go straight into master. 

#### User Stories:
```
As a developer
So that I can implement and debug tree shaking in a large project
I need an isolated project to build a test case
```