# THOR Sample Collector Plugin

## Description

This repository contains a THOR plugin that uploads files that THOR scanned to a remote server.

The server is a simple HTTP server that can be found in the `server/` directory.

## Usage

This plugin is not intended for actual use, but merely as an example of how to
implement a THOR plugin that uploads files to a remote server.

If you want to build your own plugin based on this, you may want to consider:

- Which files should be uploaded? Any files, only files with a certain score,
  only files with a certain file type, files where a custom signature matched, etc.

  _This example uploads all PE files that THOR encounters._
- What metadata should be sent along with the files?

  _This example only sends the file path._
- How should network issues (DNS resolution, connection issues, etc.) be handled? Logging, retries, ...

  _This example simply logs any errors._
