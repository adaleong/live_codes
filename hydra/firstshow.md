//s0.initImage("https://media.istockphoto.com/id/165685282/vector/water-surface-vector-painting-background.jpg?s=612x612&w=0&k=20&c=GiHO5vnpfNYZEk5Y1G3gj4Du6boamCwXPgYEYf9QiS4=")
//src(s0).modulate(noise(3)).kaleid(()=>6+Math.sin(time)*4)

 s0.initImage("https://static.wixstatic.com/media/18b291_72360286fbda4489a1050259f4a110eef000.jpg/v1/fill/w_2170,h_1190,al_c,q_90,usm_0.66_1.00_0.01,enc_avif,quality_auto/18b291_72360286fbda4489a1050259f4a110eef000.jpg")
src(s0).modulate(noise(3))//.kaleid(()=>6+Math.sin(time)*4)


//.kaleid(50).kaleid(9)

//.modulate(osc(25,0.1,0.5))
 //            .kaleid(50)
//             .scale(({time})=>Math.sin(time*0.1)*0.2+0.2)
//             .modulate(noise(0.2,0.2,0.5))

.pixelate(200,200)
.modulateScrollY(osc(10),0.5,0)

// .luma(0.5,0.1)
// .modulateScale(osc(4,-0.5,0).kaleid(50).scale(0.5),15,0)
// .color(1, 2, 3)

// 
 .out(o0)