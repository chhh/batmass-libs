# BatMass Libs
The set of libraries used in [BatMass](https://github.com/chhh/batmass).  

All libraries are wrapped into NetBeans _Library Wrapper Modules_ for use with NetBeans Platform applications. Specification version of the module corresponds to the version of the wrapped library where possible.  

## Important
If you're developing something for BatMass, try to never add wrapped libraries directly to your modules, instead:

- Wrap each library in a _Library Wrapper Module_.
- Go to the wrapper module's `Properties -> API Versioning` and mark needed packages as _public_. You'll likely want to make all the packages in a library public, not select ones.
- If you update to a newer version of the library, bump up the specification version of the wrapping module.
- From your module set the dependency on the library wrapping module.
