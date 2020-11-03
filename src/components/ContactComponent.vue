<template>
  <div id="temp">
	  <div class="content">
        <h2 style="padding: 2px;" id="contact-me">Contact Me</h2>
            <div>
             <ul>
                <li>You can reach me at <a href="mailto:shahiburrahman55@gmail.com">shahiburrahman55@gmail.com</a>.</li>
             </ul>
             <!-- <h2 style="padding: 2px;">Another way to contact</h2> -->

				<ul style="padding-left: 0px;" id="ul_form" >

				  <div class="container">
				  <form name="ask-question" method="POST" data-netlify="true"

				  data-netlify-honeypot="bot-field">
				  <input type="hidden" name="form-name" value="ask-question" />
				  
				  <div class="row">
				    <div class="col-25">
				      <label for="fname"><strong>Name</strong></label>
				    </div>
				    <div class="col-75">
				      <input type="text" id="name" name="name" placeholder="Your Name" required>
				    </div>
				  </div>
				  <div class="row">
				    <div class="col-25">
				      <label for="email"><strong>Email</strong></label>
				    </div>
				    <div class="col-75">
				      <input type="email" id="email" name="email" placeholder="Your Email Address" required>
				    </div>
				  </div>
				  <div class="row">
				    <div class="col-25">
				      <label for="subject"><strong>Subject</strong></label>
				    </div>
				    <div class="col-75">
					<select id="subject" name="subject">
					  <option value="I have a question">I have a question</option>
					  <option value="I want to hire you">I want to hire you</option>
					  <option value="Other">Other</option>
					</select>
				    </div>
				  </div>
				  <div class="row">
				    <div class="col-25">
				      <label for="message"><strong>Message</strong></label>
				    </div>
				    <div class="col-75">
				      <textarea id="message" name="message" placeholder="Explain how can I help you" style="height:120px" required ></textarea>
				    </div>
				  </div>
				  <div class="row">
				    <input type="submit" name="submit" value="SEND MESSAGE">
				  </div>

				  </form>
				</div>

				</ul>
<!--
				<ul>
					<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d605521.6632080749!2d91.30231826256644!3d24.809926435749244!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x375054d3d270329f%3A0xf58ef93431f67382!2sSylhet!5e0!3m2!1sen!2sbd!4v1594319088107!5m2!1sen!2sbd" width="600" height="450" frameborder="0" style="border:0;" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe>
				</ul>
-->

             	<div id="ul_submission">
             		<h4>
						Thank you! Your submission has been received!
             		</h4>
             	</div>


            </div>

      </div>
  </div>
</template>

<script>
export default {
  name: 'ContactComponent'
};
</script>

<style scoped>
*{box-sizing: border-box; }
input[type=text],[type=email],select, textarea {width: 100%; padding: 12px; border: 1px solid #ccc; border-radius: 9px; resize: vertical; }
label {padding: 12px 12px 12px 0; display: inline-block; }
input[type=submit]
{
background-color: white;
color: black;
padding: 12px 20px;
border: none;
border-radius: 9px;
cursor: pointer;
margin-left: 219px;
margin-top: 6px;
border: 2px solid #a5abad;
}
input[type=submit]:hover {
background-color: #a5abad;
}
.container {
border-radius: 9px; padding: 20px;
}
.col-25 {
float: left; width: 15%; margin-top: 6px;
}
.col-75 {
float: left; width: 65%; margin-top: 6px;
} /* Clear floats after the columns */
.row:after
{content: ""; display: table; clear: both; } /* Responsive layout - when the screen is less than 600px wide, make the two columns stack on top of each other instead of next to each other */ @media screen and (max-width: 600px) {.col-25, .col-75, input[type=submit] {width: 40%; margin-top: 5px; margin-left: 80px;} }

 #ul_submission {
  background-color: #7b8785;
  color: black;
  float: 50px;
  width: 350px;
  height: 100px;
  border: 1px solid #a5abad;
  padding: 16px;
  margin: 20px;
  border-radius: 9px;
  text-align: center;
  padding-top: 5px;
  position: fixed;
  top: 60%;
  left: 42%;
  margin-top: -90px;
  margin-left: -90px;
  display:none;
}
input[type=submit]{
	font-size:13px;
	display:flex;
	margin: 0 auto;
	margin-left: 230px;
	margin-top: 6px;
}
@media (max-width: 710px){
input[type=submit]{
	font-size:9px;
	display:flex;
	margin: 0 auto;	font-weight: bold;
	text-align:center;
	margin-top: 6px;
}

input[type=text],[type=email],select, textarea
{
	width:112%;
	display:flex;
	margin: 0 auto;


}
}

@media (max-width: 620px){
input[type=submit]{
	font-size:10px;
	display:flex;
	width: 24%;
	margin: 0 auto;	font-weight: bold;
	margin-top: 6px;
}

input[type=text],[type=email],select, textarea
{
	width:164%;
	display:flex;
	margin: 0 auto;

}
#ul_form{
	padding-left:0px;
}

}

@media (max-width: 520px){
input[type=submit]{
	font-size:10px;
	display:flex;
	width: 28%;
	margin: 0 auto;	font-weight: bold;
	margin-top: 6px;
}
input[type=text],[type=email],select, textarea
{
	width:150%;
	display:flex;
	margin: 0 auto;

}
}


 </style>
