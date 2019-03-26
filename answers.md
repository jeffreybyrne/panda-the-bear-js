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
