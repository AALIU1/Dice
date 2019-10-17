dice die;
int t=0;
int total=0;
int tx=890;
int ty=120;
void setup()
{
  size(2000,1000);
  die = new dice(100,150);
  noLoop();
}
void mousePressed(){
  redraw();
  total=0;
}
void draw(){
  die.ax=100;
  die.ay=150; 
  background(0,150,0);
  stroke(0,0,0);
  for(int z=0;z<=7;z++){
      for(int i=0;i<=16;i++){
        die.num=(int)(Math.random()*6+1);
        die.a=(int)(Math.random()*200+56);
        die.b=(int)(Math.random()*200+56);
        die.c=(int)(Math.random()*200+56);
        die.show();
        die.ax+=100;
        total=total+die.num;
      } 
      die.ax=100;
      die.ay+=100;
    }
  fill(0,0,0);
  textSize(100);
  text(total,tx,ty);
  if(t>=1){
    t+=1;
  }
  if(t>20){
    t=0;
  }
  noStroke();
  fill(139,69,19);
  rect(0,0,30,1100);
  rect(0,0,2200,30);
  rect(1905,0,30,1100);
  rect(0,970,2200,30);
}
class dice
{
  float ax;
  float ay;
  int num;
  int a,b,c;
  dice(int x, int y){
    ax=x;
    ay=y;
    num=(int)(Math.random()*6+1);
    a=(int)(Math.random()*200+56);
    b=(int)(Math.random()*200+56);
    c=(int)(Math.random()*200+56);
  }
  void show(){
    strokeWeight(10);
    fill(a,b,c);
    rect(ax,ay,100,100,20);
    if(num==1){
      strokeWeight(20);
      line(ax+50,ay+50,ax+50,ay+50);
    }
    if(num==2){
      strokeWeight(20);
      line(ax+25,ay+25,ax+25,ay+25);
      line(ax+75,ay+75,ax+75,ay+75);
    }
    if(num==3){
      strokeWeight(20);
      line(ax+25,ay+25,ax+25,ay+25);
      line(ax+50,ay+50,ax+50,ay+50);
      line(ax+75,ay+75,ax+75,ay+75);
    }
    if(num==4){
      strokeWeight(20);
      line(ax+25,ay+25,ax+25,ay+25);
      line(ax+75,ay+25,ax+75,ay+25);
      line(ax+25,ay+75,ax+25,ay+75);
      line(ax+75,ay+75,ax+75,ay+75);
    }
    if(num==5){
      strokeWeight(20);
      line(ax+25,ay+25,ax+25,ay+25);
      line(ax+75,ay+25,ax+75,ay+25);
      line(ax+25,ay+75,ax+25,ay+75);
      line(ax+75,ay+75,ax+75,ay+75);
      line(ax+50,ay+50,ax+50,ay+50);
    }
    if(num==6){
      strokeWeight(20);
      line(ax+25,ay+25,ax+25,ay+25);
      line(ax+75,ay+25,ax+75,ay+25);
      line(ax+25,ay+75,ax+25,ay+75);
      line(ax+75,ay+75,ax+75,ay+75);
      line(ax+25,ay+50,ax+25,ay+50);
      line(ax+75,ay+50,ax+75,ay+50);
    }
  }
}
