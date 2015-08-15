# ErasureCodes
A Javascript implementation of Reed-Solomon erasure codes. This library is optimised for, and operates on, large Uint8Arrays. To include, simply add erasure.js to your project, and call the *split*, and *recombine* methods. The recombine method assume the fragments are in the same order as they were initially after encode. 

A browser benchmark demonstrating erasure encoding and decoding is at:
http://ianopolous.github.io/ErasureCodes/erasure.html

In this, a 5 MiB file is split into 40 fragments, and an additional 20 fragments are generated. Then the decode is tested with 0 - 10 missing fragments. 
