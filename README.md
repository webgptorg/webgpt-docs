## Contributing

###TODO: review

To contribute to the documentation, you need to have Hugo installed. Follow these steps to install Hugo:

1. Download the latest version of Hugo from the [official releases page](https://github.com/gohugoio/hugo/releases).
2. Follow the installation instructions for your operating system [here](https://gohugo.io/getting-started/installing/).

After cloning the repository, you can make changes to the documentation. To preview your changes, run the following
command from the root directory of the repository:

```bash
$ hugo server
```

When done, you build the site by running the following command:
```bash
$ hugo --minify
```
and (typically all changes are made in the `public` directory) you add the changes to the staging area and commit them
with a meaningful message:
```bash
$ git add .
$ git commit -m "Your message here"
```
Finally, you push your changes to the `gh-pages` branch using the subtree command to push just the `public` directory
where the Hugo site is built:
```bash
$ git subtree push --prefix public origin gh-pages
```
