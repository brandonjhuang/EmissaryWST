# Welcome to Emissary

Welcome Devs! We're excited to have you contribute to Emissary. We understand
that there is a lot to take in and we hope to provide some clarity to speed up
your journey and get you productive quickly.

## The Project Structure

Here you'll find all the information you need to know about our project structure.

EmmisaryWST:
  - client
    - css
      - lib
      - native css files
    - html
    - images
    - js
      - lib
      - native js files
  - developer_docs: all of our docs to help new developers get up to speed
  - server
    - config
    - models
      - form
      - native js files
    - notification
    - routes
      - appointment
      - company
      - employee
      - form
      - payment
      - theme
      - visitorList
      - home.js
    - test: server-side test cases, run with `Mocha` and coverage with `Istanbul`
  - test: client-side test cases, run with `Grunt` (see our `Gruntfile.js`)
  - util: helper js files that aren't official libs

## A Note about our Pipeline

Pipelines are important to ensuring your development process is functioning
properly and that all code introduced is working seamlessly. We detail our
pipeline here so that you may explore what we've used, take what you like,
replace what you don't, and get to coding quickly.

SCM: [GitHub](https://github.com/cse112-kissmyapp/EmissaryWST)  
CI/CD: [TravisCI](https://travis-ci.org/cse112-kissmyapp/EmissaryWST)  
Code Quality: [CodeClimate](https://codeclimate.com/github/cse112-kissmyapp/EmissaryWST)  
Linters:
  - HTML: [htmlhint](http://htmlhint.com/)
  - CSS: [csslint](http://csslint.net/)
  - JS: [jshint](http://jshint.com/)
  - *Note* - CodeClimate also runs `eslint`, and `csslint`.

Backend Testing:
  - [Mocha](https://mochajs.org/)
  - [Chai](http://chaijs.com/)
  - [Istanbul](https://istanbul.js.org/)

Frontend Testing:
  - [Selenium](http://www.seleniumhq.org/)
  - [SauceLabs](https://saucelabs.com/)

Code Coverage:
  - [CodeClimate](https://codeclimate.com/github/cse112-kissmyapp/EmissaryWST/coverage)
  - [CodeCov](https://codecov.io/gh/cse112-kissmyapp/EmissaryWST)

Monitoring:
  - [Mouseflow](https://mouseflow.com/)

Hosting:
  - Us: [Google App Engine](https://kiss-my-app.appspot.com/)
  - The Original [WebStormTroopers](https://github.com/danielchristiancazares/Emissary): [Heroku](http://webstormtroopers.herokuapp.com)

We've also enforced a pre-commit check in `package.json` (see ["pre-commit"](https://github.com/cse112-kissmyapp/EmissaryWST/blob/develop/package.json)) that runs all three linters above and before a commit can be made. Ideally, it should force the three linters to completely pass, but since the code we've inherited has quite a lot of issues that we are making progress fixing but haven't be able to fix in one go, we've had to remove the forced compliance for now. In the future it should be fairly simple to make work.

## User Stories, Features, and Progress

To help understand our evaluation of Emissary, and where we hoped to take it in the future, we have provided documentation that can be found in this folder.

Our user stories detail our vision for the application. They can be found [here](https://github.com/cse112-kissmyapp/EmissaryWST/blob/develop/developer_docs/Emissary%20User%20Stories.pdf).

We have the corresponding project board setup [here](https://github.com/cse112-kissmyapp/EmissaryWST/projects). You will see it is divided into two sections: `Backlog` and `v2.0`. Backlog describes our assessment of the project as we inherited it. It details our attempt to fix known issues, refactor code, and address technical debt. You can find our progress within that board. v2.0 describes our assessment of where the project may move in the future. Similarly, you can find our progress within that board.

## Our Stack & Integrations

As we've inherited code from past years, the project has grown and shrunk in many respects. Lots of code has been added and removed which can cause quite a bit of confusion as to what is going on. After inheriting the code, our developers paid special attention to sanitization and improving overall code quality in many regards: bug fixing, refactoring, removal of stale, unused code, removal of extra libs and/or files, plugins, integrations that weren't being used, etc...Currently we use `gulp` to handle all client-side building, and `node` + `express` for backend routing.

Furthermore, we've documented heavily what we use, why, and how it all fits together. Hopefully this will enable you to come up to speed pretty quickly and painlessly and to construct your own Pipeline accordingly.

To see our documentation on our Stack & Integrations, visit [this](https://github.com/cse112-kissmyapp/EmissaryWST/blob/develop/developer_docs/INTEGRATIONS.md).
