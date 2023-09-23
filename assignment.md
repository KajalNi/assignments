-what is 'NPM'?
npm is a biggest package manager.npm is used primarily to manage and distribute packages and libraries of code written in js.All the packages are hosted over there, all the libraries, all the utility needed for our project.

1.npm allows developers to easily install, update, and manage packaged and dependencies for their js projects. Packages  can include code libraries, frameworks
2.npm provides version control for packages, allowing developers to specify which version of a package their project depends on. This will helps to ensure that project remain consistent and that new update don't cause any breaking changes 


-What is 'Parcel/ Webpack'? Why do we need it?
ans-Parcel is web application bundler. When we have normal html,  css and js file , our whole code needs to be bundeled together, it needs, to be compressed , minified , cached. Our whole code needs to be clean before it is sent to production and parcel helps us in doing that.

-what is '.parcel-cache'?
ans- The '.parcel-cache' directory is a directory used by the Parcel bundler to store cached data.It helps us subsequent builds.
This cache helps improve build performance  by reusing previously processed files when we  run the parcel bundler multiple times.
Dependencies Cache: Parcel caches information about our project's dependencies,such as our project's 'package.json' file, the 'node_modules' directory, and installed package dependencies. 

-what is 'npx'?
ans-npx is used to execute packages that are listed in your project's 'node_modules' directory or available from the npm registry. It allows us to run command-line tools and scripts provided by these packages without the need to install them globally. 

-what is the difference between 'dependencies' vs 'devDependencies'?
ans-dependencies are packages or modules that our project needs to run in a production environment. Dependencies are typically listed in the "dependencies" section of our project's package.json file whereas
DevDependencies are packages that are only needed during development or for testing purposes. These packages are not required for our app to fucntion in a production envrionment.DevDependencies typically include testing framesworks build tools and other utilities that help us develop, test and build our application.
These are listed in DevDependencies section of our package.json file.

-What is Tree Shaking?
ans- Tree shaking is a technique used in modern js development to eliminate unused or dead code from a JavaScript bundle or module.The goal is to create smaller and more efficient JavaScript bundles that load faster in web applications.


-What is Hot Module Replacement?
It is a development technique used in modern web develpment, particularly in the context of JavaScript and front-end frameworks like React,Vue.js and Angular. It allows developers to apply code and module updates in real-time, without requiring a full page reload or losing the app's current state, it means that if we have a certain state or data in our app(e.g. a form input or the current view), it won't be lost even while developers are actively making changes.

-List down your favorite 5 superpowers of Parcel and describe any 3 of them in your own words.
ans-It build dev environment for us
   -HMR
   -Tree Shaking
   -faster build becausing of caching
   -minification of code
   - 

























-what is '.gitignore'?What should we add and not add into it?
ans- Those files which are not supposed to be pushed on git repository are put inside .gitignore.we don't add those files on git repository which can be regenerated and we put them in .gitignore(e.g dist,node_modules,.parcel_cache), and those files which cannot be renerated are are not put inside .gitignore.


-what is the difference berween 'package.json' and 'package-lock.json'?
ans-'package.json' is a configuration of npm , it keeps those packages which are installed into our system, and it keeps their upgrade version , if there is ^-carent in front of the version , then will upgrade minor version of those packages and if it will have ~ - tilda, it will upgrade major version of those packages where as
'package-lock.json' will keep a track of exact version of package that is being installed.


-why should I not modify 'package-lock.json'?
ans-'package-lock.json' should not  be modified because because it contains the exact version of dependencies which is being installed in our system for our project. This ensures that all team members or deployment environment use the exact same versions of pakcages, it will prevent version conflicts and ensures consistency across different environment.

-What is 'node_modules'?Is it a good idea to push that on git?
ans-'node_modules' is a directory which contains all the third-party packages and modules that our project depends on. When we use npm to  install packages, they are typically downloaded and stored in the 'node_modules' directory of our project. It is kind of like database, it contains all the actual data of that dependencies that our project needs.It contains all the dependencies and their codes which are being used in project
It is not a good idea to push node_modules in git because it is automatically generated and its code may also change based on the dependency version.


-What is the 'dist' folder?
ans-when we install Parcel ,The 'dist' folder, short for distribution , it is also one of our directory in our project. It typically contains the compiled, bundled, or minified versions of our code.

-What is 'browserlists' Read about dif bundlers:vite, webpack,parcel
ans- 'browserlists' is a configuration files , in browserlist we can add which version of browser can support our app (e.g. 'last 2 chrome versions'), it means that our app will be supported 100% on last 2 versions of chrome. if the configuration will be like this(last 2 version),it means that our app will be supported on every last 2 versions of browsers.

-
