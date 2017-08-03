# Data Entry Clerk

> Hello, I'm your friendly _data entry clerk_. I take whatever data you give me
and store them in your database for later processing.

**Data Entry Clerk** might be a little demeaning, but it describes the purpose
of this project perfectly: To be able to analyse data, you need to have data.
The DEC stores whatever data you give it in a database for later processing.

Most external services allow data to be shared via [webhooks][webhook]. The DEC
provides an endpoint that accepts such webhooks and stores their payload in a
database.

## Development

To extend the service or customize it, either fork or clone this repository.

### Installation

We recommend that you create a [virtual environment](virtualenv) to isolate the
Python interpreter and all dependencies from your system Python or any other
projects you're working on.

```bash
virtualenv --python=$(which python3) .venv
source .venv/bin/activate
```

Then, install DEC's dependencies:

```bash
pip install -r requirements.txt
```

After that, you can hack away and make any changes you require to make the code
work for you. 😊

### Running the server

During development, you can run the server by simply starting the app:

    FLASK_APP=app.py flask run

## License

Copyright (c) 2017 Automatiqa

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

[virtualenv]: http://python-guide-pt-br.readthedocs.io/en/latest/dev/virtualenvs/
[webhook]: https://en.wikipedia.org/wiki/Webhook
