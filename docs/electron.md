# Octant as an Electron application

Octant is migrating to an Electron application. This document provides
information on design and how to run the application in development
mode.

## Running

Octant is still primarily a browser-based application. To run the
Electron application, the Angular frontend must be running first.

`$ go run build.go build-electron-dev`

An application will be generated in `cmd/octant-electron/output`. Currently,
the application is configured to proxy the frontend to a separately running
Angular frontend (at 127.0.0.1:4200).