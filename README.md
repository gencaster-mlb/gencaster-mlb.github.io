# gencaster.org

A website about the [Gencaster](https://gencaster.org/) project. The site builds from [Nuxt 3](https://nuxt.com/docs/getting-started/introduction) with [Content](https://content.nuxtjs.org/).

## Content

The content is located in the `/content` directory. To create new content add a Markdown file in the according subdirectory. It's easiest to copy an existing file, to make sure all the required fields are there.  
Images need to be placed in the `/public/img` directory. See `/content/3.news/.blueprint.md` (the leading `.` in the filename hides it from being published) for an example of how to link them in a news article. 

## Local Development

Make sure to install the dependencies:

```bash
yarn install
```

Start the development server on http://localhost:3000

```bash
yarn dev
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.

## Supported by

[Media Tech Lab Bayern batch #3](https://github.com/media-tech-lab)

<a href="https://www.media-lab.de/en/programs/media-tech-lab">
    <img src="https://raw.githubusercontent.com/media-tech-lab/.github/main/assets/mtl-powered-by.png" width="240" title="Media Tech Lab powered by logo">
</a>
