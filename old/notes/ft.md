Since each harmonic (frequency bin) is independent,
perform a row-wise fourier transform on the NxK matrix.

In higher dimensions, you only care about the "top two" dimensions (the front face), 
i.e. the sequence dimension (N) and the previous frequency dimension (K)

Treat all lower dimensions as "scalars", since they are just values.
That is, don't perform any transform on their values.
Therefore, you're only performing the row-wise fourier transform on the "top face."

Hopefully, this results in invertibility?


If two trajectories map to the same symbol, they should be close together.
It doesn't mean they are the same or equivalent.
