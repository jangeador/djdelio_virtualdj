## Actions

### Piano mode:
```
hot_cue [number] temporary
```

### Roll Pads

```
<map value="ROLL_PAD1" action="loop_roll 0.125" />
<map value="ROLL_PAD2" action="loop_roll 0.25" />
<map value="ROLL_PAD3" action="loop_roll 0.5" />
<map value="ROLL_PAD4" action="loop_roll 1" />
<map value="ROLL_PAD5" action="effect_active &apos;flanger&apos; temporary " />
<map value="ROLL_PAD6" action="effect_active &apos;reverb&apos; temporary &amp; effect_slider &apos;reverb&apos; 1 85% &amp; effect_slider &apos;reverb&apos; 2 100% &amp; effect_slider &apos;reverb&apos; 3 0% &amp; effect_slider &apos;reverb&apos; 4 50% &amp; effect_button &apos;reverb&apos; 1 off &amp; effect_button &apos;reverb&apos; 2 on" />
<map value="ROLL_PAD7" action="effect_active &apos;frenada ajustable 1&apos; temporary" />
<map value="ROLL_PAD8" action="effect_active &apos;slipbrake8&apos; " />
```


### Saved Loops Pads
```
<map value="SAVED_LOOP_PAD1" action="loop ? loop_half : loop 0.5" />
<map value="SAVED_LOOP_PAD2" action="loop 1" />
<map value="SAVED_LOOP_PAD3" action="loop 2" />
<map value="SAVED_LOOP_PAD4" action="loop ? loop_double : loop 4" />
<map value="SAVED_LOOP_PAD5" action="pause ? play &amp; effect &quot;Echo&quot; active off &amp; slip : effect &quot;Echo&quot; active &amp; effect &quot;Echo&quot; slider 1 70% &amp; effect &quot;Echo&quot; slider 2 70% &amp; pause &amp; slip" />
<map value="SAVED_LOOP_PAD6" action="pause ? play &amp; effect &quot;Echo&quot; active off &amp; slip : effect &quot;Echo&quot; active &amp; effect &quot;Echo&quot; slider 1 70% &amp; effect &quot;Echo&quot; slider 2 50% &amp; pause &amp; slip" />
<map value="SAVED_LOOP_PAD7" action="pause ? play &amp; effect &quot;Echo&quot; active off &amp; slip : effect &quot;Echo&quot; active &amp; effect &quot;Echo&quot; slider 1 70% &amp; effect &quot;Echo&quot; slider 2 40% &amp; pause &amp; slip" />
<map value="SAVED_LOOP_PAD8" action="pause ? play &amp; effect &quot;Echo&quot; active off &amp; slip : effect &quot;Echo&quot; active &amp; effect &quot;Echo&quot; slider 1 70% &amp; effect &quot;Echo&quot; slider 2 30% &amp; pause &amp; slip" />
<map value="SHIFT_SAVED_LOOP_PAD1" action="loop 0.125 temporary &amp; effect_active &apos;loopcut&apos; temporary &amp; effect_slider &apos;loopcut&apos; 1 66% &amp; effect_active &apos;keyloopdown&apos; temporary &amp; slip temporary" />
<map value="SHIFT_SAVED_LOOP_PAD2" action="loop 0.25 temporary &amp; effect_active &apos;loopcut&apos; temporary &amp; effect_slider &apos;loopcut&apos; 1 66% &amp; effect_active &apos;keyloopdown&apos; temporary &amp; slip temporary" />
<map value="SHIFT_SAVED_LOOP_PAD3" action="loop 0.5 temporary &amp; effect_active &apos;loopcut&apos; temporary &amp; effect_slider &apos;loopcut&apos; 1 66% &amp; effect_active &apos;keyloopdown&apos; temporary &amp; slip temporary" />
<map value="SHIFT_SAVED_LOOP_PAD4" action="loop 1 temporary &amp; effect_active &apos;loopcut&apos; temporary &amp; effect_slider &apos;loopcut&apos; 1 66% &amp; effect_active &apos;keyloopdown&apos; temporary &amp; slip temporary" />
<map value="SHIFT_SAVED_LOOP_PAD5" action="loop 0.125 temporary &amp; effect_active &apos;loopcut&apos; temporary &amp; effect_slider &apos;loopcut&apos; 1 66% &amp; effect_active &apos;keyloopup&apos; temporary &amp; slip temporary" />
<map value="SHIFT_SAVED_LOOP_PAD6" action="loop 0.25 temporary &amp; effect_active &apos;loopcut&apos; temporary &amp; effect_slider &apos;loopcut&apos; 1 66% &amp; effect_active &apos;keyloopup&apos; temporary &amp; slip temporary" />
<map value="SHIFT_SAVED_LOOP_PAD7" action="loop 0.5 temporary &amp; effect_active &apos;loopcut&apos; temporary &amp; effect_slider &apos;loopcut&apos; 1 66% &amp; effect_active &apos;keyloopup&apos; temporary &amp; slip temporary" />
<map value="SHIFT_SAVED_LOOP_PAD8" action="loop 1 temporary &amp; effect_active &apos;loopcut&apos; temporary &amp; effect_slider &apos;loopcut&apos; 1 66% &amp; effect_active &apos;keyloopup&apos; temporary &amp; slip temporary" />

```

### Saved Loops Leds

```
<map value="LED_SAVED_LOOP_PAD1" action="loop 0.5 ? blink 700ms ? constant &apos;green&apos; :: loop 0.25 ? blink 300ms ? constant &apos;green&apos; :: loop 0.125 ? blink 300ms ? constant &apos;green&apos; :: loop 0.0625 ? blink 300ms ? constant &apos;green&apos; :: loop 0.03125 ? blink 300ms ? constant &apos;green&apos; :: constant &apos;green&apos;" />
<map value="LED_SAVED_LOOP_PAD2" action="loop 1 ? blink 700ms ? constant &apos;green&apos;  :: constant &apos;green&apos;" />
<map value="LED_SAVED_LOOP_PAD3" action="loop 2 ? blink 700ms ? constant &apos;green&apos;  :: constant &apos;green&apos;" />
<map value="LED_SAVED_LOOP_PAD4" action="loop 4 ? blink 700ms ? constant &apos;green&apos; :: loop 8 ? blink 300ms ? constant &apos;green&apos; :: loop 16 ? blink 300ms ? constant &apos;green&apos; :: loop 32 ? blink 300ms ? constant &apos;green&apos; :: loop 64 ? blink 300ms ? constant &apos;green&apos;  :: constant &apos;green&apos;" />
<map value="LED_SAVED_LOOP_PAD5" action="effect_active &apos;echo&apos; ? constant &apos;blue&apos; : constant &apos;white&apos;" />
<map value="LED_SAVED_LOOP_PAD6" action="effect_active &apos;echo&apos; ? constant &apos;blue&apos; : constant &apos;white&apos;" />
<map value="LED_SAVED_LOOP_PAD7" action="effect_active &apos;echo&apos; ? constant &apos;blue&apos; : constant &apos;white&apos;" />
<map value="LED_SAVED_LOOP_PAD8" action="effect_active &apos;echo&apos; ? constant &apos;blue&apos; : constant &apos;white&apos;" />
<map value="SHIFT_LED_SAVED_LOOP_PAD1" action="blink 500ms ? constant &apos;orange&apos; : off" />
<map value="SHIFT_LED_SAVED_LOOP_PAD2" action="blink 500ms ? constant &apos;orange&apos; : off" />
<map value="SHIFT_LED_SAVED_LOOP_PAD3" action="blink 500ms ? constant &apos;orange&apos; : off" />
<map value="SHIFT_LED_SAVED_LOOP_PAD4" action="blink 500ms ? constant &apos;orange&apos; : off" />
<map value="SHIFT_LED_SAVED_LOOP_PAD5" action="blink 500ms ? constant &apos;orange&apos; : off" />
<map value="SHIFT_LED_SAVED_LOOP_PAD6" action="blink 500ms ? constant &apos;orange&apos; : off" />
<map value="SHIFT_LED_SAVED_LOOP_PAD7" action="blink 500ms ? constant &apos;orange&apos; : off" />
<map value="SHIFT_LED_SAVED_LOOP_PAD8" action="blink 500ms ? constant &apos;orange&apos; : off" />
<map value="SAVED_LOOP_PARAM-" action="pad_param -1" />
<map value="SAVED_LOOP_PARAM+" action="pad_param +1" />
<map value="SHIFT_SAVED_LOOP_PARAM-" action="pad_param2 -1" />
<map value="SHIFT_SAVED_LOOP_PARAM+" action="pad_param2 +1" />
```

### Quick Mix
```
<map value="SAMPLER_VEL_PAD1" action="device_side &apos;left&apos; ? &amp; deck left hot_cue 1 &amp; deck right cue_stop : deck right hot_cue 1 &amp; deck left cue_stop " />
<map value="SAMPLER_VEL_PAD2" action="device_side &apos;left&apos; ? deck left hot_cue 2 &amp; deck right cue_stop : deck right hot_cue 2 &amp; deck left cue_stop" />
<map value="SAMPLER_VEL_PAD3" action="device_side &apos;left&apos; ? deck left hot_cue 3 &amp; deck right cue_stop : deck right hot_cue 3 &amp; deck left cue_stop" />
<map value="SAMPLER_VEL_PAD4" action="device_side &apos;left&apos; ? deck left hot_cue 4 &amp; deck right cue_stop : deck right hot_cue 4 &amp; deck left cue_stop" />
<map value="SAMPLER_VEL_PAD5" action="device_side &apos;left&apos; ? deck left hot_cue 5 &amp; deck right cue_stop : deck right hot_cue 5 &amp; deck left cue_stop" />
<map value="SAMPLER_VEL_PAD6" action="device_side &apos;left&apos; ? deck left hot_cue 6 &amp; deck right cue_stop : deck right hot_cue 6 &amp; deck left cue_stop " />
<map value="SAMPLER_VEL_PAD7" action="device_side &apos;left&apos; ? deck left hot_cue 7 &amp; deck right cue_stop : deck right hot_cue 7 &amp; deck left cue_stop " />
<map value="SAMPLER_VEL_PAD8" action="device_side &apos;left&apos; ? deck left hot_cue 8 &amp; deck right cue_stop : deck right hot_cue 8 &amp; deck left cue_stop" />

```