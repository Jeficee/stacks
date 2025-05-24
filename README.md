<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Employee Information Form</title>
  <link rel="stylesheet" href="form.css">
</head>
<body>
  <h1>EMPLOYEE INFORMATION FORM</h1>
  <hr>

  <form id="employeeForm">
    <h3>Personal Information</h3>
    Full Name: <input type="text" name="fullName" required><br><br>
    Address: <input type="text" name="address" required><br><br>
    Phone Number: <input type="text" name="phone" required>
    Email: <input type="email" name="email" required><br><br>

    <h3>Employment Information</h3>
    Title: <input type="text" name="title" required>
    Department: <input type="text" name="department" required><br><br>
    Date of Hire: <input type="date" name="hireDate" required><br><br>
    Employment Status:<br>
    <input type="checkbox" name="status" value="Full Time"> Full Time
    <input type="checkbox" name="status" value="Part Time"> Part Time
    <input type="checkbox" name="status" value="Contractor"> Contractor
    <input type="checkbox" name="status" value="Intern"> Intern
    <input type="checkbox" name="status" value="Other"> Other: <input type="text" name="otherStatus"><br><br>

    <h3>Education</h3>
    Highest Level of Education: <input type="text" name="educationLevel" required><br><br>
    Name of Institution: <input type="text" name="institution" required>
    Degree Earned: <input type="text" name="degree" required><br><br>
    Major/Field of Study: <input type="text" name="major" required>
    Graduation Date: <input type="date" name="gradDate" required><br><br>

    <h3>Professional Experience</h3>
    Licenses: <input type="text" name="licenses"><br><br>
    Previous Work Experience:<br>
    <textarea name="experience" style="height: 150px; width: 300px;"></textarea><br><br>

    <h3>Emergency Contact Information</h3>
    Full Name: <input type="text" name="emergencyName" required><br><br>
    Address: <input type="text" name="emergencyAddress" required><br><br>
    Phone Number: <input type="text" name="emergencyPhone" required>
    Cell Phone Number: <input type="text" name="emergencyCell" required><br><br>
    Relationship: <input type="text" name="relationship" required><br><br>

    <p>Employee Signature</p>
    Signature: <input type="text" name="signature">
    Date: <input type="text" name="date"><br><br>

    <input type="submit" value="Submit" style="background-color: lightblue;">
  </form>

  <script src="form.js"></script>
</body>
</html>


document.getElementById("employeeForm").addEventListener("submit", function (e) {
  e.preventDefault();
  const form = e.target;

  const formData = {
    fullName: form.fullName.value,
    address: form.address.value,
    phone: form.phone.value,
    email: form.email.value,
    title: form.title.value,
    department: form.department.value,
    hireDate: form.hireDate.value,
    status: Array.from(form.querySelectorAll('input[name="status"]:checked')).map(cb => cb.value),
    otherStatus: form.otherStatus.value,
    educationLevel: form.educationLevel.value,
    institution: form.institution.value,
    degree: form.degree.value,
    major: form.major.value,
    gradDate: form.gradDate.value,
    licenses: form.licenses.value,
    experience: form.experience.value,
    emergencyName: form.emergencyName.value,
    emergencyAddress: form.emergencyAddress.value,
    emergencyPhone: form.emergencyPhone.value,
    emergencyCell: form.emergencyCell.value,
    relationship: form.relationship.value,
    signature: form.signature.value,
    date: form.date.value,
  };

  localStorage.setItem("employeeFormData", JSON.stringify(formData));
  window.location.href = "submitted.html";
});


<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Submitted Info</title>
  <link rel="stylesheet" href="form.css">
</head>
<body>
  <h1>SUBMITTED EMPLOYEE INFORMATION</h1>
  <hr>
  <div id="displayData"></div>

  <script>
    const data = JSON.parse(localStorage.getItem("employeeFormData"));
    const output = document.getElementById("displayData");

    if (data) {
      output.innerHTML = `
        <h3>Personal Information</h3>
        <p><strong>Name:</strong> ${data.fullName}</p>
        <p><strong>Address:</strong> ${data.address}</p>
        <p><strong>Phone:</strong> ${data.phone}</p>
        <p><strong>Email:</strong> ${data.email}</p>

        <h3>Employment Info</h3>
        <p><strong>Title:</strong> ${data.title}</p>
        <p><strong>Department:</strong> ${data.department}</p>
        <p><strong>Date of Hire:</strong> ${data.hireDate}</p>
        <p><strong>Status:</strong> ${data.status.join(", ") || data.otherStatus}</p>

        <h3>Education</h3>
        <p><strong>Level:</strong> ${data.educationLevel}</p>
        <p><strong>Institution:</strong> ${data.institution}</p>
        <p><strong>Degree:</strong> ${data.degree}</p>
        <p><strong>Major:</strong> ${data.major}</p>
        <p><strong>Graduation:</strong> ${data.gradDate}</p>

        <h3>Experience</h3>
        <p><strong>Licenses:</strong> ${data.licenses}</p>
        <p><strong>Work Experience:</strong> ${data.experience}</p>

        <h3>Emergency Contact</h3>
        <p><strong>Name:</strong> ${data.emergencyName}</p>
        <p><strong>Address:</strong> ${data.emergencyAddress}</p>
        <p><strong>Phone:</strong> ${data.emergencyPhone}</p>
        <p><strong>Cell:</strong> ${data.emergencyCell}</p>
        <p><strong>Relationship:</strong> ${data.relationship}</p>

        <h3>Signature</h3>
        <p>${data.signature} | ${data.date}</p>
      `;
    } else {
      output.innerHTML = "<p>No submitted data found.</p>";
    }
  </script>
</body>
</html>
