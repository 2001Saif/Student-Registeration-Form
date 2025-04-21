# Student-Registeration-Form
An Html Code Of Student Registeration Form
<html>
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1"/>
    <link rel="stylesheet" href="Assng1.css"/>
</head>
<body>
    <div class="formContainer">
        <div class="formHeader">
            <div class="formLogo">
                <img src="LOGO.jfif"/>
                <div>
                    <p>MUSLIM YOUTH UNIVERSITY ISLAMABAD</p>
                    <p>H69J+P3X Japan Road, ISLAMABAD</p>
                    <p>Tel: +923412698698 | E-mail: https://myu.edu.pk</p>
                </div>
            </div>
            <!-- Moved the reference number above the profile image -->
            <div class="refNumber">
                Ref No: <span class="refBold">14573</span>
            </div>
            <img src="S.jfif" class="profileImage"/>
        </div>
        <h1 class="formTitle">STUDENT REGISTERATION FORM</h1>
        <form>
            <div class="formSection">
                <h2>• Student Information</h2>
                <label for="fullName">Full Name:</label>
                <input id="fullName" type="text" /><br/>
                <label for="dob">Date of Birth:</label>
                <input id="dob" type="date" /><br/>
                <label>Gender:</label>
                <label><input type="radio" name="gender" value="Male"/> Male</label>
                <label><input type="radio" name="gender" value="Female"/> Female</label><br/>
                <label for="nationality">Nationality:</label>
                <input id="nationality" type="text" /><br/>
                <label for="contactInfo">Contact Information:</label>
                <input id="contactInfo" type="text" />
            </div>
            <div class="formSection">
                <h2>• Parent/Guardian Information</h2>
                <label for="parentName">Parent/Guardian Name(s):</label>
                <input id="parentName" type="text" /><br/>
                <label for="relationship">Relationship to Student:</label>
                <input id="relationship" type="text" /><br/>
                <label for="contactParent">Contact Information (Phone Number, Email):</label>
                <input id="contactParent" type="text" /><br/>
                <label for="emergencyContact">Emergency Contact Information:</label>
                <input id="emergencyContact" type="text" />
            </div>
            <div class="formSection">
                <h2>• Education Information</h2>
                <label for="schoolName">School/Institution Name:</label>
                <input id="schoolName" type="text" /><br/>
                <label for="graduationDate">Graduation Date (if applicable):</label>
                <input id="graduationDate" type="date" /><br/>
                <label for="hearAboutUs">How did you hear about us?</label>
                <input id="hearAboutUs" type="text" /><br/>
                <label for="interestReason">Why are you interested in our program?</label>
                <input id="interestReason" type="text" />
            </div>
            <div class="termsBox">
                <span>Are you agree to the terms and conditions of enrollment?</span>
                <span class="thumbsUp">👍</span>
                <span class="thumbsDown">👎</span>
            </div>
        </form>

        <div class="termsInfo">
            <span>• Terms and Conditions</span>
        </div>

        <div class="signatureSection">
            <p>Signature of the student and, if the student is a minor, a parent or guardian</p>
            <div class="signatureBox"></div>
        </div>
    </div>
</body> 
</html>

CSS CODE:
body {
    background-color: #fae7b4;
    font-family:  sans-serif;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    align-items: center;
    color: #2c2c2c;
}
.formContainer {
    width: 50%;
    background: #fef8dc;
    border-radius: 10px;
    padding: 40px;
    box-shadow: 0 6px 16px rgba(0, 0, 0, 0.1);
    box-sizing: border-box;
}
.formHeader {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 30px;
}
.formLogo {
    display: flex;
    align-items: center;
}
.formLogo img {
    width: 90px;
    height: 90px;
    margin-right: 12px;
}
.profileImage {
    width: 140px; 
    height: 140px; 
    border-radius: 50%;
    object-fit: cover;
    margin-top: 10px; 
}

.formContainer {
    width: 50%;
    background: #fef8dc;
    border-radius: 10px;
    padding: 40px;
    box-shadow: 0 6px 16px rgba(0, 0, 0, 0.1);
    box-sizing: border-box;
    position: relative; 
}

.refNumber {
    font-size: 16px;
    font-weight: 600;
    position: absolute; 
    top: 20px; 
    right: 20px;
    text-align: right;
}

.formTitle {
    text-align: center;
    font-weight: 700;
    font-size: 28px;
    margin-bottom: 30px;
    color: #333;
}
.formSection {
    margin-bottom: 35px;
}
.formSection h2 {
    background: #f7941d;
    color: white;
    padding: 8px 12px;
    margin-bottom: 16px;
    font-size: 18px;
    font-weight: 600;
    border-radius: 5px;
}
label {
    width: 180px;
    display: inline-block;
    font-size: 15px;
    color: #444;
    font-weight: 600;
    padding: 6px 0;
    margin-bottom: 10px;
    transition: color 0.3s;
}
input {
    background: #ffffff;
    border: 1px solid #ccc;
    border-radius: 6px;
    padding: 8px;
    width: calc(100% - 190px);
    margin-bottom: 15px;
    box-sizing: border-box;
    font-size: 14px;
    font-family: 'Poppins', sans-serif;
}
input[type="radio"] {
    width: auto;
    margin-right: 6px;
}
.termsBox {
    display: flex;
    align-items: center;
    font-size: 15px;
    margin-bottom: 10px;
    font-weight: 500;
}
.termsInfo {
    display: flex;
    align-items: center;
    margin-left: 20px;
    font-size: 13px;
    color: #111;
    font-weight: 500;
}
.signatureSection {
    margin-top: 25px;
    font-size: 14px;
    font-weight: 500;
}
.signatureBox {
    width: 160px;
    height: 50px;
    background: #f9e6a0;
    border: 1px solid #f9e6a0;
    margin-top: 12px;
    border-radius: 4px;
}
.thumbsUp,
.thumbsDown {
    font-size: 20px;
    margin-left: 12px;
    cursor: pointer;
    transition: transform 0.2s ease;
}
.thumbsUp:hover,
.thumbsDown:hover {
    transform: scale(1.2);
}
.refBold {
    font-weight: 700;
}
