
## tdf

* 


## code

```
#ifdef GL_ES
precision mediump float;
#endif

#extension GL_OES_standard_derivatives : enable

uniform float time;
uniform vec2 mouse;
uniform vec2 resolution;

void main( void ) {
	vec2 position = (( gl_FragCoord.xy / resolution.xy ) - 0.5) * 5.0;
	float wave = sin(position.x * time * 10.0);
	gl_FragColor = vec4(vec3(wave, wave * position.y, position.x * wave),  1.0);
}
```


