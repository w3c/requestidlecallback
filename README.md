# Cooperative Scheduling of Background Tasks

Also known as **`requestIdleCallback`**.

This document defines an API that web page authors can use to cooperatively schedule background tasks such that they do not introduce delays to other high priority tasks that share the same event loop, such as input processing, animations and frame compositing. The user agent is in a better position to determine when background tasks can be run without introducing user-perceptible delays or jank in animations and input response, based on its knowledge of currently scheduled tasks, vsync deadlines, user-interaction and so on. Using this API should therefore result in more appropriate scheduling of background tasks during times when the browser would otherwise be idle.

Latest draft: https://w3c.github.io/requestidlecallback/

See also [Web performance README](https://github.com/w3c/web-performance/blob/gh-pages/README.md)
