# Python + Selenium + Geckodriver devcontainer

This devcontainer setup consists of:

- A python container with `Pipenv` and `Selenium` already installed
- A Selenium firefox container acting as the browser

## Configration

Go to `devcontainer.json` and modify the parameters you want. Everything is commented in the file so it should be straightforward.

Add any other components you require in the `docker-compose.yml` file.

## Starting the devcontainer

To start the dev container just run:

```
Dev Containers: Reopen in Container
```

## Code

In your python code you need to initialize the webdriver this way:

```
options = webdriver.FirefoxOptions()
driver = webdriver.Remote(command_executor="http://browser:4444/wd/hub", options=options)
```

To view what's going on with the browser:

http://localhost:7900/?autoconnect=1&resize=scale&password=secret

You can also head to http://localhost:7900 and insert the password `secret` manually
