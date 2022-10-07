# webplatform
Build tools for Web Driven: Platforms, Operating Systems, Embedded Devices

Mainly this supplys the glue code for the modules: chromium-content and wpe-webkit
- chromium/src/content (webkit)
- chromium/src/webkit (content)
- chromium/src/third_party/webkit (content,chromium)

## Motivation
For Historical Reasons there existed a lot of Monolithical Solutions to build WebPlatforms but with today Distributed and Incremental Build Systems this does not scale and is not maintainable anymore. As the code has grown, features inevitably hooked into the wrong places, causing layering violations and dependencies that shouldn‘t exist. It’s been hard for developers to figure out what the “best” way is because the APIs (when they existed) and features were together in the same directory. To avoid this happening, and to add a clear separation between the core pieces of the code that render a page using a multi-process browser, consensus was reached to move rendering into its own module called content.
