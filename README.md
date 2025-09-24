# google_search_proxy

google_search_proxy is a magical Python module that performs Google searches with superpowers like automatic proxy handling, so you don't have to worry about a thing!

## Installation

### Install directly from GitHub (recommended)

```bash
pip install git+https://github.com/balasurajp/google_search_proxy.git
```

### Install from source

```bash
git clone https://github.com/balasurajp/google_search_proxy.git
cd google_search_proxy
pip install .
```

## Quick Start

```python
from google_search_proxy import GoogleSearch

# Let google_search_proxy do its magic!
search = GoogleSearch("your query", num=5, region="us", language="en", proxy=False)

# Perform search with automatic proxy handling
results = search.search()

# Print the magic search results
for result in results:
    print(result)
```

### Notes

- `proxy=True` enables automatic proxy retrieval using the `free-proxy` library.
- A random realistic User-Agent is selected for each request.

## Features

- Perform Google searches effortlessly with custom parameters.
- Automatic handling of proxies for each search.
- google_search_proxy selects a random user-agent for each request.
- It's super easy to use and makes searching Google a breeze.

## CLI (optional)

No CLI is provided at the moment. Use the Python API as shown above.

## Credits
- The updated project has been forked from [goprox](https://github.com/cloudkissed/goprox) and transformed into python package for easy installation.
- This project uses the amazing [free-proxy](https://github.com/jundymek/free-proxy) module to fetch and validate proxies.

## License

google_search_proxy is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
