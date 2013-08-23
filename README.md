gjrGARCH.jl
================

[![Build Status](https://travis-ci.org/JuliaStats/Distributions.jl.png)](https://travis-ci.org/JuliaStats/Distributions.jl)

## Quick Review of the package

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris aliquet mattis odio vitae bibendum. Suspendisse hendrerit malesuada nibh. Sed ac lacinia est, quis adipiscing orci. Pellentesque habitant morbi tristique senectus et netus et malesuada fames ac turpis egestas. Duis dignissim quam sit amet fringilla faucibus. Integer a laoreet lacus. Suspendisse eget feugiat nibh. Fusce commodo at dui eget ornare. Praesent vitae sem mauris.

Donec dapibus est vel nibh facilisis accumsan ac ac odio. Vivamus dolor lectus, aliquet et facilisis eget, congue sit amet ipsum. Nam adipiscing viverra est vitae condimentum. Quisque vitae erat quis neque accumsan placerat. Etiam tellus augue, ultricies vel ullamcorper nec, porta in sem. Nulla consequat, quam at congue pulvinar, risus ipsum adipiscing elit, vitae tincidunt ante nunc ac neque. Proin ultricies mi nunc, sed placerat dui consequat et. Suspendisse augue erat, placerat vel tortor eget, lacinia accumsan magna. Pellentesque ut turpis id mauris vehicula elementum. Mauris interdum ipsum ut nisl volutpat, ut facilisis elit mollis.

## Example

```julia
using gjrGARCH, Quandl
quotes = quandl("YAHOO/INDEX_GSPC")
ret = diff(log(quotes["Close"]))*100
returns=convert(Vector,ret[1:1000]);
@time GJRGARCHged(returns);
```


