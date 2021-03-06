# Delta Instructions

Ivy exports a number of functions prefixed with `Δ`, for example `ΔelementStart`, or `Δinject`, et al. These functions are referred to an "instructions" or "delta" instructions. They are functions that are called by code generated by the Ivy compiler that must be publicly exposed in order to be consumed by this generated code. **They are not meant for developer consumption**. The reason they are prefixed with `Δ` is not only to identify them as different from other functions, but also to make them not show up at the top of IDE code completion in environments such as Visual Studio code.


### Guidance

- Do not use `Δ` functions directly. They are meant to be used in generated code.
- Do not create new `Δ` functions, it's not a convention that Angular consumes, and it is liable to confuse other developers into thinking consuming Angular's `Δ` functions is a good pattern to follow.
