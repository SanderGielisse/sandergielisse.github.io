---
title: "Optical Flow Upsamplers Ignore Details: Neighborhood Attention Transformers for Convex Upsampling"
collection: publications
permalink: 'http://resolver.tudelft.nl/uuid:1e4321eb-4fc0-4e98-8e51-81b891fc8d63'
date: 2023-03-03
venue: 'TU Delft Repository'
paperurl: 'http://sandergielisse.github.io/files/msc_thesis_alexander_gielisse.pdf'
citation: 'A.S. Gielisse. (2023). Master Thesis. TU Delft Repository.'
---

**Abstract**
Most recent works on optical flow use convex upsampling as the last step to obtain high-resolution flow. In this work, we show and discuss several issues and limitations of this currently widely adopted convex upsampling approach. We propose a series of changes, inspired by the observation that convex upsampling as currently implemented performs badly in high-detail areas. We identify three possible causes; wrong training data, the non-existence of a convex combination, and the inability of the convex upsampler to find the correct convex combination.

We propose several ideas in an attempt to resolve current issues. First, we propose to decouple the weights for the final convex upsampler, making it easier to find the correct convex combination. For the same reason, we also provide extra contextual features to the convex upsampler. Then, we increase the convex mask size by using an attention-based alternative convex upsampler; Transformers for Convex Upsampling. This upsampler is based on the observation that convex upsampling can be reformulated as attention, and we propose to use local attention masks as a drop-in replacement for convex masks in order to increase the mask size. We provide empirical evidence that a larger mask size increases the likelihood of the existence of the convex combination. Lastly, we propose an alternative training scheme to remove bilinear interpolation artifacts from the model output.

We investigate whether an increase in accuracy can be achieved while leaving the low-resolution flow prediction architecture unchanged. Due to that, our proposed ideas could theoretically be applied to almost every current state-of-the-art optical flow architecture. On the FlyingChairs + FlyingThings3D training setting we reduce the Sintel Clean training end-point-error of GMA from 1.31 to 1.18, which is a 10% decrease caused solely by changes regarding the convex upsampler.

[Visit TU Delft Library Repository](http://resolver.tudelft.nl/uuid:1e4321eb-4fc0-4e98-8e51-81b891fc8d63)
[Download paper here](http://sandergielisse.github.io/files/msc_thesis_alexander_gielisse.pdf)
