<!DOCTYPE html>

<html>

<body>



<h2>Community Survey</h2>



<div id="question1">
  <label for="q1">Hi! Am I speaking to _______</label><br>

<input type="radio" id="q1" name="answer" value="yes" onclick="section1Q1answer(this);">

  <label for="q1">Yes</label><br>

  <input type="radio" id="q1" name="answer" value="don't call again" onclick="section1DontCallAgain(this);">

  <label for="q1">Don't Call Again</label><br>

  <input type="radio" id="q1" name="answer" value="did not pick up" onclick="section1DidNotPickUp(this);">

  <label for="q1">Did Not Pick Up</label><br>

  <input type="radio" id="q1" name="answer" value="deceased" onclick="section1Deceased(this);">

  <label for="q1">Deceased</label><br>
   <input type="radio" id="q1" name="answer" value="call later" onclick="section1CallLater(this);">

  <label for="q1">Call Later</label><br>
   <input type="radio" id="q1" name="answer" value="wrong number" onclick="section1WrongNumber(this);">

  <label for="q1">Wrong Number</label><br>
   <input type="radio" id="q1" name="answer" value="different language" onclick="section1DifferentLangauge(this);">

  <label for="q1">Different Language</label><br><br>
</div>

<div id="question2" Style="display:none;">
<label for="second">My name is ______ and I am a volunteer with a student led initiative called Empowered to gage community support on issues that affect voters like you. I was wondering if you had a second to share your opinions regarding the police in your community.</label><br>

<input type="radio" id="second" name="opinion" value="yes" onclick="question2(this);">

  <label for="second">Yes</label><br>

  <input type="radio" id="second" name="opinion" value="no" onclick="answer2(this);">

  <label for="second">No</label><br><br>
</div>


<div id="section1" Style="display:none;">

  <label for="bq1">What are your first thoughts and feelings when you see a police officer?</label><br>

   <input type="radio" id="bq1" name="feeling" value="positive" onclick="section1Positive(this);">

  <label for="bq1">Positive</label><br>

  <input type="radio" id="bq1" name="feeling" value="neutral" onclick="section1Neutral(this);">

  <label for="bq1">Neutral</label><br>

  <input type="radio" id="bq1" name="feeling" value="negative" onclick="section1Negative(this);">

  <label for="bq1">Negative</label><br><br>



 <label for="bq2">Do you feel safe when you see a police officer?</label><br>

   <input type="radio" id="bq2" name="safe" value="yes" onclick="section1Yes(this);">

  <label for="bq2">Yes</label><br>

  <input type="radio" id="bq2" name="safe" value="no" onclick="section1No(this);">

  <label for="bq2">No</label><br>

  <input type="radio" id="bq2" name="safe" value="unsure" onclick="section1Unsure(this);">

  <label for="bq2">Unsure</label><br><br>
</div>




<div id="section2" Style="display:none;">
<!— first new form if they answered yes to base question 2 —>

<label for="bq2Ylv2">What about the police force makes you feel safe?</label><br>
   <input type="text" id="bq2Ylv2" name="feelingsAbout" required ><br><br>

<label for="bq2Ylv3">Would you say all members of your community feel safe around the police?</label><br>

  <input type="radio" id="bq2Ylv3" name="CommunitySafe" value="yes" onclick="section2Yes(this);">

  <label for="bq2Ylv3">Yes</label><br>

  <input type="radio" id="bq2Ylv3" name="CommunitySafe" value="no" onclick="section2No(this);">

  <label for="bq2Ylv3">No</label><br>

  <input type="radio" id="bq2Ylv3" name="CommunitySafe" value="unsure" onclick="section2Unsure(this);">

  <label for="bq2Ylv3">Unsure</label><br><br>
</div>





<div id="section3" Style="display:none;">
<!—this question will appear if they answered yes to the previous form. Goes to the end dialogue after question is answered>

<label for="bq2Ylv4">Why would you say they feel safe?</label><br>
        <input type="text" id="bq2Ylv4" name="WhyCommunitySafe" required><br><br><br>


<p>Thank you for taking the time to answer our community survey. Have a great day!</p>

<label for="endMsgTextBoxsec3">Name: </label><br>
        <input type="text" id="endMsgTextBoxsec3" name="nameTextBox"  required><br><br>

<label for="numberTextBoxsec3">Phone Number: </label><br>
<input type="text" id="endMsgTextBox2sec3" name="numberTextBox" onfocusout="section3();" required><br><br>
<input type="submit" value="Submit" onclick="save()">

</div>



<div id="section4" Style="display:none;">

<!— this question will appear if they answered no to question bq2Ylv3. This question will go to base question 3 after being submitted —>

<label for="bq2Ylv5">Why would you say they don’t feel safe?</label><br>

   <input type="text" id="bq2Ylv5" name="WhyCommunityNotSafe" required><br><br>

<label for="bq3">Are you comfortable with the equipment of the police including military equipment, such as drones, armed speed boats, and grenade launchers?</label><br>

   <input type="radio" id="bq3" name="equipment" value="yes" onclick="section4Yes(this);">

  <label for="bq3">Yes</label><br>

  <input type="radio" id="bq3" name="equipment" value="no" onclick="section4No(this);">

  <label for="bq3">No</label><br>

  <input type="radio" id="bq3" name="equipment" value="unsure" onclick="section4Unsure(this);">

  <label for="bq3">Unsure</label><br><br>

</div>



<!— if answer is unsure then go straight to end dialogue —>



<div id="section5" Style="display:none;">

<!— this form is for the answer unsure for base question 2 —>

<label for="bq2NSlv2">Would you say all members of your community feel safe around the police?</label><br>

   <input type="radio" id="bq2NSlv2" name="CommunitySafe2" value="yes" onclick="section5Yes(this);">

  <label for="bq2NSlv2">Yes</label><br>

  <input type="radio" id="bq2NSlv2" name="CommunitySafe2" value="yes" onclick="section5No(this);">

  <label for="bq2NSlv2">No</label><br>

 <input type="radio" id="bq2NSlv2" name="CommunitySafe2" value="yes" onclick="section5Unsure(this);">

  <label for="bq2NSlv2">Unsure</label><br><br>

</div>



<div id="section6" Style="display:none;">

<!— this question will appear if they answered yes to question bq2NSlv2 . Cuts to end dialogue after this question appears —>

<label for="bq2NSlv3">Why would you say they feel safe?</label><br>

   <input type="text" id="bq2NSlv3" name="WhyCommunitySafe2" onfocusout="section6();" required><br><br>
   

<p>Thank you for taking the time to answer our community survey. Have a great day!</p>

<label for="endMsgTextBoxsec6">Name: </label><br>
        <input type="text" id="endMsgTextBoxsec6" name="nameTextBox" required><br><br>

<label for="numberTextBoxsec6">Phone Number: </label><br>
<input type="text" id="endMsgTextBox2sec6" name="numberTextBox" onfocusout="section6();" required><br><br>
<input type="submit" value="Submit" onclick="save()">
</div>



<div id="section7" Style="display:none;">

<!— this question will appear if they answered no to question bq2NSlv2. Goes to base question 3 after this question appears —>

<label for="bq2NSlv4">Why would you say they don’t feel safe?</label><br>

   <input type="text" id="bq2NSlv4" name="WhyCommunityNotSafe2" required ><br><br>
   
<label for="bq3">Are you comfortable with the equipment of the police including military equipment, such as drones, armed speed boats, and grenade launchers?</label><br>

   <input type= "radio" id="bq3" name="equipment" value="yes" onclick="section7Yes(this);">

  <label for="bq3">Yes</label><br>

  <input type= "radio" id="bq3" name="equipment" value="no" onclick="section7No(this);">
 

  <label for="bq3">No</label><br>

   <input type= "radio" id="bq3" name="equipment" value="unsure" onclick="section7Unsure(this);">

  <label for="bq3">Unsure</label><br><br>
</div>



<div id="section8" Style="display:none;">

<!— this question will appear if they answered no to the base question 2. Goes to base question 3 after this question appears —>

<label for="bq2Nlv2">What about the police doesn’t make you feel safe?</label><br>

   <input type="text" id="bq2Nlv2" name="WhatPoliceNotSafe" required><br><br>
<label for="bq3">Are you comfortable with the equipment of the police including military equipment, such as drones, armed speed boats, and grenade launchers?</label><br>

   <input type= "radio" id="bq3" name="equipment" value="yes" onclick="section8Yes(this);">

  <label for="bq3">Yes</label><br>

  <input type= "radio" id="bq3" name="equipment" value="no" onclick="section8No(this);">

  <label for="bq3">No</label><br>

  <input type= "radio" id="bq3" name="equipment" value="unsure" onclick="section8Unsure(this);">

  <label for="bq3">Unsure</label><br><br>

<!— this question will appear if they answered no to the base question 2. Goes to base question 3 after this question appears —>
</div>






<div id="section9" Style="display:none;">

<label for="bq3">Are you comfortable with the equipment of the police including military equipment, such as drones, armed speed boats, and grenade launchers?</label><br>

   <input type="radio" id="bq3" name="equipment" value="yes" onclick="section9Yes(this);">

  <label for="bq3">Yes</label><br>

<input type="radio" id="bq3" name="equipment" value="no" onclick="section9No(this);">

  <label for="bq3">No</label><br>

<input type="radio" id="bq3" name="equipment" value="unsure" onclick="section9Unsure(this);">

  <label for="bq3">Unsure</label><br><br>

</div> 



<!— if yes is answered to bq3, cut to end dialogue. —>



<div id="section10" Style="display:none;">

<!— this question will appear if unsure is answered to bq3. —>

<label for="bq3NSlv2">That’s okay. Do you believe that these things make out community safer?</label><br>

   <input type="radio" id="bq3NSlv2" name="saferCommunity" value="yes" onclick="section10Yes(this);">

  <label for="bq3NSlv2">Yes</label><br>

  <input type="radio" id="bq3NSlv2" name="saferCommunity" value="no" onclick="section10No(this);">

  <label for="bq3NSlv2">No</label><br>

  <input type="radio" id="bq3NSlv2" name="saferCommunity" value="unsure" onclick="section10Unsure(this);">

  <label for="bq3NSlv2">Unsure</label><br><br>

<!— if yes is answered to this question, go to end dialogue.  If no is answered to this question, go the form that would appear is no was answered to bq3 —>

</div>
 



<div id= "section11" Style="display:none;">

<!— this question will appear if unsure is answered to question bq3NSlv2. if no is answered to this question, cut to end dialogue. The question details will be provided tmr.—>

<label for="bq3NSlv3"> Would you be interested in hearing about local police budget information so you can make an informed decision on the issue?</label><br>

   <input type="radio" id="bq3NSlv3" name="hearInfo" value="yes" onclick="section11Yes(this);">

  <label for="bq3NSlv3">Yes</label><br>

  <input type="radio" id="bq3NSlv3" name="hearInfo" value="no" onclick="section11No(this);">
  <label for="bq3NSlv3">No</label><br>

</div>



<div id="section12" Style="display:none;">

<!— this form will appear if no is answered to bq3. —>

<label for="bq3Nlv2">Do you think the money used to pay for this equipment could be spent anywhere better?</label><br>

   <input type="radio" id="bq3Nlv2" name="money" value="yes" onclick="section12Yes(this);">

  <label for="bq3Nlv2">Yes</label><br>

  <input type="radio" id="bq3Nlv2"name="money" value="no" onclick="section12No(this);">

  <label for="bq3Nlv2">No</label><br>

  <input type="radio" id="bq3Nlv2" name="money" value="unsure" onclick="section12Unsure(this);">

  <label for="bq3Nlv2">Unsure</label><br><br>

<!— if no is answered to this question, cut to end dialogue. If unsure is answered to this question, go to bq3Nlv3  —>

</div>



<div id="section13" Style="display:none;">

<!— this form will appear if yes is answered to question bq3Nlv2 —>

<label for="bq3Nlv3">If you could spend these funds anywhere in our community where would you spend these funds?</label><br>

   <input type="text" id="bq3Nlv3" name="SpendFunds"><br><br>



<label for="bq3Nlv4">Would you or anyone you know be interested in finding out how you can make these changes happen in our community?</label><br>

   <input type="radio" id="bq3Nlv4" name="interested" value="yes" onclick="section13Yes(this);" required>

  <label for="bq3Nlv4">Yes</label><br>

  <input type="radio" id="bq3Nlv4" name="interested" value="no" onclick="section13No(this);" required>

  <label for="bq3Nlv4">No</label><br><br>

<!—if no is answered to this question, cut to end dialogue. —>
</div>



<div id="section14" Style="display:none;">

<!— this question will appear if yes is answered to question bq3Nlv4. If no, display a certain message before showing end dialogue —>

<label for="bq3Nlv5">That’s great! Would you like to sign up to our email list for more information and volunteer opportunities to make the changes we need?</label><br>

   <input type="radio" id="bq3Nlv5" name="EmailSignUp" value="yes" onclick="section14Yes(this);" required>

  <label for="bq3Nlv5">Yes</label><br>

  <input type="radio" id="bq3Nlv5" name="EmailSignUp" value="no" onclick="section14No(this);" required>

  <label for="bq3Nlv5">No</label><br><br>

</div>



<div id="section15" Style="display:none;">

<!— this question will appear if yes was answered to the email question bq3Nlv5. —>

<label for="bq3Nlv6">Great to hear. We can get you started with your name and your email address.</label><br><br>

<label for="bq3Nlv6sec15">Full Name: </label><br>
<input type="text" id="bq3Nlv6sec15" name="FullName" required><br>

<label for="bq3Nlv6emailsec15">Email: </label><br>
<input type="text" id="bq3Nlv6emailsec15" name="Email" onfocusout="section15();" required><br><br>

</div>


<div id="endMsg" Style="display:none;">

<p>Thank you for taking the time to answer our community survey. Have a great day!</p>

<label for="endMsgTextBox">Name: </label><br>
        <input type="text" id="endMsgTextBox" name="nameTextBox" required><br>

<label for="numberTextBox">Phone Number: </label><br>
<input type="text" id="endMsgTextBox2" name="numberTextBox" onfocusout="endMsg();" required><br><br>
<input type="submit" value="Submit" onclick="save()">
<!—end message—>
</div>

<div id="section11Paragraph" Style="display:none;">
<p>GETTING THIS INFORMATION LATER</p>
</div>

<div id="section15NoMsg" Style="display:none;">
<p>That's okay. You can still visit our website at empoweredusa.org</p>
<p>Thank you for taking the time to answer our community survey. Have a great day!</p>

<label for="endMsgTextBoxsec15NoMsg">Name: </label><br>
        <input type="text" id="endMsgTextBoxsec15NoMsg" name="nameTextBox" required><br>

<label for="numberTextBox">Phone Number: </label><br>
<input type="text" id="endMsgTextBox2sec15NoMsg" name="numberTextBox" onfocusout="section15NoMsg();" required><br><br>
<input type="submit" value="Submit" onclick="save()">
</div>

<div id="endMsg2" Style="display:none;">
<p>Sorry to bother you. Have a great day!</p>
</div>







<script>

var nameOfInterviewee="";
var dataEntered="";

function question2(opinion){
        document.getElementById("section1").style.display="block";
document.getElementById("endMsg2").style.display="none";
}

function answer2(opinion){
        document.getElementById("endMsg2").style.display="block";
}

function section1Q1answer(answer){
        document.getElementById("question2").style.display="block";
}

function section1DontCallAgain(answer){
document.getElementById("endMsg2").style.display="block";
}

function section1Deceased(answer){
        section1DontCallAgain(answer);
}

function section1CallLater(answer){
        section1DontCallAgain(answer);
}

function section1WrongNumber(answer){
        section1DontCallAgain(answer);
}

function section1DifferentLanguage(answer){
        section1DontCallAgain(answer);
}

function section1DidNotPickUp(answer){
        document.getElementById("endMsg").style.display="block";
}

function section1Positive(feeling){
        var feelingVal=feeling.value;
    dataEntered= dataEntered + "What are your first thoughts and feelings when you see a police officer? : " + feelingVal + "\n\n";
}

function section1Neutral(feeling){
        var feelingVal=feeling.value;
        dataEntered= dataEntered + "What are your first thoughts and feelings when you see a police officer? : " + feelingVal + "\n\n";
}

function section1Negative(feeling){
        var feelingVal=feeling.value;
        dataEntered= dataEntered + "What are your first thoughts and feelings when you see a police officer? : " + feelingVal + "\n\n";
}

function section1Yes(safe){
var safeVal=safe.value;
dataEntered= dataEntered + "Do you feel safe when you see a police officer? : " + safeVal + "\n\n";
document.getElementById("section8").style.display="none";
    document.getElementById("section5").style.display="none";
    document.getElementById("section2").style.display="block";
}

function section1No(safe){
var safeVal=safe.value;
dataEntered= dataEntered + "Do you feel safe when you see a police officer? : " + safeVal + "\n\n";

document.getElementById("section2").style.display="none";
    document.getElementById("section8").style.display="block";
    document.getElementById("section5").style.display="none";
}

function section1Unsure(safe){
var safeVal=safe.value;
dataEntered= dataEntered + "Do you feel safe when you see a police officer? : " + safeVal + "\n\n";

document.getElementById("section2").style.display="none";
    document.getElementById("section8").style.display="none";
    document.getElementById("section5").style.display="block";
}

function section2Yes(CommunitySafe){
var feelingsAboutVal=document.getElementById("bq2Ylv2").value;
var CommunitySafeVal=CommunitySafe.value;
dataEntered= dataEntered + "What about the police force makes you feel safe? : " + feelingsAboutVal + "\n\n" + "Would you say all members of your community feel safe around the police? : " + CommunitySafeVal + "\n\n" ;

document.getElementById("section4").style.display="none";
        document.getElementById("section3").style.display="block";
    document.getElementById("endMsg").style.display="none";
}

function section2No(CommunitySafe){
var feelingsAboutVal=document.getElementById("bq2Ylv2").value;
var CommunitySafeVal=CommunitySafe.value;
dataEntered= dataEntered + "What about the police force makes you feel safe? : " + feelingsAboutVal + "\n\n" + "Would you say all members of your community feel safe around the police? : " + CommunitySafeVal + "\n\n";

document.getElementById("section3").style.display="none";
    document.getElementById("section4").style.display="block";
    document.getElementById("endMsg").style.display="none";
}

function section2Unsure(CommunitySafe){
var feelingsAboutVal=document.getElementById("bq2Ylv2").value;
var CommunitySafeVal=CommunitySafe.value;
dataEntered= dataEntered + "What about the police force makes you feel safe? : " + feelingsAboutVal + "\n\n" + "Would you say all members of your community feel safe around the police? : " + CommunitySafeVal + "\n\n";

document.getElementById("section3").style.display="none";
        document.getElementById("section4").style.display="none";
    document.getElementById("endMsg").style.display="block";   
}

function section3(){
var WhyCommunitySafeVal=document.getElementById("bq2Ylv4").value;
var nameTextBoxVal=document.getElementById("endMsgTextBoxsec3").value;
var numberTextBoxVal=document.getElementById("endMsgTextBox2sec3").value;
dataEntered= dataEntered + "Why would you say they feel safe? : " + WhyCommunitySafeVal + "\n\n" + "Name : " + nameTextBoxVal + "\n\n" + "Phone Number : " + numberTextBoxVal + "\n\n";
nameOfInterviewee=nameTextBoxVal;
}

function section4Yes(equipment){
var WhyCommunityNotSafeVal=document.getElementById("bq2Ylv5").value;
var equipmentVal=equipment.value;
dataEntered= dataEntered + "Why would you say they don’t feel safe? : " + WhyCommunityNotSafeVal + "\n\n" + "Are you comfortable with the equipment of the police including military equipment, such as drones, armed speed boats, and grenade launchers? : " + equipmentVal + "\n\n";
    section9Yes(equipment);
}

function section4No(equipment){
var WhyCommunityNotSafeVal=document.getElementById("bq2Ylv5").value;
var equipmentVal=equipment.value;
dataEntered= dataEntered + "Why would you say they don’t feel safe? : " + WhyCommunityNotSafeVal + "\n\n" + "Are you comfortable with the equipment of the police including military equipment, such as drones, armed speed boats, and grenade launchers? : " + equipmentVal + "\n\n";
    section9No(equipment);
}

function section4Unsure(equipment){
var WhyCommunityNotSafeVal=document.getElementById("bq2Ylv5").value;
var equipmentVal=equipment.value;
dataEntered= dataEntered + "Why would you say they don’t feel safe? : " + WhyCommunityNotSafeVal + "\n\n" + "Are you comfortable with the equipment of the police including military equipment, such as drones, armed speed boats, and grenade launchers? : " + equipmentVal + "\n\n";      
    section9Unsure(equipment);
}

function section5Yes(CommunitySafe2){
var CommunitySafe2Val=CommunitySafe2.value;
dataEntered=dataEntered + "Would you say all members of your community feel safe around the police? : " + CommunitySafe2Val + "\n\n";
document.getElementById("section6").style.display="block";
    document.getElementById("section7").style.display="none";
        document.getElementById("section9").style.display="none";
}

function section5No(CommunitySafe2){
var CommunitySafe2Val=CommunitySafe2.value;
dataEntered=dataEntered + "Would you say all members of your community feel safe around the police? : " + CommunitySafe2Val + "\n\n";

document.getElementById("section6").style.display="none";
    document.getElementById("section7").style.display="block";
    document.getElementById("section9").style.display="none";
}

function section5Unsure(CommunitySafe2){
var CommunitySafe2Val=CommunitySafe2.value;
dataEntered=dataEntered + "Would you say all members of your community feel safe around the police? : " + CommunitySafe2Val + "\n\n";

document.getElementById("section6").style.display="none";
    document.getElementById("section7").style.display="none";
    document.getElementById("section9").style.display="block";
}

function section6(){
var WhyCommunitySafe2Val=document.getElementById("bq2NSlv3").value;
var nameTextBoxVal=document.getElementById("endMsgTextBoxsec6").value;
var numberTextBoxVal=document.getElementById("endMsgTextBox2sec6").value;
dataEntered= dataEntered + "Why would you say they feel safe? : " + WhyCommunitySafe2Val + "\n\n" + "Name : " + nameTextBoxVal + "\n\n" + "Phone Number : " + numberTextBoxVal + "\n\n";
nameOfInterviewee=nameTextBoxVal;
}




function section7Yes(equipment){
var WhyCommunityNotSafe2Val=document.getElementById("bq2NSlv4").value;
var equipmentVal=equipment.value;
dataEntered= dataEntered + "Why would you say they don’t feel safe? : " + WhyCommunityNotSafe2Val + "\n\n";     
    section9Yes(equipment);
}

function section7No(equipment){
var WhyCommunityNotSafe2Val=document.getElementById("bq2NSlv4").value;
var equipmentVal=equipment.value;
dataEntered= dataEntered + "Why would you say they don’t feel safe? : " + WhyCommunityNotSafe2Val + "\n\n";
    section9No(equipment);
}

function section7Unsure(equipment){
var WhyCommunityNotSafe2Val=document.getElementById("bq2NSlv4").value;
var equipmentVal=equipment.value;
dataEntered= dataEntered + "Why would you say they don’t feel safe? : " + WhyCommunityNotSafe2Val + "\n\n";     
    section9Unsure(equipment);
}

function section8Yes(equipment){
var WhatPoliceNotSafeVal=document.getElementById("bq2Nlv2").value;
var equipmentVal=equipment.value;
dataEntered= dataEntered + "What about the police doesn't make you feel safe? : " + WhatPoliceNotSafeVal + "\n\n";      
    section9Yes(equipment);
}

function section8No(equipment){
var WhatPoliceNotSafeVal=document.getElementById("bq2Nlv2").value;
var equipmentVal=equipment.value;
dataEntered= dataEntered + "What about the police doesn't make you feel safe? : " + WhatPoliceNotSafeVal + "\n\n";      
    section9No(equipment);
}

function section8Unsure(equipment){
var WhatPoliceNotSafeVal=document.getElementById("bq2Nlv2").value;
var equipmentVal=equipment.value;
dataEntered= dataEntered + "What about the police doesn't make you feel safe? : " + WhatPoliceNotSafeVal + "\n\n";      
    section9Unsure(equipment);
}

function section9Yes(equipment){
var equipmentVal=equipment.value;
dataEntered=dataEntered + "Are you comfortable with the equipment of the police including military equipment, such as drones, armed speed boats, and grenade launchers? : " + equipmentVal + "\n\n";

document.getElementById("endMsg").style.display="block";
        document.getElementById("section10").style.display="none";
        document.getElementById("section12").style.display="none";
}

function section9Unsure(equipment){
var equipmentVal=equipment.value;
dataEntered=dataEntered + "Are you comfortable with the equipment of the police including military equipment, such as drones, armed speed boats, and grenade launchers? : " + equipmentVal + "\n\n";      
   document.getElementById("section10").style.display="block";
    document.getElementById("endMsg").style.display="none";
        document.getElementById("section12").style.display="none";
}

function section9No(equipment){
var equipmentVal=equipment.value;
dataEntered=dataEntered + "Are you comfortable with the equipment of the police including military equipment, such as drones, armed speed boats, and grenade launchers? : " + equipmentVal + "\n\n";      
   document.getElementById("section12").style.display="block";
    document.getElementById("section10").style.display="none";
    document.getElementById("endMsg").style.display="none";
}
    
function section10Unsure(saferCommunity){
var saferCommunityVal=saferCommunity.value;
dataEntered=dataEntered + "That’s okay. Do you believe that these things make out community safer? : " + saferCommunityVal + "\n\n";

document.getElementById("section11").style.display="block";
        document.getElementById("section12").style.display="none";
        document.getElementById("endMsg").style.display="none";
}

function section10No(saferCommunity){
var saferCommunityVal=saferCommunity.value;
dataEntered=dataEntered + "That’s okay. Do you believe that these things make out community safer? : " + saferCommunityVal + "\n\n";

document.getElementById("section11").style.display="none";
        document.getElementById("section12").style.display="block";
        document.getElementById("endMsg").style.display="none";
}

function section10Yes(saferCommunity){
var saferCommunityVal=saferCommunity.value;
dataEntered=dataEntered + "That’s okay. Do you believe that these things make out community safer? : " + saferCommunityVal + "\n\n";      
    document.getElementById("section11").style.display="none";
        document.getElementById("section12").style.display="none";
        document.getElementById("endMsg").style.display="block";
}
        
function section11Yes(hearInfo){                                        
var hearInfoVal=hearInfo.value;
dataEntered=dataEntered + "Would you be interested in hearing about local police budget information so you can make an informed decision on the issue? : " + hearInfoVal + "\n\n";


        getElementById("endMsg").style.display="block";
}

function section11No(hearInfo){
var hearInfoVal=hearInfo.value;
dataEntered=dataEntered + "Would you be interested in hearing about local police budget information so you can make an informed decision on the issue? : " + hearInfoVal + "\n\n";        document.getElementById("endMsg").style.display="block";
}

function section12Yes(money){
var moneyVal=money.value;
dataEntered=dataEntered + "Do you think the money used to pay for this equipment could be spent anywhere better? : " + moneyVal + "\n\n";

document.getElementById("section13").style.display="block";
        document.getElementById("endMsg").style.display="none";
}

function section12Unsure(money){
var moneyVal=money.value;
dataEntered=dataEntered + "Do you think the money used to pay for this equipment could be spent anywhere better? : " + moneyVal + "\n\n"; 
    
    section12Yes(money);
        document.getElementById("endMsg").style.display="none";
}

function section12No(money){
var moneyVal=money.value;
dataEntered=dataEntered + "Do you think the money used to pay for this equipment could be spent anywhere better? : " + moneyVal + "\n\n"; 

document.getElementById("endMsg").style.display="block";
        document.getElementById("section13").style.display="none";
}

function section13Yes(interested){
var SpendFundsVal=document.getElementById("bq3Nlv3").value;
var interestedVal=interested.value;
dataEntered=dataEntered + "If you could spend these funds anywhere in our community where would you spend these funds? : " + SpendFundsVal + "\n\n" + "Would you or anyone you know be interested in finding out how you can make these changes happen in our community? : " + interestedVal + "\n\n";      

document.getElementById("section14").style.display="block";
}

function section13No(interested){
var SpendFundsVal=document.getElementById("bq3Nlv3").value;
var interestedVal=interested.value;
dataEntered=dataEntered + "If you could spend these funds anywhere in our community where would you spend these funds? : " + SpendFundsVal + "\n\n" + "Would you or anyone you know be interested in finding out how you can make these changes happen in our community? : " + interestedVal + "\n\n";      
    document.getElementById("endMsg").style.display="block";
        document.getElementById("section14").style.display="none";
}

function section14Yes(EmailSignUp){
var EmailSignUpVal=EmailSignUp.value;
dataEntered=dataEntered + "That’s great! Would you like to sign up to our email list for more information and volunteer opportunities to make the changes we need? : " + EmailSignUpVal + "\n\n";

document.getElementById("section15").style.display="block";
        document.getElementById("endMsg").style.display="block";
}

function section14No(EmailSignUp){
var EmailSignUpVal=EmailSignUp.value;
dataEntered=dataEntered + "That’s great! Would you like to sign up to our email list for more information and volunteer opportunities to make the changes we need? : " + EmailSignUpVal + "\n\n"; document.getElementById("section15NoMsg").style.display="block";
    document.getElementById("endMsg").style.display="none";
}

function section15(){
var FullNameVal=document.getElementById("bq3Nlv6sec15").value;
var EmailVal=document.getElementById("bq3Nlv6emailsec15").value;
dataEntered= dataEntered + "Full Name : " + FullNameVal + "\n\n" + "Email : " + EmailVal + "\n\n";
nameOfInterviewee=nameTextBoxVal;
}

function endMsg(){
var nameTextBoxVal=document.getElementById("endMsgTextBox").value;
var numberTextBoxVal=document.getElementById("endMsgTextBox2").value;
dataEntered= dataEntered + "Name : " + nameTextBoxVal + "\n\n" + "Phone Number : " + numberTextBoxVal + "\n\n";
nameOfInterviewee=nameTextBoxVal;
}

function section15NoMsg(){
var nameTextBoxVal=document.getElementById("endMsgTextBoxsec15NoMsg").value;
var numberTextBoxVal=document.getElementById("endMsgTextBox2sec15NoMsg").value;
dataEntered= dataEntered + "Name : " + nameTextBoxVal + "\n\n" + "Phone Number : " + numberTextBoxVal + "\n\n";
nameOfInterviewee=nameTextBoxVal;
}

function save(){
    
        var d=new Date();
        var timestamp = d.getFullYear().toString() + (d.getMonth()+1).toString() + d.getDate().toString() + d.getHours().toString() + d.getMinutes().toString();
      
      	var fileHeading = "SURVEY RESULTS FOR " + nameOfInterviewee + " ON " + d.getFullYear().toString() + (d.getMonth()+1).toString() + d.getDate().toString() + " AT " + d.getHours().toString() +":"+ d.getMinutes().toString();
            
		var textToSave = fileHeading + "\n\n" + dataEntered;
        var textToSaveAsBlob = new Blob([textToSave], {type:"text/plain"});
        var textToSaveAsURL = window.URL.createObjectURL(textToSaveAsBlob);
        var downloadLink = document.createElement("a");
        downloadLink.download = nameOfInterviewee + "-" + timestamp + ".txt"
        downloadLink.innerHTML = "Download File";
        downloadLink.href = textToSaveAsURL;
        downloadLink.style.display = "none";
        document.body.appendChild(downloadLink);
        downloadLink.click();

}

</script>



</body>

</html>

















