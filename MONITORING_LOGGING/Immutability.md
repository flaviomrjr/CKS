IMMUTABILITY
============

securityContext
  readOnlyRootFilesystem: true

And then add enptyDir volumes where this pod needs to write

Good practice disable the privileged option
`privilaged: false`