# web_ui_test_sample
Web UI Test sample of [chromium](https://www.chromium.org/) and [pytest](https://docs.pytest.org/en/latest/)


## Environment

* macOS: 10.0.0 above
* pip: 20.0.2
* Virtual ENV: pipenv, version 2018.11.26
* Language: python 3.7.5
* Chrome: Version 80.0.3987.132 (Official Build) (64-bit)
* Firefox: 73.0.1 (64 bit)

# Setup
1. Install [python](https://www.python.org/) on your machine, [pip](https://pypi.org/project/pip/) will be installed with this python installation；
2. Install [pipenv](https://github.com/pypa/pipenv);
3. Copy file `chromedriver` and `geckodriver` to `/usr/local/bin`;

# Manual
1. Enter the pipenv:
```shell
$ pipenv shell
```
2. Install the requirements libraries:
```shell
$ pipenv install
```
3. Run test:
```shell
// test special function with report
$ pytest --capture=no --verbose --html=./reports/pytest_selenium_test_report.html test_selenium_webdriver.py::TestURL::test_open_url
// test a file with report
$ pytest --capture=no --verbose --html=./reports/pytest_selenium_test_report.html test_selenium_webdriver.py
// test all items of the project
$ pytest
```

## License

`web_ui_test_sample` is avaliable under the MIT license. See the [LICENSE](https://github.com/gaoshanyu/web_ui_test_sample/master/LICENSE) file for more info.
