E {
  transform: skewx(160deg) skewy(-160deg); x轴受力后，y轴受力
}
E {
  transform: skewx(160deg, -160deg); 这是一个矩形，x轴，y轴同时受力
  同时基于前一个坐标系。
}
不相同，后一个函数会乘以前一个函数的结果。
transform：translate（100px） rotate（30deg） translate（150px） rotate（-60deg）；
transform： translate（50px， 60px）；
transform：rotate（30deg） translate（150px） rotate（-60deg）；