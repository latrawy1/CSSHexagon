# CSSHexagon

## Introduction

as we all know, items in html is formed in rectangle. it is obvious that our computer can not recongize shapes other than rectangle. so
when i see the demo picture (which is alse put at the root folder), i think why i can not create components in shapes of Hexagon while 
somebody else have realize it.
it is quite insteresting in doing researching on it. i hope we all enjoy the procedure

## solutions
after serveral days of jods,i found some solutions 

### take advantage of border
if you set the width of border to a big value, you can create  hypotenuses. when the content is 0 * 0 , all your borders will be 
triangles. if you hide some of them ,you can get an triangle. if you put two triangles beside a rectangle,you may get a hexagon.

you can find more info in https://jtauber.github.io/articles/css-hexagon.html

this is sufficient in creating a single color hexagon. but you can not control the behaviour of borders ,e.g  if you want to show a img

### use overflow:hidden
it uses serveral embedded div. we rotate them step by step. at last we get an visiable area in Hexagon  

this is also very interesting in using this method. this gives me new ideas. i make a demo of this named [index1.html] at the root folder

some disadvantages: 
  some edges are tough
  can not add borders

### take advantage of overflow area
it also uses serveral embedded div. the difference between this and the former one is it use div to ocuppy an area to create a 
Hexagon.
we use background:inherited   to inherit the background and make it looks like one component.
(small tips we use :before and z-index to clear the evidence of div's rotation)

it make a demo called [index2.html] at the root folder

## Future
it is hard for i to do further research. but i will try my best to realize the effect in demo.jpg
