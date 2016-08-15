Mesh Compression Examples
=========================

These are minimal examples of mesh compression techniques that can be decoded on-the-fly on the GPU, thus leading to savings in transmission time, memory footprint, and GPU bus usage.

- [The first example](https://tsherif.github.io/mesh-compression-examples/quantize.html) simply draws two triangles to the screen, one using standard 32-bit floats to represent the positions, and the other with positions quantized to 16-bit unsigned ints, leading to a 50% reduction in size. The technique is described in [Mesh Geometry Compression for Mobile Graphics by Lee, Choe and Lee](http://cg.postech.ac.kr/research/mesh_comp_mobile/mesh_comp_mobile_conference.pdf)

- [The second example](https://tsherif.github.io/mesh-compression-examples/quantize-oct.html) draws two spheres to the screen, one with 32-bit floats representing positions and normals, the other with the positions quantized as above and the normals oct-encoded into 2 bytes. This leads to the same 50% reduction in size for positions and an 83% reduction in size for normals. The oct-encoding technique is described in [A Survey of Efficient Representations for Independent Unit Vectors by Cigolle et al.](http://jcgt.org/published/0003/02/01/).

