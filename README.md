Bevy [Example Extended Material](https://github.com/bevyengine/bevy/blob/release-0.13.1/assets/shaders/extended_material.wgsl) with additional parameters

Currently this will crash and cause a binding error `cargo run`
```
wgpu error: Validation Error

Caused by:
    In Device::create_render_pipeline
      note: label = `pbr_opaque_mesh_pipeline`
    Error matching ShaderStages(FRAGMENT) shader requirements against the pipeline
    Shader global ResourceBinding { group: 2, binding: 100 } is not available in the pipeline layout
    Buffer structure size 8, added to one element of an unbound array, if it's the last field, ended up greater than the given `min_binding_size`
```
