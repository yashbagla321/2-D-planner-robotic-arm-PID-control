%% setting frames speed
d=2;
j=1:d:length(T);
%% generating images in 2D
figure
for i=1:length(j)-1
 hold off
 plot([y1(j(i))*2 yee(j(i))], [x1(j(i))*2 xee(j(i))], 'o',[0 y1(j(i))*2],[0 x1(j(i))*2], 'k',[y1(j(i))*2 yee(j(i))],[x1(j(i))*2 xee(j(i))],'k')
 title('Motion of 2DOF Robotic Arm')
 xlabel('x')
 ylabel('y')
 axis([-3 3 -3 3]);
 grid
 hold on
 MM(i)=getframe(gcf);
end
drawnow;
%% exporting to 'mpg' movie
mpgwrite(MM,'RGB','2DOF_rob.mpg')
