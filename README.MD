# Pareto Operating System (ParetOS)

The ParetOS is a browser-based, high-level operating system designed to maximize human potential. It is designed to give you the 20% of software you need on a day-to-day basis that gives you 80% of the benefits modern tech has to offer.

Live at [https://paret0.com](https://paret-os.vercel.app/)

## The Arena

A multiplayer, competitive habit tracking competition where you and your friends can see who has the best work ethic. Or who spends the most time playing videogames. Or who makes the most outbound sales call in your company. You can create your own template, and invite friends to play.

![The Pareto Arena](/screenshots/new_sprint.png "The Pareto Arena")

## Pareto Learning

Focus on learning the 20% of a skill that gives you 80% of the value. In the ParetOS, we start with offering Full-Stack JavaScript Development as a proof of concept for mentorship-guided, self-study learning through building. Included is a fully featured curriculum for you to start from the basics of creating a GitHub account, through building your first project and tackling technical interviews.

![Learn Full-Stack JS](/screenshots/new_learning.png "Pareto Learning - JavaScript")

## Mentorship

More effective than almost anything towards helping people thrive in life is mentorship. We have built-in support, though limited, to allow members to become mentors to other Paretoans. They can review their stats in the Arena, and leave comments/feedback/approval for the curriculum they submit through the Learning modules.

![Mentorship](/screenshots/mentorship.png "Mentorship Built-In")

## Library of Context

A crowd-sourced & curated collection of resources that help decrease the barriers to success in the tech industry. Discover job boards you didn't know about, understand the players and heavy hitters in your local area & read curated tutorials, articles and resources designed to help you learn full-stack development in an optimized way. We encourage people to introduce themselves in our Discussions thread, so that we can add new regions, cities and countries to our Library for our community to contribute towards.

![Library of Context](/screenshots/new_context.png "The Library of Context")

## We are live folks

Signup is open at https://paret0.com - for those making an account, you may notice that the 'Training' that focuses on Full-Stack JavaScript Development is hiding behind a paywall. This is what I call the 'Paywall Puzzle' - based entirely on the code in this front-end repository, after forking it, you can modify the code and freely gain access to all the educational curriculum without paying. It requires changing a couple of values, commenting out a couple of functions while executing something. Believe it or not, this is a generous hint. If you can figure out how to do that - congratulations, you probably don't need to buy access to the curriculum! If you can't figure it out, you should seriously consider investing in your education. Included in the $89 is the Full-Stack Starter Kit, a set of laminated paper cheat-sheets, stikers, workbooks and playing cards that help teach you the 20% of JavaScript you need to know to get 80% of the actionable information needed to start writing code. In addition to the online curriculum. If you cannot make that payment (for example, living in Uganda and don't have VISA/Mastercard payment option) - open an Issue, and explain your situation! We will find a creative solution. 

It's also a great way of supporting this project, and you get real value that you can either use yourself to prepare for technical interviewing, or donate to a friend/colleague/connection who needs it.

### Open-Source Development

Want to contribute? Great! We have quite some issues in the repository, and I have tried to mark the easier ones as 'good first issue'. There are also issues marked as 'ownership' - these issues cover an item on our product backlog, a discrete, end to end piece of functionality that requires polish and a significant amount of work to implement. Completing one of these ownership tasks qualifies you to become a maintainer of the project, pending your availability and desire to do so. You will be a member of our Open-Source Hall of Fame as well!

To fix a bug or contribute a new feature, follow these steps:
- Fork the repo
- Install the pnpm package manager `brew install pnpm` or `npm i -g pnpm`
    a. Why pnpm? It uses an 'offline caching' approach, where you keep all of your download dependencies in an offline repository, and automatically put them into other projects that need to install them. This way, we are limiting the amount of hard drive space being used. This creates two major benefits.
        1. We can theoretically run `pnpm install` when troubleshooting while fully offline.
        2. When reviewing forks of ParetOS, we do not need to redownload 150mb of node_modules every time. This is beneficial for some of our international contributors, who pay for data by the GB. If they integrate pnpm into their dev workflow, it will save them a lot of space.
        3. For the record, `yarn install` and `npm install` still work for now (I think). However, `pnpm` is the package manager that will have first class support.
- Run `pnpm install` to install the dependencies, once you have `cd`'d into the directory
    a. There is a known issue where Puppeteer's install script may hang indefinitely. In this case, first try updating to Node 16 and running again.
    b. If this does not work, this will sound weird, but try using a different wireless connection. Yours may be too slow, or have some weird configuration settings. `https://github.com/puppeteer/puppeteer/issues/5611`
- Run `pnpm start` to start the dev server
    a. `pnpm add <package_name>` to add a new npm dependency to the project.
- You will get an es-lint error about some config - go to `package.json`, and press Command+S - the error should go away.
- Create a new branch (`git checkout -b improve-feature`)
- Make the appropriate changes in the files
- Add Git changes to reflect the changes made
- Commit your changes (`git commit -m 'Improve feature'`)
- Push to the branch
- Send a PR, and become a legend

### Bug / Feature Request

If you find a bug, have a great idea or just a question - please open an issue [here](https://github.com/mikhael28/paretOS/issues/new)!

## Built with

- [React + JavaScript](https://reactjs.org/) - The classics, the essentials..
- [Progressive Web Application](https://web.dev/progressive-web-apps/) - Better than investing time into a mobile application, I figure that having the offline functionality of a PWA will give us the right balance of features and accessibility. Right now, the PWA service-worker is disabled - it will be re-enabled after a truly stable build is ready for launch (Product Hunt, Show HN, all that jazz)
- [AWS Lambda](https://aws.amazon.com/lambda/) - Serverless first
- MongoDB + other services.

## Admin

- There is a separate, not quite fully featured admin platform.
- We can create mentees, mentors, match them, and a host of other options.
- Currently hidden from view, along with the APIs, to prevent foul play. This open-source repository focuses strictly on the front-end - trusted contributors will be invited to collaborate on the back-end.

## Intellectual Property Notice
- This CODE is open-source. 
- The intellectual property in regards to the branding of the Pareto logos, the educational curriculum inside the Full-Stack Starter Kit, and the knowledge base belongs to Michael Litchev. 


## Team

[![Michael 'Misha' Litchev](https://avatars.githubusercontent.com/u/15205259?s=400&u=64ad9374b8d98f09dc5709fcc737e5ec4f2447f3&v=4)](https://github.com/mikhael28)

## [License](https://github.com/mikhael28/paretOS/blob/main/LICENSE)

GNU General Public License Version 2 Only © [Michael 'Misha' Litchev](https://github.com/mikhael28)
