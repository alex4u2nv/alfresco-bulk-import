<img align="right" width="96px" height="96px" src="https://raw.github.com/pmonks/alfresco-bulk-import/master/icon.png">
# Alfresco Bulk Import Tool

[![Build Status](https://img.shields.io/travis/pmonks/alfresco-bulk-import.svg)](https://travis-ci.org/pmonks/alfresco-bulk-import)
[![Downloads](https://img.shields.io/github/downloads/pmonks/alfresco-bulk-import/latest/total.svg)](https://github.com/pmonks/alfresco-bulk-import/releases)
[![Open Issues](https://img.shields.io/github/issues/pmonks/alfresco-bulk-import.svg)](https://github.com/pmonks/alfresco-bulk-import/issues)
[![License](https://img.shields.io/github/license/pmonks/alfresco-bulk-import.svg)](https://github.com/pmonks/alfresco-bulk-import/blob/master/LICENSE)

## What Is It?
A high performance bulk import tool for the open source [Alfresco Document
Management System](http://www.alfresco.org/).

"'High Performance', you say?"

Why yes.  Alfresco's built-in mechanisms for moving large amounts of content into the repository (the various [file-server protocols](http://docs.alfresco.com/5.0/concepts/protocols-about.html), the venerable [ACP mechanism](http://docs.alfresco.com/3.4/concepts/acp-files.html), the mind-bogglingly inefficient [CMIS standard](https://www.oasis-open.org/committees/cmis/) etc.) all suffer from a variety of limitations that make them a lot slower than the core Alfresco repository.  This tool cuts out virtually all of that nonsense, attempts to maximise "mechanical sympathy" (which, for Alfresco, basically means treating your database nicely), and makes one or two large and opinionated assumptions that allows it to be a lot faster than anything else out there.

In terms of benchmarks, the old v1.x versions of the tool have regularly demonstrated sustained ingestion rates of over 500 documents per second in production environments, and in testing, the v2.x version has been shown to be up to 4X faster than 1.x (in specific circumstances, notably for streaming imports).

## Documentation
 * [Installation](https://github.com/pmonks/alfresco-bulk-import/wiki/Installation)
 * [Usage](https://github.com/pmonks/alfresco-bulk-import/wiki/Usage)
 * [Troubleshooting Tips](https://github.com/pmonks/alfresco-bulk-import/wiki/Troubleshooting)
 * [All Documentation](https://github.com/pmonks/alfresco-bulk-import/wiki/Home)

## Resources
 * [Mailing List](https://groups.google.com/forum/#!forum/alfresco-bulk-filesystem-import)
 * [Known Issues](https://github.com/pmonks/alfresco-bulk-import/labels/bug)

Older resources (less relevant for v2.0+):
 * [Project site for v1.x](https://github.com/pmonks/alfresco-bulk-filesystem-import)
 * [DevCon 2011 presentation](http://www.slideshare.net/alfresco/taking-your-bulk-content-ingestions-to-the-next-level)
 * [Design overview from 2009](http://blogs.alfresco.com/wp/pmonks/2009/10/22/bulk-import-from-a-filesystem/)

## What's New?
 * [Commit log](https://github.com/pmonks/alfresco-bulk-import/commits/master)

## Commercial Support
**This extension is not supported by [Alfresco Software Inc.](http://www.alfresco.com/)**,
although a fork of an early, pre-release version of this tool has been included in Alfresco
Enterprise since v4.0, and is supported by [Alfresco support](http://support.alfresco.com).

Please note that the embedded fork has never been rebased against upstream, meaning that it
is functionally equivalent to the 1.0-RC1 (ancient, circa mid-2010) version of the tool.  It
also has a number of serious bugs (e.g. incorrect "source striping" algorithm, no support
for Alfresco clusters) that the orignal has never had.  It has also been reported to be
around 25% slower than v1.x of the original (which themselves are slower than v2.x).

**Use of the embedded fork is STRONGLY discouraged!**

## License
Copyright © [Peter Monks](mailto:pmonks@gmail.com) 2007-2015. Licensed under the [Apache 2.0 License](http://www.apache.org/licenses/LICENSE-2.0.html).

## Attributions
 * [Contributors list](https://github.com/pmonks/alfresco-bulk-import/blob/master/CONTRIBUTORS.md)
 * Icon adapted from [Appzgear](http://www.flaticon.com/free-icon/arrow-pointing-down-a-container_26007) on [www.flaticon.com](http://www.flaticon.com/).
 * [Contributing](CONTRIBUTING.md) file heavily inspired by the [Atom](https://github.com/atom/atom/blob/master/CONTRIBUTING.md) project.

## Contributing
Please see [Contributing](CONTRIBUTING.md).
