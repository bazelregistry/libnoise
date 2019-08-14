# Bazel Registry - libnoise

This repository contains a copy of the [libnoise](http://libnoise.sourceforge.net) sources, noiseutils and examples as well as `WORKSPACE` and `BUILD.bazel` files for [bazel](https://bazel.build/).

| Path | Source URL |
|------|------------|
| / | [libnoisesrc-1.0.0.zip](http://prdownloads.sourceforge.net/libnoise/libnoisesrc-1.0.0.zip?download)  |
| /noiseutils | [noiseutils.zip](http://libnoise.sourceforge.net/downloads/noiseutils.zip) |
| /examples | [examples.zip](http://libnoise.sourceforge.net/downloads/examples.zip) |

## Installation

Add this to your `WORKSPACE`

```python
load("@bazel_tools//tools/build_defs/repo:http.bzl", "http_archive")

http_archive(
    name = "bazelregistry_libnoise",
    strip_prefix = "libnoise-931a97a2568822e9774a3dcf7364639f7ddfd80b",
    url = "https://github.com/bazelregistry/libnoise/archive/931a97a2568822e9774a3dcf7364639f7ddfd80b.zip",
    sha256 = "fe2491c49fa5fd54acad23e9fbf6be430fa4a8ecd087ac7dd8d36b611f159227",
)
```
