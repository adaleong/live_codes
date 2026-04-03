# ONE · · ────── ꒰ঌ·✦·໒꒱ ────── · ·

speed=1 // speed >
shape(99,.15,.5).color(2,1,2)

//.pixelate(100,100) //  3

.diff( shape(900,.5,0).scrollX(.05).rotate( ()=>time/10 ).color(2,0,.75) )
.diff( shape(900.4,.002).scrollX(.10).rotate( ()=>time/20 ).color(2,0,.75) )
.diff( shape(900,.3,.002).scrollX(.15).rotate( ()=>time/30 ).color(4,0,.75) )
.diff( shape(900,.2,.002).scrollX(.20).rotate( ()=>time/40 ).color(4,0,.75) )
.diff( shape(900,.1,.002).scrollX(.25).rotate( ()=>time/50 ).color(5,0,.75) )

.modulateScale(
  shape(240,.5,0).scrollX(.05).rotate( ()=>time/20 )
  , ()=>(Math.sin(time/3)*.2)+.2 )

//.modulate(noise(3),0.005).blend(shape(4),0.01) // 1

// .pixelate(80,80) // 2

.scale(1.6,.6,1)
.out()


# TWO · · ────── ꒰ঌ·✦·໒꒱ ────── · ·

speed = 0.1
shape(20,0.2,0.3)
  
  .color(2,0,.75)
// 	.color(2,1,2)
// .color(2,0,.75)
// .color(4,0,.75)
// .color(4,0,.75)
// .color(5,0,.75)


  .scale(() => Math.sin(time)+1*2)
  .repeat(() => Math.sin(time)*10)
  .modulateRotate(o0)
  .scale(() => Math.sin(time)+1 *1.5)
  .modulate(noise(2,2))
  .rotate(1, .2)

//.pixelate(100,100)

.out(o0)

# THREE · · ────── ꒰ঌ·✦·໒꒱ ────── · ·

s0.initImage("https://images.unsplash.com/photo-1724423942786-e83a6b1a4351?q=80&w=1036&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D")
src(s0).modulate(noise(3))//.kaleid(()=>6+Math.sin(time)*4)
.pixelate(20,20)

.kaleid(50).kaleid(9)
.modulate(osc(25,0.1,0.5))
            .kaleid(50)
            .scale(({time})=>Math.sin(time*0.1)*0.2+0.2)
            .modulate(noise(0.2,0.2,0.5))

// .pixelate(200,200)
// .modulateScrollY(osc(10),0.5,0)

// .luma(0.5,0.1)
// .modulateScale(osc(4,-0.5,0).kaleid(50).scale(0.5),15,0)


 .out(o0)



## FOURRRRR 

speed = 0.1
shape(20,0.2,0.3)
  
  .color(2,0,.75)
// 	.color(2,1,2)
// .color(2,0,.75)
// .color(4,0,.75)
// .color(4,0,.75)
// .color(5,0,.75)


.repeat(2,2)
.modulateScale(osc(3,0.5),-0.6)
.add(o0,0.5)
.scale(0.9)

.out(o0)

