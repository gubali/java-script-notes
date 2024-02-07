# java-script-notes
A11y

1) anybody with disabilities or withpout disabilities can access.


tools: screen reader


1) Four priciple (POUR)
  - percevable: open, clear, visible,recognizible
 - operable: usable,functional, useful
 - understanble
 -Robust



1- use alt in img
1- aria-labelledby


ARIA: Accessible Rich Internet Applications

role:
properties: give extra meaning to element

<label for="email">Email</label>
<input type="email" id="email" />

state: aria-disabled="true"
aria-hidden:
name:identifier

aria-label: override the elemrnt name and replacing it with name given by you.

exp: <button aria-label="close" >X</button>

aria-labelledby: override the element name and repalce with content of another name.
<div id"tblLabel">Email</div>
<div id="txtBox" aria-labelledby="tbllabel" id="email"></div>

aria-describedby
<input aria-describedby="a" />
<p id="a">
lore ipsum</p>

nor focusable: -1
0: focusble
1,2,3


WAI(Web accessabiity initiative)-ARIA is a technology that can be used to add extra information about the structure and function of a page.




improve website performance;
 1_ Reduce the Number of HTTP Requests
2) Optimize Image Sizes
3) Use a Content Delivery Network (CDN)
4)  Write Mobile-First Code
5)right hosting paln
6) Minify and Combine CSS, JavaScript, and HTML Files
7) Load JavaScript Asynchronously
8) redue plugin




blocking nature which results in slow loading.

Two boolean attribute: defer and Async
Defer:tells the browser not to wait for the script. Instead, the browser will continue to process the HTML, build DOM.never blcok the page and ecxecute when DOM is ready
 = continue on DOM and script loade parallel
 - script only executed when html parsing fully complete
 
aync:  It is also very useful for loading scripts in the middle of the DOM which are already there.( script will be executed asynchronously when it is available)

  - doesnot gaurentee order of execution


# Event loop program:
$.on('button', 'click', function onClick() {
    setTimeout(function timer() {
        console.log('You clicked the button!');    
    }, 2000);
});

console.log("Hi!");

setTimeout(function timeout() {
    console.log("Click the button!");
}, 5000);

console.log("Welcome to loupe.");





