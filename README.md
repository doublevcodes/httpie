<br/>
<a href="https://httpie.io" target="blank_">
    <img height="100" alt="HTTPie" src="docs/httpie-logo.svg" />
</a>
<br/>

# HTTPie: human-friendly CLI HTTP client for the API era

HTTPie (pronounced _aitch-tee-tee-pie_) is a command-line HTTP client.
Its goal is to make CLI interaction with web services as human-friendly as possible.
HTTPie is designed for testing, debugging, and generally interacting with APIs & HTTP servers.
The `http` & `https` commands allow for creating and sending arbitrary HTTP requests.
They use simple and natural syntax and provide formatted and colorized output.

<img src="docs/httpie-animation.gif" alt="HTTPie in action" width="100%"/>

[![Docs](https://img.shields.io/badge/stable%20docs-httpie.io%2Fdocs-brightgreen?style=flat&color=%2373DC8C&label=Docs)](https://httpie.org/docs)
[![Latest version](https://img.shields.io/pypi/v/httpie.svg?style=flat&label=Latest&color=%234B78E6&logo=&logoColor=white)](https://pypi.python.org/pypi/httpie)
[![Build](https://img.shields.io/github/workflow/status/httpie/httpie/Build?color=%23FA9BFA&label=Build)](https://github.com/httpie/httpie/actions)
[![Coverage](https://img.shields.io/codecov/c/github/httpie/httpie?style=flat&label=Coverage&color=%2373DC8C)](https://codecov.io/gh/httpie/httpie)
[![Twitter](https://img.shields.io/twitter/follow/httpie?style=flat&logo=twitter&color=%234B78E6&logoColor=%234B78E6)](https://twitter.com/httpie)
[![Chat](https://img.shields.io/badge/chat-Discord-brightgreen?style=flat&label=Chat%20on&logo=discord&color=%23FA9BFA)](https://httpie.io/chat)


## Main features

- Expressive and intuitive syntax
- Formatted and colorized terminal output
- Built-in JSON support
- Forms and file uploads
- HTTPS, proxies, and authentication
- Arbitrary request data
- Custom headers
- Persistent sessions
- `wget`-like downloads

See the [complete list of features](https://httpie.io/docs).

## Documentation

Visit full documentation and installation guides at [httpie.io/docs](https://httpie.io/docs).

## Installation

HTTPie can be installed using Homebrew on macOS (`brew install httpie`), and `pip` on Linux, Windows and other Operating Systems (e.g. `python -m pip install --upgrade httpie`).

Learn more at [httpie.io/docs#installation](https://httpie.io/docs#installation)

## Examples

Hello World:

```
$ https httpie.io/hello
```

Custom [HTTP method](https://httpie.io/docs#http-method), [HTTP headers](https://httpie.io/docs#http-headers) and [JSON](https://httpie.io/docs#json) data:

```
$ http PUT pie.dev/put X-API-Token:123 name=John
```

Build and print a request without sending it using [offline mode](https://httpie.io/docs#offline-mode):

```
$ http --offline pie.dev/post hello=offline
```

Use [GitHub API](https://developer.github.com/v3/issues/comments/#create-a-comment) to post a comment on an [Issue](https://github.com/httpie/httpie/issues/83) with [authentication](https://httpie.io/docs#authentication):

```
$ http -a USERNAME POST https://api.github.com/repos/httpie/httpie/issues/83/comments body='HTTPie is awesome! :heart:'
```

See [the documentation](https://httpie.io/docs) for a complete list of examples and use cases.

## Contributing

Please read the [contribution guide](https://github.com/httpie/httpie/blob/master/CONTRIBUTING.md) for how to contribute.
Have a look through existing [Issues](https://github.com/httpie/httpie/issues) and [Pull Requests](https://github.com/httpie/httpie/pulls) that you could help with. If you'd like to request a feature or report a bug, please [create a GitHub Issue](https://github.com/httpie/httpie/issues) using one of the templates provided.

## Community & support

- Visit the [HTTPie website](https://httpie.io) for full documentation and useful links.
- Join our [Discord server](https://httpie.io/chat) is to ask questions, discuss features, and for general API chat.
- Tweet at [@httpie](https://twitter.com/httpie) on Twitter.
- Use [StackOverflow](https://stackoverflow.com/questions/tagged/httpie) to ask questions and include a `httpie` tag.
- Create [GitHub Issues](https://github.com/httpie/httpie/issues) for bug reports and feature requests.
- Subscribe to the [HTTPie newsletter](https://httpie.io) for occasional updates.
