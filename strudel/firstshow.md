# my first live coding show!

```
// ᓚᘏᗢ
cpm (100/4) 

$: s("c").s("brown").gain(.7).pan(-3).gain(slider(4, 0, 10, 1))
$: s("1").s("gm_seashore").gain(.7).pan(3).gain(slider(4, 0, 10, 1))
$: s("1").s("crackle").gain(.9).pan(3).gain(slider(0, 0, 10, 1))

$: note(`<
[ab1 eb3 c3 eb ab1 eb3 bb3 eb]
[ab1 eb3 c3 g3 ab1 eb3 c3 f3]
[f1 eb3 f3 g3 ab1 eb3 f3 g3]
>`).scale("<eb5:minor gb5:major>/2").s("piano").room(1).gain(.9).pan(-5)
.lpf(slider(759, 0, 1000, 1)).hpf(slider(404, 0, 1000, 1)).scaleTranspose(3).gain(slider(1, 0, 2, 1))

// $: n("0 [4 <3 2>] <2 3> [~ 1]"
// .off(1/16, x=>x.add(4))
// //.off(1/8, x=>x.add(7))
// ).scale("<eb5:minor gb5:major>/2")
// .s("triangle").room(.5).dec(.1)
// .gain(.2).pan(4)
// .scaleTranspose(3)

// $: note("eb1*16").transpose(irand(36)).scale("<eb5:minor gb5:major>/2")
//   .lpf(slider(583, 0, 1000, 1)).hpf(slider(583, 0, 1000, 1)).gain(slider(1, 0, 10, 1)).scaleTranspose(3)

// $: s("saw").seg(16).n(irand(12)).scale("eb1:minor")
// .penv(48).panchor(0).pdec(0.05)
// .delay(0.25).room(0.25)
// .compressor(-20).vib(0.3)
// .partials(randL(200))
// .phases(randL(200)).gain(slider(0.15, 0, 5, 1))

// samples('github:bubobubobubobubo/dough-waveforms')
// $: note("eb2*8").s("wt_dbass").n(run(8))
// .lpenv(-3).lpa(.1).room(.5).fast(2).gain(slider(1, 0, 5, 1))

// samples('github:switchangel/pad')
// $: s("swpad:0").scrub("{0.1!2 .25@3 0.7!2 <0.8:1.5>}%8").scale("<eb2:minor c2:minor bb1:major>/2").gain(slider(0, 0, 5, 1))

// $: sound("- rim").bank("RolandTR707").room(.6).delay(".2").rev().gain(.4)
// $: sound("bd -").bank("RolandTR707").room(.2).delay(".2").rev().gain(.4)
// $: n("0 2 [4 2] 3*2").sound("jazz").gain(.2).rev()
// $: sound("hh*16").gain("[.25 1]*4").gain(0.05)
// $: sound("bd*4,[~ sd:1]*2").gain(0.0)

// $: note("eb4").s("gm_fx_atmosphere").gain(slider(0.2, 0, 5, 1))

// $: note(`<
// [f6 f6 f6 f6 f6 f6]
// [db6 db6 db6 db6 db6 db6]
// [bb5 bb5 bb5 bb5 bb5 bb5]
// [eb6 eb6 eb6 eb6 eb6 eb6]
// [ab6 ab6 ab6 ab6 ab6 ab6]
// >`).s("piano")
```