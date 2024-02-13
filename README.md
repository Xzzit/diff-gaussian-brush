# Differential Gaussian Rasterization
Used as the rasterization engine for the paper "3D Gaussian Splatting for Real-Time Rendering of Radiance Fields". If you can make use of it in your own research, please be so kind to cite us.


# What's changed?
1. `p_view.z` has been replaced by `p_proj.z` for [frustum culling](./cuda_rasterizer/auxiliary.h#L151) and [depth estimation](./cuda_rasterizer/forward.cu#L249).
2. add `brush_stroke` to `raster_settings`, which is used to activate the brush stroke mode.
3. add `RasterizeGaussiansBrushStrokeCUDA` for brush stroke mode.


<section class="section" id="BibTeX">
  <div class="container is-max-desktop content">
    <h2 class="title">BibTeX</h2>
    <pre><code>@Article{kerbl3Dgaussians,
      author       = {Kerbl, Bernhard and Kopanas, Georgios and Leimk{\"u}hler, Thomas and Drettakis, George},
      title        = {3D Gaussian Splatting for Real-Time Radiance Field Rendering},
      journal      = {ACM Transactions on Graphics},
      number       = {4},
      volume       = {42},
      month        = {July},
      year         = {2023},
      url          = {https://repo-sam.inria.fr/fungraph/3d-gaussian-splatting/}
}</code></pre>
  </div>
</section>