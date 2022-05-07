To start the slide show locally:

- `yarn install`
- `yarn dev <presentation>`
- visit http://localhost:3030

With this options, it's possible to record a presentation and edit files on browser.

To generate the html files locally:

- `yarn build`


There is also the option to export the presentations to pdf files:

- `yarn export`


To reproduce the project, including the github-pages:

- Fork de project
- Allow permission: settings -> Actions (General) -> Workflow permissions (Read and write permissions)
- It'll be generated a gh-pages branch with the content. It can take more than 3min.
- Start gh-pages branch: settings -> Pages -> Source -> Branch: gh-pages -> Save.

Learn more about [Slidev](https://github.com/slidevjs/slidev) on [guide](https://sli.dev/guide).

[Demo Slidev](https://kindelia.github.io/slidev/slides/) and [source code](./presentations/slides.md)

#### Improvements

- Decrease `yarn build` time.
- Can't go to a slide page directly from url. Example: [https://kindelia.github.io/slidev/slides/2](https://kindelia.github.io/slidev/slides/2)

