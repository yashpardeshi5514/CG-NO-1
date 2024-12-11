#include<stdio.h>
#include<graphics.h>
int main()
{
int x1=200,y1=100,x2=100,y2=200,gd=DETECT,gm,dx,dy,steps,i,x,y;
initgraph(&gd,&gm,NULL);
dx=(x2-x1);
dy=(y2-y2);
if(dx>dy)
steps=dx;
else
steps=dy;
dx=dx/steps;
dy=dy/steps;
x=x1,x=y1,i=1;
while(i<=steps)
{
putpixel(x,y,RED);
x=x+dx;
y=y+dy;
i=i+1;
delay(100);
}
getch();
return 0;
}
