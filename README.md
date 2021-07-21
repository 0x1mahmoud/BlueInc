# BlueInc
## CyberTalents BlueInc web security challenge writeup

**Challenge Description**
Blue Inc is a new social media website that's still under construction, However it doesn't have registration yet, but if you are interested in seeing our website then you can login with **demo/demo.**

so let's click the challenge link ` http://35.240.62.111/blue_inc/chal1/ `

so now click on login in the top right of page 

![Image of mahmoudashraf1344](https://github.com/mahmoudashraf1344/BlueInc.md/blob/main/login.png)

<br/>
<h3>it will take you to login page so set the <h2>username: demo and password= demo</h2> as they told us in **Challenge Description**</h3>
<br/>

![Image of mahmoudashraf1344](https://github.com/mahmoudashraf1344/BlueInc.md/blob/main/login1.png)

<h3>after that make sure that you open the proxy and Burp Suite to see the http request and response</h3>

![Image of mahmoudashraf1344](https://github.com/mahmoudashraf1344/BlueInc.md/blob/main/test.png)

as you can see we have Successfully logged in! so let's see something is more interesting

![Image of mahmoudashraf1344](https://github.com/mahmoudashraf1344/BlueInc.md/blob/main/test2.png)

we see there that `Cookie: user=demo` so let's think creativity we need the ADMIN we need the privilege escalation

oki let's see the last one

![Image of mahmoudashraf1344](https://github.com/mahmoudashraf1344/BlueInc.md/blob/main/test2.png)
 
we see there `user=demo` and also `Cookie: user=demo` so let's test by setting "admin" without setting "demo"
 
![Image of mahmoudashraf1344](https://github.com/mahmoudashraf1344/BlueInc.md/blob/main/test3.png)
 
so let's type `user=admin` and also `Cookie: user=demo`
 
![Image of mahmoudashraf1344](https://github.com/mahmoudashraf1344/BlueInc.md/blob/main/test4.png)

<h2>now check of the Response in Burp and you'll see the Flag<h2>
<h1>Good Luck all...<h1>
