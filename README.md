# pulsar-outline-view

Displays a hierarchical outline of your file’s symbols in a sidebar.

This package is a drop-in replacement for `atom-ide-outline`, but does not implement symbol search (use [symbols-view-redux][]) or call hierarchy.

<img width="1403" alt="pulsar-outline-view screenshot" src="https://github.com/savetheclocktower/pulsar-outline-view/assets/3450/0250ec54-80ac-461d-a718-f9548ed41c47">


## Outline providers

Many IDE integration packages will provide outlines. [Here’s the entire list of packages that provide the `outline-view` service.](https://web.pulsar-edit.dev/packages?service=outline-view&serviceType=provided)

### Fallback to symbol providers

When an outline provider isn’t available, `pulsar-outline-view` can fall back to displaying a flat list of symbols by consuming [packages that provide the  `symbol.provider` service](https://web.pulsar-edit.dev/packages?service=symbol.provider&serviceType=provided).

In some cases, `pulsar-outline-view` can even infer a hierarchy from the flat list.


[symbols-view-redux]: https://web.pulsar-edit.dev/packages/symbols-view-redux
