- 👋 Hi, I’m @set59
- 👀 I am interested in the factorization of numbers using the COLLATZ hypothesis
- Let l, m be prime numbers, x(1)=l*m. if x(1)=2*k then x(2) =x(1) /2 else x(2) =(x(1) *3+1)/2 and these COLLATZ numbers are direct. if (x(1)*2-1) MOD 3=0 then x(-1) =(x(1) *3+1)/2 else x(-1) =x(1))/2 and these COLLATZ numbers are inverse. I believe that among the direct and inverse COLLATZ numbers, there are such that x(i)^2 MOD X(1)=k^2, then (x(i)+-k) MOD l=0 and (x(i)+-k) MOD m=0. The factorization of numbers takes place in a reasonable time. Example: x(1)=l*m=209=11*19; Then the direct Collatz numbers are 314, 157, 236,118, 58, ......... and the reverse ones are 139, 278, 185, 123. So 157^2 MOD 209 = 14^2 then (157-14) MOD 11 =0 and (157+14) MOD 19 =0, also 123^2 MOD 209 = 9^2 then (123-9) MOD 19=0 and (1237+9) MOD 11 =0.
- 💞️ I want to cooperate further on this topic, I ask for help.
- program COLLATZ;
Var 
x,m,n,p,l,r,s:UInt64; 
label 1,2;
begin
x:=359*487;
m:=x;
s:=0;
repeat
p:=trunc(x/2);
if odd(x) = true then
p:=trunc((x*3+1)/2);
x:=p;
if sqr(x)<=m then goto 2;
n:=sqr(x) mod m;
r:=trunc(sqrt(n));
l:=n-trunc(sqr(r));
s:=s+1;
if l=0 then goto 1;
2:
until  x=1;
1:
writeln (n,' = ',r,' = ',x,' = ',s);
end.

- 📫 How to contact me, my email address: serar2022@mail.ru , serar59@mail.ru

<!---
set59/set59 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
