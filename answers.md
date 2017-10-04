

1.  document.querySelector("img")
<img src=​"images/​self-portrait-grassbg.jpg" alt=​"Self Portrait" title=​"Self Portrait" class=​"profile-image">​

images = document.querySelectorAll('img')

document.querySelector("img")

profileImage = images[0]
profileImage.src = "http://www.clubpimble.com/uploads/headings_8619_69773.jpeg"
"http://www.clubpimble.com/uploads/headings_8619_69773.jpeg"


2.  heading = document.querySelector('h1')
<h1 class=​"highlight">​Panda The Bear​</h1>​
heading
<h1 class=​"highlight">​Panda The Bear​</h1>​
heading.innerText = "Kara Capozzi"
"Kara Capozzi


3.  titles = document.querySelectorAll('.info-title')
(3) [h3.info-title, h3.info-title, h3.info-title]


titles[1].innerText = "Work"


4.  body = document.querySelector('body')  
body.style.background = 'blue'


5.  Change the colour of each element using the highlight class. Use a for loop to do this.

6.  Change the font family of the h1 to 'monospace'.

heading.style.fontFamily = 'monospace'
"monospace"


7. left = document.querySelector('aside')

var bigIcons = document.querySelectorAll('.action-icon-bg')
undefined
bigIcons[0]
<a class=​"action-icon-bg" href=​"#">​…​</a>​
big = bigIcons[0]
<a class=​"action-icon-bg" href=​"#">​…​</a>​
big.style.background = 'yellow'


8.  title = document.querySelectorAll('.bio-info-title')
(3) [span.bio-info-title, span.bio-info-title, span.bio-info-title]
title[0].innerText = 'Identify Yourself'
"Identify Yourself"


9. **** Change the placeholder attribute of the message field to "state your business".

message = document.querySelectorAll('textarea')
[textarea#message]

message = document.querySelector('textarea')
<textarea name=​"message" id=​"message" placeholder=​"State your business">​</textarea>​
message.placeholder = "State your business please"
"State your business please"

10.  
Give the name field a "value" attribute of "your nemesis".

n = document.querySelector('.contact-info')
<input type=​"text" name=​"name" class=​"contact-info" id=​"name" placeholder=​"Name">​
n
<input type=​"text" name=​"name" class=​"contact-info" id=​"name" placeholder=​"Name">​
n.placeholder;
"Name"
n.placeholder = "Your nemesis"
"Your nemesis"


11.  
mail = document.querySelectorAll('.contact-info')
(2) [input#name.contact-info, input#email.contact-info]
mail[1]
<input type=​"email" name=​"email" class=​"contact-info" id=​"email" placeholder=​"Email">​
mail[1].placeholder
"Email"
mail[1].placeholder = "koalathebear@gmail.com"
"koalathebear@gmail.com"


12.  
sub = document.querySelectorAll('input')
(3) [input#name.contact-info, input#email.contact-info, input#submit]length: 30: input#name.contact-info1: input#email.contact-info2: input#submit__proto__: NodeList
sub[3]
undefined
sub[2]
<input type=​"submit" name=​"submit" id=​"submit" value=​"Submit">​
sub[2].value = "En garde!"
"En garde!"

13.  
sub[2].disabled = "false"
"false"


14.  
container = document.querySelector('.bio-info')
<ul class=​"bio-info">​…​</ul>​
container.hidden
false
container.hidden = 'true'
"true"



Removing Elements from the DOM

Panda the Bear is lying about their skills! Take the "time travel" skill off the page to satisfy your personal sense of justice. Use your googling and docs-skimming skillz to find a jQuery function that will allow you to remove elements from the DOM. (hint: there are multiple ways of doing this, but the parent() function might be useful when it comes to selecting the right element)
Adding Elements to the DOM

That drawing of Pikachu is really cute. Let’s duplicate it using cloneNode() and insert it at the bottom of the .portfolio-container using insertAdjacentHTML() or appendChild().

Wow, that was so satisfying I think we should do it 10 more times. Use a for loop to help you do this.

Let’s add a message about when the page was last updated. We'll do this by appending a new <li> element to the <ul> in the sidebar (you might need to refresh the page to bring back the list items that we emptied out earlier).

screenshot of final effect

document.createElement, document.createTextNode, and appendChild are the keys to this process.

First we need to construct a new <li> tag.

var listItem = document.createElement('li');

It isn't part of the DOM yet, it's just floating in the void. We'll eventually attach it to the <ul> in the sidebar, below Panda's name, location, and phone number.

Now we need a new <span> tag to go inside the <li> we just made. This span will eventually go in the left column below 'Phone'.

var leftSpan = document.createElement('span');

Next we need to make a "text node" in order to put text inside our new span. A text node is a chunk of plain text that lives inside some HTML tag in the DOM.

var lastUpdated = document.createTextNode('Page last updated on');

We're ready to put that new text node inside our new <span> using appendChild.

leftSpan.appendChild(lastUpdated);

And we'll put the <span> inside the <li>, again using appendChild.

listItem.appendChild(leftSpan);

At this point our new elements are attached to each other but are still floating in the void separate from our webpage's DOM.

It's up to you to go through the same process for the second span that will go in the right-hand column of the <ul> (below Panda's phone number). Look up the docs for the Date class to find a way of displaying the current date inside your next text node.

After that, find a way of selecting the <ul> and append the new <li> to it. For bonus marks, apply the correct classes to these new elements of yours so the styling is consistent with the rest of the list items.
