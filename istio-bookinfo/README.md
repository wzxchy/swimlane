# Helm Chart of Istio Bookinfo Example

This example of helm chart deploys a sample application composed of four separate microservices used to demonstrate various Istio features.


The Bookinfo application is broken into four separate microservices:

* `productpage`. The productpage microservice calls the details and `reviews`
  microservices to populate the page.
* `details`. The details microservice contains book information.
* `reviews`. The `reviews` microservice contains book reviews. It also calls the
  `ratings` microservice.
* `ratings`. The `ratings` microservice contains book ranking information that
  accompanies a book review.

There are 3 versions of the `reviews` microservice:

* Version v1 doesn’t call the `ratings` service.
* Version v2 calls the `ratings` service, and displays each rating as 1 to 5
  black stars.
* Version v3 calls the `ratings` service, and displays each rating as 1 to 5 red
  stars.

