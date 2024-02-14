# matlab


I did earlier matlab code that was more involved with genetics; however, I do not have a license.  So, this is just doing some quick demos using an available online Matlab code editor and  tricking it to display graphs.
&nbsp;

I apologize for not having more scientific data feeding into these examples; but, I have done that.
&nbsp;

<img width="402" alt="matlab_001" src="https://github.com/programweb/matlab/assets/12736699/fd3b46de-4ece-41fc-9f0b-60b88115fb7a">
&nbsp;

Above:
```matlab
function y = plotWithSinForY(x)
   y = sin(x);
   plot(x, y), xlabel('x'), ylabel('Sin(x)'), title('Sin(x) Graph'),
   grid on, axis equal
end

plotWithSinForY([0:0.01:7])
```
&nbsp;

<img width="402" alt="matlab_002" src="https://github.com/programweb/matlab/assets/12736699/db54a9f9-6e3f-4ba5-822d-ab37b9eab7a9">
&nbsp;

Above:
```matlab
a = [0:0.5:5];
b = 2*a.^3 + 2*a -5;
plot(a,b)
```
&nbsp;

<img width="363" alt="matlab_003" src="https://github.com/programweb/matlab/assets/12736699/e97bcfb8-b575-48c4-a7ad-d5f94ba5ad52">
&nbsp;

Above:
```matlab
a = [0:0.5:5];
b = 2*a.^3 + 3*a -5;
c = 1.5*a.^2+7*a-3;
subplot(1,2,1)
plot(a,b,'-or','MarkerFaceColor','g','LineWidth',2)
xlabel('X'); ylabel('Y'); legend('Curve ','Location','NorthWest')
subplot(1,2,2)
plot(a,c,'--ok','MarkerFaceColor','c','LineWidth',2)
xlabel('X'); ylabel('Y'); legend('Curve 2','Location','NorthWest')
```
&nbsp;

<img width="393" alt="matlab_004" src="https://github.com/programweb/matlab/assets/12736699/9d98212b-f7a3-4d98-9729-c343384594c3">
&nbsp;

Above:
```matlab
x = -2:.1:2;
y = -2:.5:2;
z = -2:.9:2;

[x,y,z] = meshgrid(x,y,z);
v = x.*exp(-x.^2-y.^2-z.^2);

xslice = [-1.2,.8,2];    % location of y-z planes
yslice = 2;              % location of x-z plane
zslice = [-2,0];         % location of x-y planes

slice(x,y,z,v,xslice,yslice,zslice)
xlabel('x')
ylabel('y')
zlabel('z')
```
&nbsp;

<img width="400" alt="matlab_005" src="https://github.com/programweb/matlab/assets/12736699/5229aa45-2aad-4d12-9e66-53d50a271569">
&nbsp;

Above:
```matlab
z = peaks(33);

figure
mesh(z)
```
&nbsp;

<img width="403" alt="matlab_006" src="https://github.com/programweb/matlab/assets/12736699/7264c648-fa26-465a-86f4-86d055a59f97">
&nbsp;

Above:
```matlab
xd=linspace(-1,1);
yd=linspace(0,2*pi);
[x,y]=meshgrid(xd,yd);
z=x.*cos(y);
mesh(x,y,z) 
```
&nbsp;

<img width="404" alt="matlab_007" src="https://github.com/programweb/matlab/assets/12736699/2e78bbbb-6c2b-434f-84dc-ecfa29a0b392">
&nbsp;

Above:
```matlab
[x,y] = peaks(10);
z =[(x.^3)-(y.^4)];
ribbon(z);
title('\bf Multiple Ribbons')
```
&nbsp;

