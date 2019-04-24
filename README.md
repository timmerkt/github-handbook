# VA GitHub Handbook

Helping Veterans Affairs (VA) teams design, build, and launch great digital services that meet the [Digital Standards](https://department-of-veterans-affairs.github.io/github-handbook/digital-standards) for the [Veteran-facing Services Platform](#fn1) by using and understanding GitHub.

Contact ___TDB___ for any questions, comments, or feedback.

## Contributing

* See [the repo Wiki](https://github.com/department-of-veterans-affairs/github-handbook/wiki) for
  * How this Jekyll site is organized
  * How to use Markdown for writing/editing content
  * How to update the ```modified-date``` that displays on site pages.
* See [CONTRIBUTING](CONTRIBUTING.md) for how to contribute content.

## Running and Development

Clone the project by executing `git clone https://github.com/department-of-veterans-affairs/github-handbook.git`.

After the clone is completed change your location to the project directory: `cd github-handbook`.

The rest of this guide will assume you are in this project directory.

### Installing and Running locally

This project is built using [Jekyll](https://jekyllrb.com). To run this project locally on your computer you will need to intall some dependencies.

<details>

<summary>Click here for pre-requisites instrucions</summary>

1. [Install Ruby](https://www.ruby-lang.org/en/downloads/) for your environment before you try to install the project dependencies.

2. Install Jekyll:

    `gem install bundler jekyll`

</details>

1. Install project dependencies:

    `bundle install`

2. Run Jekyll dev server:

    `bundle exec jekyll serve`

3. Once running visit [http://0.0.0.0:4000/github-handbook/](http://localhost:4000/github-handbook/)

### Docker and Docker Compose

<details>

<summary>Click here for more on Docker and its installation</summary>

This project has two file that help you use [Docker](https://docker.com) for development and running the project localy:

* [Dockerfile](Dockerfile)
* [docker-compose.yml](docker-compose.yml)

To be able to use this you will need Docker installed on your system:

* [Docker Desktop for MacOs or Windows](https://www.docker.com/products/docker-desktop)
* [Linux](https://hub.docker.com/search/?type=edition&offering=community&operating_system=linux)

`docker-compose` is an optional requirement but is highly recommended.

* [Install docker-compose](https://docs.docker.com/compose/install/)

</details>

#### Using docker-compose

Using docker-compose is as simple as excuting:

```shell
docker-compose up web
```

Once the project is running you can visit [http://0.0.0.0:4000/github-handbook/](http://0.0.0.0:4000/github-handbook/)

### Development

Thanks for considering contributing to our project! Please take some time and look at our [CONTRIBUTING.md](CONTRIBUTING.md) file.

#### General Tips

Take a quick look at our [project WIKI](https://github.com/department-of-veterans-affairs/github-handbook/wiki). Here you will find general information about the structure of our project.

#### How to start with development

1. Clone/fork this repo.
2. For best results (urls work correctly), run locally at 127.0.0.1:4000/github-handbook/

    ```shell
    docker-compose up web
    ```

    The Jekyll server will detect changes from files and reload the site. The only exception will be when editing the `_config.yml` file.

3. Whenever you make a change to content, also change the ```modified-date``` in the yml at the top of the relevant ```.md``` file.

    Eg.

    ```
    ---
    #
    modified-date: April 08, 2019
    ...
    other text
    ...
    ```

## License

All content is available under the [Creative Commons Zero v1.0 Universal license](LICENSE), except where otherwise stated.

## Colophon

* This project is based on the [18F/handbook](https://github.com/18f/handbook)

<hr>

<a name="fn1"></a>The *Veteran-facing Services Platform* is the set of technologies (and processes) that veteran-facing services on the [VA.gov](https://www.va.gov) website. VA teams who want to release a digital service for veterans using the Veteran-facing Services Platform should use this [Handbook](http://department-of-veterans-affairs.github.io/va-digital-service-handbook/) to learn how to do that.
