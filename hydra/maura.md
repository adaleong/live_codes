

speed = 1
src(o0).modulate(noise(3),0.005).blend(shape(4),0.01)
gradient([135, 159, 214])
  .mult(osc(3,0.5,8))
  .modulateRepeat(osc(10), 3.0, 3.0, 0.5, 0.5)
.kaleid(50)
.color(43, 52, 74)
.pixelate(20,20)
.out(o0)




speed = 0.1
shape(20,0.2,0.3)
.color(0.5,0.8,50)
  .scale(() => Math.sin(time)+1*2)
  .repeat(() => Math.sin(time)*10)
  .modulateRotate(o0)
  .scale(() => Math.sin(time)+1 *1.5)
  .modulate(noise(2,2))
  .rotate(1, .2)
// .pixelate(100,100)
// .mult(osc(4,0.25,1))
//   .modulateRepeatY(osc(10), 5.0, ({time}) => Math.sin(time) * 5)
//   .scale(1,0.5,0.05)
.out(o0)



shape(20,0.1,0.01)
  .scale(() => Math.sin(time)*3)
  .repeat(() => Math.sin(time)*10)
  .modulateRotate(o0)
  .scale(() => Math.sin(time)*2)
  .modulate(noise(2,0))
  .rotate(0.1, 0.9)
//.brightness( () => Math.sin(time) )

// src(o0)
// .modulate(osc(500,0,0))
// .out(o1)

src(o1)
// .modulateKaleid(voronoi(() => Math.sin(time)*3,0.1,0.01),() => Math.sin(time)*3)
// .scale(() => Math.sin(time)*3)
.out(o2)




s0.initImage("https://images.unsplash.com/photo-1724423942786-e83a6b1a4351?q=80&w=1036&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D")
src(s0).modulate(noise(3))//.kaleid(()=>6+Math.sin(time)*4)
//.pixelate(20,20)

// .kaleid(50).kaleid(9)

// .modulate(osc(25,0.1,0.5))
//             .kaleid(50)
//             .scale(({time})=>Math.sin(time*0.1)*0.2+0.2)
//             .modulate(noise(0.2,0.2,0.5))

// .pixelate(200,200)
// .modulateScrollY(osc(10),0.5,0)

// .luma(0.5,0.1)
// .modulateScale(osc(4,-0.5,0).kaleid(50).scale(0.5),15,0)

// 
 .out(o0)
