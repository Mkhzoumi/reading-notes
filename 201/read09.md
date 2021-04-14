# *forms*
## *forms: a printed document that contains spaces for you to fill in information.*
## *there are several types of fomrs control:*
+ ## *adding text: text input, password input.*
+ ## *making choices: checkboxes, drop down boxes.*
+ ## *submitting forms: subment butons, image buttons.*
+ ## *uploading files.*

## *this is the steps of how forms work:*
1. ## *the user fill the form and submit it.*
2. ## *the name of form control is send with its information which the user enters to the server.*
3. ## *the server process the information using programming language.*
4. ## *the server send bake a new page based on the informatiion received.*

## *we use forms by writing the form element then we write the attribute action and then the method of that form, example:*

```
<form action="http://www.example.com/subscribe.php" method="get">

<p>This is where the form controls will appear.</p>

</form>
```
## *text input:*
## *in this example the username input type is text, and the size of the input rectangle is 15, and the maximum length a user can input in 30 character.*

```
<form action="http://www.example.com/login.php">
<p>Username:
 <input type="text" name="username" size="15" 
 maxlength="30" />
</p>
<p>Password:
 <input type="password" name="password" size="15" 
 maxlength="30" />
</p>
</form>
```

## *text area.*

```
<form action="http://www.example.com/comments.php">
<p>What did you think of this gig?</p>
 <textarea name="comments" cols="20" rows="4">Enter 
 your comments...</textarea>
</form>
```

## *radio buttons.*

```
<form action="http://www.example.com/profile.php">
<p>Please select your favorite genre:
 <br />
 <input type="radio" name="genre" value="rock" 
 checked="checked" /> Rock
 <input type="radio" name="genre" value="pop" /> 
 Pop
 <input type="radio" name="genre" value="jazz" /> 
 Jazz
</p>
</form>
```

## *checkbox.*

```
<form action="http://www.example.com/profile.php">
<p>Please select your favorite music service(s):
 <br />
 <input type="checkbox" name="service" 
 value="itunes" checked="checked" /> iTunes
 <input type="checkbox" name="service" 
 value="lastfm" /> Last.fm
 <input type="checkbox" name="service" 
 value="spotify" /> Spotify
</p>
</form>
```

# *CSS list styling*
## *in css you can style the bullet point of the list.*
## *for example if you want to change the style of a list we use:*

```
ol {
list-style-type: lower-roman;}

ul {
list-style-type: circle;}

ul {
list-style-image: url("images/star.png");}   // to put an image instead of bullet
```

# *CSS table styling*
## *we can use css to style talbes, and there is a lot of changes you can make on table styling, for exampe check this code:*

```
table {
width: 600px;
empty-cells: show;}
th, td {
padding: 7px 10px 10px 10px;}
th {
text-transform: uppercase;
letter-spacing: 0.1em;
font-size: 90%;
border-bottom: 2px solid #111111;
border-top: 1px solid #999;
text-align: left;}
```

# *events*
## *Events are the browser's way of indicating when something has happened .*
## *when user interact with html, there are some steps to trigger javascript code.*
## *these steps are known as event handling:*
1. ## *select the element node.*
2. ## *indicate which event on the selected node will trigger the response.*
3. ## *state the code you want to run when the event occurs.*

## *there are 3 event handlers:*
1. ## *html event handlers. (this is old and its a bad practice so dont use it.)*
2. ## *traditional DOM event handlers.*
3. ## *DOM level 2 event listeners.*




# [back](../README.md)