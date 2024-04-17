# Python Web Scraping Demo
## Introduction
To give my students a taste of how web scraping looks like

## Some Info Before You Begin
* Instead of using `conda` virtual environments, I'm using a package manager called [Pipenv](https://pipenv.pypa.io/en/latest/).
    * `conda` is great for quickness if you want to get everything setup. However, it is bloated as it installs generally everything that you may not use on your app.
    * You can always install the relevant modules and packages within your `conda` setup without going through `pipenv`.

## How to run Jupyter Notebooks in VS Code With Pipenv
### Why?
This is to tightly control what modules and packages we install for our app, so that it is not bloated and we can safely run it in any environment.
### How?
* Install the `Jupyter` extension on your VS Code.
    * It will enable VS Code the ability to detect kernels for use.
* Install `ipykernel` with `pipenv` in your project folder.
    * `pipenv install ipykernel`
* Activate your `pipenv shell`.
    * `pipenv shell`
* Create a virtual environment for `ipykernel` using the `pipenv` environment (you should have activated your `pipenv shell` when you run the following code):
    * python -m ipykernel install --user --name=my-virtualenv-name
* Create and open a Jupyter notebook file in your VSCode, and you should be able to select the name of the virtual environment which you just created.
* Or run `jupyter notebook` in your `pipenv shell` and select the name of the virtual environment which you just created.

## How does web scraping work in layman terms?
* It simulates and automates the behavior of a web browser, and in our case, we are using Chrome, thus we need to install `ChromeDriver` in our machines.
    * Easy to install on MacOS, but takes a level of understanding to install ChromeDriver on Windows.
    * `ChromeDriver` actually uses the Chrome version found in your local machine.
        * It is not in parity, you might run into errors running it. Ensure version parity between the ChromeDriver and your Chrome browser.
        * Download ChromeDriver here: https://googlechromelabs.github.io/chrome-for-testing/

