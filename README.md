# feedback-popup
Html,css

# Corner
C# Corner Search
TECHNOLOGIES
ANSWERS
LEARN
NEWS
BLOGS
VIDEOS
INTERVIEW PREP
BOOKS
EVENTS
CAREER
MEMBERS
JOBS
Creating a Feedback Form Using HTML
Dhanush M Dhanush M  Updated date Apr 09, 2020
  28.4k 0 3

facebook
twitter
linkedIn
Reddit
WhatsApp
Download Free .NET & JAVA Files API
Try Free File Format APIs for Word/Excel/PDF
Introduction
 
During the creation of websites for online classes, shopping, or anything else, you need to attach a feedback form for the purpose of getting the feedback from the customer or user. Those feedbacks help the organisation to improve their services. The fields for the feedback forms vary for the organizations and their services, but there will be a common layout for all those forms, such as first name, last name, mail ID and feedback section. Creating this kind of forms using HTML is not a tedious process. In this article, we will discuss creating a feedback form using HTML for web development.
 
Creating a Feedback Form
 
For creating a feedback form you can open a new HTML code editing page in your IDE. Here, I am using Visual Studio Code for this purpose. You can install the Visual Studio Code by clicking here. I embedded the codes in the single file, but you can link the different files for style sheet, Javascript and PHP work. You can use the source code given below for creating a page:
<!DOCTYPE html>    
<html>    
<head>    
<meta name="viewport" content="width=device-width, initial-scale=1">    
<style>    
* {    
  box-sizing: border-box;    
}    
    
input[type=text], select, textarea {    
  width: 100%;    
  padding: 12px;    
  border: 1px solid rgb(70, 68, 68);    
  border-radius: 4px;    
  resize: vertical;    
}    
input[type=email], select, textarea {    
  width: 100%;    
  padding: 12px;    
  border: 1px solid rgb(70, 68, 68);    
  border-radius: 4px;    
  resize: vertical;    
}    
    
label {    
  padding: 12px 12px 12px 0;    
  display: inline-block;    
}    
    
input[type=submit] {    
  background-color: rgb(37, 116, 161);    
  color: white;    
  padding: 12px 20px;    
  border: none;    
  border-radius: 4px;    
  cursor: pointer;    
  float: right;    
}    
    
input[type=submit]:hover {    
  background-color: #45a049;    
}    
    
.container {    
  border-radius: 5px;    
  background-color: #f2f2f2;    
  padding: 20px;    
}    
    
.col-25 {    
  float: left;    
  width: 25%;    
  margin-top: 6px;    
}    
    
.col-75 {    
  float: left;    
  width: 75%;    
  margin-top: 6px;    
}    
    
/* Clear floats after the columns */    
.row:after {    
  content: "";    
  display: table;    
  clear: both;    
}    
    
/* Responsive layout - when the screen is less than 600px wide, make the two columns stack on top of each other instead of next to each other */    
</style>    
</head>    
<body>    
<h2>FEED BACK FORM</h2>    
<div class="container">    
  <form>    
    <div class="row">    
      <div class="col-25">    
        <label for="fname">First Name</label>    
      </div>    
      <div class="col-75">    
        <input type="text" id="fname" name="firstname" placeholder="Your name..">    
      </div>    
    </div>    
    <div class="row">    
      <div class="col-25">    
        <label for="lname">Last Name</label>    
      </div>    
      <div class="col-75">    
        <input type="text" id="lname" name="lastname" placeholder="Your last name..">    
      </div>    
    </div>    
    <div class="row">    
        <div class="col-25">    
          <label for="email">Mail Id</label>    
        </div>    
        <div class="col-75">    
          <input type="email" id="email" name="mailid" placeholder="Your mail id..">    
        </div>    
      </div>    
    <div class="row">    
      <div class="col-25">    
        <label for="country">Country</label>    
      </div>    
      <div class="col-75">    
        <select id="country" name="country">    
            <option value="none">Select Country</option>    
          <option value="australia">Australia</option>    
          <option value="canada">Canada</option>    
          <option value="usa">USA</option>    
          <option value="russia">Russia</option>    
          <option value="japan">Japan</option>    
          <option value="india">India</option>    
          <option value="china">China</option>    
        </select>    
      </div>    
    </div>    
    <div class="row">    
      <div class="col-25">    
        <label for="feed_back">Feed Back</label>    
      </div>    
      <div class="col-75">    
        <textarea id="subject" name="subject" placeholder="Write something.." style="height:200px"></textarea>    
      </div>    
    </div>    
    <div class="row">    
      <input type="submit" value="Submit">    
    </div>    
  </form>    
</div>    
    
</body>    
</html>    
