<h1>Quo <img src="https://media.giphy.com/media/12oufCB0MyZ1Go/giphy.gif" width="50"></h2>



---

Quo is a Python  based web frame and a toolkit for writing Command-Line Interface(CLI) applications.

---
<p align="center">
  <a href="https://quo.rtfd.io"><img src="https://miro.medium.com/max/1400/1*wXEkk8gS6FMrBC-mJvVekQ.png" alt="Quo"></a>
</p
---


[![PyPI version](https://img.shields.io/pypi/v/quo.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/quo/)
[![Documentation Status](https://readthedocs.org/projects/quo/badge/?version=latest)](https://quo.readthedocs.io/en/latest/?badge=latest)
[![Supported Python versions](https://img.shields.io/pypi/pyversions/quo.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/quo/)
[![Travis CI status](https://img.shields.io/travis/secretum/quo/master?label=Travis%20CI&logo=travis)](https://travis-ci.org/secretum/quo)
[![codecov](https://codecov.io/gh/secretum/quo/branch/master/graph/badge.svg)](https://codecov.io/gh/secretuminc/quo)
[![GitHub](https://img.shields.io/github/license/secretuminc/quo.svg)](LICENSE.txt)
[![quo](https://snyk.io/advisor/python/quo/badge.svg)](https://snyk.io/advisor/python/quo)

---

Quo improves programmer's productivity because it's easy to use and supports auto completion which means less time will be spent debugging. Simple to code, easy to learn, and does not come with needless baggage.

---

---

**Quo📄** : <a href="https://quo.rtfd.io" class="external-link" target="_blank">Documentation</a>

---

## Requirements

Python 3.6+

## Installation

<div class="termy">

```console
Install
$ pip install quo

or install and update
$ pip install -U quo
🔸🔸🔸🔸🔸💯 
Quo has been installed successfully🎉 
```

</div>

## Example

### Example 1

* Create a  file `test1.py` 

```Python
import quo
quo.echo(f'Hi there')

```

### Example 2
`test2.py`

```Python
import quo
quo.flair(f'This is colorful', bg="red", fg="white")

```

### Example 3

`test3.py`

```Python
import quo
@quo.command()
@quo.option("--name", prompt="What is your name?:") 
def hello(name):
   quo.echo(f'Hello {name}!')

if __name__ == '__main__':
    hello() 

```

### Example2
* `test.py`

```Python
import quo 
    @quo.command()
    @quo.option("--count", default=1, help="The number of times the feedback is printed.")
    @quo.option("--name", prompt="What is your name", help="This prompts the user to input their name.")
    @quo.option("--profession", prompt="What is your profession", help="This prompts user to input their proffession")
    def survey(count, name, proffession):
       
        for _ in range(count):
            quo.echo(f"Thank you for your time, {name}!")

    if __name__ == '__main__':
        survey() 
// A simple survey application
```

## Contributing

If you run into an issue or want to contribute, we would be very happy if you would file a bug on the [issue tracker](https://github.com/viewerdiscretion/quo/issues).

## Donate
In order to for me to maintain this project, `please consider donating today` 

* <a href="https://www.paypal.com/donate?hosted_button_id=KP893BC2EKK54" target="_blank"><img src="https://res.cloudinary.com/edev/image/upload/v1583011476/button_y8hgt8.png" alt="Donate" style="width: 250px !important; height: 60px !important;" width="250" height="60"></a>

