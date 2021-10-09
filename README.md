# go mod init github.com/progmamun/Go-API

# go get -u github.com/gorilla/mux

- Package mux implements a request router and dispatcher.

The name mux stands for "HTTP request multiplexer". Like the standard http.ServeMux, mux.Router matches incoming requests against a list of registered routes and calls a handler for the route that matches the URL or other conditions. The main features are:

- Requests can be matched based on URL host, path, path prefix, schemes,
  header and query values, HTTP methods or using custom matchers.
- URL hosts, paths and query values can have variables with an optional
  regular expression.
- Registered URLs can be built, or "reversed", which helps maintaining
  references to resources.
- Routes can be used as subrouters: nested routes are only tested if the
  parent route matches. This is useful to define groups of routes that
  share common conditions like a host, a path prefix or other repeated
  attributes. As a bonus, this optimizes request matching.
- It implements the http.Handler interface so it is compatible with the
  standard http.ServeMux.
