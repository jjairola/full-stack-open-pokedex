# Exercise 1 - CI/DI pipeline

For this example, I use in examples JavaScript because it is the used language in Full Stack Open course series. When there are more developers working ins same project, tooling plays important part of development. It ensures that code base stays coherent when people with different skills, background and operating systems (for example. line endings)  work together in same codebase.

For example,

* Linting ensures that team follows same principles with code base and ensures some level of minimal “standard” for avoiding some basic mistakes, tools like ESLint (code quality) with Prettier (for styling) Also, when linting used with pre -commit hooks like Husky, some mistakes are catched early and no need to wait lint results from CI.

* Testing ensures (if done) ensures that code doesn’t break when project grows. Usually tools like Jest and Playwright are popular choices. Playwright offers speed of development with integration with VSCode with plugin that allows recoding of tests using UI.

* Building packages final project for distribution. In JavaScript this includes packaging modules, minimizing assets and transpiling code for combability. Tools like Vite and Webpack with babel transpilation are popular.

All these steps can be automated with CI/DI tools such as GitHub actions, Gitlab and Argo. Depending on the project CI/DI can be self-hosted or cloud. Jenkins is popular option for self-hosting. Now both GitHub and Gitlab provides free tier for small teams so in basic cases there is no need for self-hosting even in free -tier. Self-hosting good choice is there is very platform specific tasks that needs to be ran and custom configuration. But, managing Jenkins, it is just installed.
