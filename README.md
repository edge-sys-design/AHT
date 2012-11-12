# AHT

This is code specific to the AHT series of radios. This is upstream to the
public developer API -- the API itself calls functions which are implemented
here, and functions implemented here are expected to be as consistent as
possible among all of the AHT lineup, and preferably all Android radios.

Every model (and upcoming models) will be branched.

`master` is code that will be branched for the next upcoming release.
`AHT-#` is code that has already been branched, and already appears, or is
about to appear in a current release.

This means that when the AHT-1 is about to be released, master will get
branched to AHT-1. Commits to master will then go toward AHT-2. Patches can, of
course, be merged from master back into AHT-1, if they are found necessary for
AHT-1.

This lets us keep a constant/raw moving target (`master`) and still have
stability when we need it most. Releases are tagged with `#.y.z` where
`y.z` follow the same `y.z` from [semver](http://semver.org/).

Ideally master will be kept in a working state, but don't expect it to be
as stable as a branched release.

**Note:** `master` of this branch and `master` of the public developer API
should remain in-sync, and the public developer API should remain backwards
compatible to the end user. This means that the API should detect which version
of AHT is being used, if it needs to, in a transparent way.

# Licensing

This repository, and code within, is released under the GPL version 2 or, at
your option, any later version (GPLv2+).
