# GLSL tech study in TECH LAB PAAK

```
#ifdef GL_ES
precision mediump float;
#endif

uniform float time;
uniform vec2 mouse;
uniform vec2 resolution;

#define PI 3.14159

void main(void){
    vec2 p = (gl_FragCoord.xy - resolution) / min(resolution.x, resolution.y);
    gl_FragColor = vec4(p, 0.0, 1.0);
}
```
