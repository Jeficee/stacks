<script>
  const form = document.getElementById('loginForm');

  form.addEventListener('submit', function (event) {
    event.preventDefault(); // Prevent the default form submission
    event.stopPropagation();

    if (form.checkValidity()) {
      // Redirect to the dashboard if form is valid
      window.location.href = 'dashboard.html';
    }

    form.classList.add('was-validated');
  });
</script>