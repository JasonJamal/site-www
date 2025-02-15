---
title: Using Google Cloud
short-title: Google Cloud
description: Your Dart app can use many Google Cloud services — Firebase, Google Cloud Platform, and more.
---

Dart servers can use many
[Google Cloud products](https://cloud.google.com/products),
often with the help of pre-packaged [Docker images][]
that the Dart team maintains.
For information about creating HTTP servers with Dart, see the
[Write HTTP servers page](/tutorials/server/httpserver).

For information about other Google APIs (including Firebase)
that you might want to use from Dart code,
see the [Google APIs page](/guides/google-apis).

## Cloud Run

You can use Cloud Run's flexible container support,
combined with Dart's Docker images,
to run server-side Dart code.
Examples of Dart servers implemented to run on Cloud Run are
[in the dart-lang/samples/repo][server examples].

For more information about using Cloud Run, see the documentation for
[building and deploying a service in other languages][cr].


## Compute Engine

To run Dart code on Compute Engine,
use Compute Engine's support for running containers,
combined with Dart's Docker images.

For more information, see the Compute Engine documentation for
[using software containers][ce].

## Kubernetes

To run Dart on clusters of Compute Engine instances,
use Google Kubernetes Engine (GKE).

For more information, see the [GKE overview][].

## App Engine

[App Engine][] support for Dart is incomplete,
so we recommend that you **use Cloud Run** instead of App Engine for new
server-side Dart code.
If you _want_ to use App Engine, consider using the [`appengine` package][].

## Functions Framework for Dart

The [Dart Functions Framework][] is a Google-sponsored open source 
FaaS (Function as a Service) project that makes it easy to write Dart functions
instead of server applications for handling web requests.
Using the framework, you can create functions that handle HTTP requests
and [CloudEvents][] and deploy them to Google Cloud.

[Read the documentation][functions docs] to get started.

[App Engine]: https://cloud.google.com/appengine
[`appengine` package]: {{site.pub-pkg}}/appengine
[ce]: https://cloud.google.com/compute/docs/containers
[cr]: https://cloud.google.com/run/docs/quickstarts/build-and-deploy/other
[server examples]: https://github.com/dart-lang/samples/tree/master/server
[Docker images]: https://hub.docker.com/r/google/dart
[GKE overview]: https://cloud.google.com/kubernetes-engine/docs/concepts/kubernetes-engine-overview
[Dart Functions Framework]: {{site.pub-pkg}}/functions_framework
[CloudEvents]: https://cloudevents.io/
[functions docs]: https://github.com/GoogleCloudPlatform/functions-framework-dart/tree/main/docs
