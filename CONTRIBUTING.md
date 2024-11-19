# Getting Started

## Dependencies

- [Pipenv](https://pipenv.pypa.io/en/latest/)
- [git](https://git-scm.com/)
- [GitHub Desktop](https://github.com/apps/desktop) (optional)

GitHub Desktop is useful if you don't want to memorize commands.
Alternatively, use [GitHub CLI](https://cli.github.com/) to setup authentication.

## Downloading

First fork the project (on GitHub, there will be a link for forking).
Run `git clone <url>` where `<url>` is the git link found on the forked repo's GitHub page.

This will clone the project into a local directory.

## Installing

Pipenv allows for traditional lockfile-based package management.
It's a bit cleaner than other python package managers, since it doesn't store environments
in the local directory, but focuses on reproducible builds.
In order to run commands in pipenv's virtual environment, you will either call
`pipenv run <command>` or drop into `pipenv shell`.

Install all python dependencies by running `pipenv install` inside the project directory.

In order to download the dataset, you'll want a [Kaggle](https://www.kaggle.com/) account
(or just download it directly and extract the file: [dataset](https://www.kaggle.com/datasets/nelgiriyewithana/global-youtube-statistics-2023)).
Then follow the instructions for [setting up authentication](https://www.kaggle.com/docs/api#authentication).

Download the dataset by running `kaggle datasets download nelgiriyewithana/global-youtube-statistics-2023 --unzip`
(Make sure you run this in `pipenv shell` or prepend `pipenv run` to the beginning!)

You're now ready to begin coding!
Just start jupyterlab in the virtual env: `jupyter lab`.

## Contributing

To add changes back to the upstream repo, first switch to a new branch (`git checkout -b <name>`).
Make your commits (`git commit -m <message>`) and then push to your remote (`git push`).
Then setup a pull request on GitHub. 
