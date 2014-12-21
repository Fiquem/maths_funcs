Minimal maths functions header for 3d graphics.
Functions designed to resemble GLSL and GLUT.
Column-major matrix operations and memory layout.

## data types ##

* vec2
* vec3
* vec4
* mat3
* mat4
* versor (quaternion)

Data is stored in simple 1d arrays of floats inside data types. I didn't bother
with messy recreation of myvector.x access.

To access the x component of a vector:

    vec2 v = vec2 (1.0f, 0.0f, 0.0f);
    float x = v.v[0];

To access the row 0, col 1 of a 4X4 matrix:

    float f = my_matrix.m[4];

## functions ##

* overloaded basic mathematical and assignment operators for data types
* print() for each data type (contents)
* vector length, squared length, normalisation, dot and cross products
* some converstions between direction vectors and angles
* matrix identity, inverse, determinant, transpose
* affine matrix construction
* virtual camera matrix construction in GLUT format (look at etc.)
* quaternion construction from axis-angle
* versor to matrix
* slerp (spherical interpolation)
