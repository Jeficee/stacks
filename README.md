<DOCTYPE! html>
<html>
<head>
    <style>
        h1 {
        text-align: center;
        }
        </style>
     <title>Employee Information Form</title>
     <h1>EMPLOYEE INFORMATION FORM<hr></h1>
</head>
<body>

    <h3>Personal Information</h3>
    <form>
        Full Name: <input type="text" required><br>
        <br>
        Address: <input type="text" required><br>
        <br>
        Phone Number: <input type="text" required>
        Email: <input type="text" required> <br>

        <h3>Employment Information</h3>
        Title: <input type="text" required>
        Department: <input type="text" required><br>
        <br>
        Date of Hire: <input type="text" required><br>
        <br>
        Employment Status: 
        <input type="checkbox">Full Time
        <input type="checkbox">Part Time
        <input type="checkbox">Contractor
        <input type="checkbox">Intern
        <input type="checkbox">Other:<input type="text"><br>

        <h3>Education</h3>
        Highest Level of Education: <input type="text" required><br>
        <br>
        Name of Institution: <input type="text" required>
        Degree Earned: <input type="text" required> <br>
        <br>
        Major/Field of Study: <input type="text" required>
        Graduation Date: <input type="text" required> <br>
        <br>

        <h3>Professional Experience</h3>
        Professional Experience and Licenses: <input type="text"><br>
        <br>
        Previous Work Experience: <br><textarea name="textarea" rows="5" cols="40"></textarea><br>
        <br>
        
        <h3>Emergency Contact Information</h3>
        Full Name: <input type="text" required><br>
        <br>
        Address: <input type="text" required><br>
        <br>
        Phone Number: <input type="text" required>
        Cell Phone Number: <input type="text" required> <br>
        <br>
        Relationship: <input type="text" required><br>
        <br>
        <input type="submit" value="Send" style="background-color: lightblue;">
    </form>
</body>
</html>
