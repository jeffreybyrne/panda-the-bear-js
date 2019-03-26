1. Select the element that contains the profile image (hint: look for the class). Change the src attribute so it points to a picture of your choosing instead.

profilePic = document.querySelector('.profile-image');
<img src=​"images/​self-portrait-grassbg.jpg" alt=​"Self Portrait" title=​"Self Portrait" class=​"profile-image">​
profilePic.src = 'https://s3.amazonaws.com/pix.iemoji.com/images/emoji/apple/ios-12/256/panda-face.png'

2. Use the same approach to select the element that contains the photo of the sky and change the src attribute to another picture URL of your choosing.

skyImage = document.querySelectorAll('img')[1]
<img src=​"images/​clouds-man.jpg" alt=​"Man Walking on Ice" title=​"Man Walking on Ice">​
skyImage.src = 'http://zoranmarinovic.com/wp-content/gallery/under-dark-oil-cloud-2/thumbs/thumbs_Under-Dark-Oil-Cloud-2-49.jpg'

3. Select the heading that says "Panda the Bear" and change it to your own name.

mainHeader = document.body.querySelector('h1')
<h1 class=​"highlight">​Panda The Bear​</h1>​
mainHeader.innerText = 'Jeff Byrne'

4. Select the heading that says "Employment" and change it to something else. (hint: use a descendant selector)

empHeader = document.querySelector('#employment h3');
<h3 class=​"info-title">​<i class=​"icon-suitcase">​::before​</i>​" &nbsp; Employment"</h3>​
empHeader.innerText = "Unemployment"

5. Change the colour of the body.

body = document.querySelector('body')
<body>​…​</body>​
body.style.color = 'red'

6. Change the colour of each element using the highlight class. Use a for loop to do this.

highlights = document.querySelectorAll('.highlight')
highlights.forEach(function(element) {element.style.color = 'blue'})

7. Change the font family of the h1 to 'monospace'.

header = document.querySelector('h1')
<h1 class=​"highlight" style=​"color:​ blue;​">​Panda The Bear​</h1>​
header.style.fontFamily = 'monospace';

8. Find a way to select the round icons in the sidebar and then change their colour.

circles = document.querySelectorAll('.action-icon-bg');
circles.forEach(function(element) {element.style.backgroundColor = 'brown'})

9. Scroll down to the contact form. Change the placeholder attribute of the name field to "identify yourself".

nameBox = document.querySelector('.contact-info');
<input type=​"text" name=​"name" class=​"contact-info" id=​"name" placeholder=​"Name">​
nameBox.placeholder = 'identify yourself'

10. Change the placeholder attribute of the message field to "state your business".

messageBox = document.querySelector('#message')
<textarea name=​"message" id=​"message" placeholder=​"Message">​</textarea>​
messageBox.placeholder = 'state your business'

11. Give the name field a "value" attribute of "your nemesis".

nameBox.value = 'your nemesis'

12. Change the value attribute of the email field to "koalathebear@gmail.com".

emailBox = document.querySelector('#email')
<input type=​"email" name=​"email" class=​"contact-info" id=​"email" placeholder=​"Email">​
emailBox.value = 'koalathebear@gmail.com'

13. Change the value of the submit button on the contact form to "En garde!".

submitButton = document.querySelector('#submit')
<input type=​"submit" name=​"submit" id=​"submit" value=​"Submit">​
submitButton.value = "En garde!"

14. We should stop Koala from sending an email to Panda that they might regret! Find a way to disable the submit button (hint: familiarize yourself with the disabled attribute).

submitButton.disabled = true

15. We should help Panda protect their privacy by erasing their personal details from the sidebar.

childObjs = document.querySelectorAll('.bio-info li')
parentObj.removeChild(childObjs[0])
<li class=​"bio-info-item">​…​</li>​
parentObj.removeChild(childObjs[1])
<li class=​"bio-info-item">​…​</li>​
parentObj.removeChild(childObjs[2])
<li class=​"bio-info-item">​…​</li>​


PART 2

Panda the Bear is lying about their skills! Take the "time travel" skill off the page to satisfy your personal sense of justice. Use your googling and docs-skimming skillz to find a function that will allow you to remove elements from the DOM. (hint: there are multiple ways of doing this, but parentNode might be useful when it comes to selecting the right element)

timeTravel = document.querySelectorAll('.bar-default')[2]
<div class=​"bar-default">​…​</div>​
timeTravelParent = timeTravel.parentNode
<div>​…​</div>​
timeTravelParent.removeChild(timeTravel)
<div class=​"bar-default">​…​</div>​

That drawing of Pikachu is really cute. Let’s duplicate it using cloneNode() and insert it at the bottom of the .portfolio-container using insertAdjacentHTML() or appendChild().

pika = document.querySelector('#right-image > img')
<img src=​"images/​pikachu-drawing.jpg" alt=​"Pikachu" title=​"Pikachu">​
pikanew = pika.cloneNode(true)
<img src=​"images/​pikachu-drawing.jpg" alt=​"Pikachu" title=​"Pikachu">​
portfolio = document.querySelector('.portfolio-container')
<div class=​"portfolio-container">​…​</div>​
portfolio.appendChild(pikanew)
<img src=​"images/​pikachu-drawing.jpg" alt=​"Pikachu" title=​"Pikachu">​
