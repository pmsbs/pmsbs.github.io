# [Departamento de Tecnologia e Inovação | Prefeitura Municipal de São Bento do Sapucaí](www.pmsbs.sp.gov.br)

A Jekyll-based website for Refugio Pinheiro Beira Rio. This site provides information about the location, services, and how to get in touch.

## About the Project

This repository contains the source code for the Refugio Pinheiro Beira Rio website, built using the Jekyll static site generator. The site is hosted on GitHub Pages, which automatically builds and serves the content from this repository.

## Getting Started
To get a local copy up and running, follow these simple steps.

### Prerequisites

You'll need to have Ruby, Jekyll, and Bundler installed on your machine.

* Ruby: Download and install Ruby

* Jekyll: Install Jekyll and Bundler gems.

```sh
gem install jekyll bundler
```

### Installation

1. Clone the repository:


```sh
git clone git@github.com:pmsbs/pmsbs.github.io.git
```

2. Install the required gems:

```sh
bundle install
```

### Running Locally

To serve the site locally and see changes in real-time, run the following command from the project's root directory:

```
bundle exec jekyll serve
```

This will start a local server, typically at http://localhost:4000.

## File Structure

The project has a standard Jekyll file structure:

* `_config.yml`: Global configuration file for the site.

* `_layouts/`: Contains the site's main layouts (e.g., `default.html`, `page.html`).

* `_includes/`: Holds reusable snippets of code like the header, footer, or navigation.

* `_posts/`: Stores blog posts or news articles. The filenames must follow the `YYYY-MM-DD-title.md` format.

* `assets/`:Contains static assets like images, stylesheets, and JavaScript files.

* `_sass/`: Stores Sass files for generating the site's CSS.

* `index.html`: The main homepage of the site.

* `about.md`, `contact.md`, etc.: Markdown files for static pages.

## Contributing

Contributions are what make the open-source community an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

1. Fork the Project.

2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`).

3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`).

4. Push to the Branch (`git push origin feature/AmazingFeature`).

5. Open a Pull Request.

## License

Distributed under the MIT License. See `LICENSE` for more information.

## Credits

This site was built using Jekyll and various open-source resources.
