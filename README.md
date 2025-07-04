<!DOCTYPE html><html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>SnapEdit Pro - AI Photo Enhancer</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
    }
    .hero {
      background: url('https://images.unsplash.com/photo-1526170375885-4d8ecf77b99f') center/cover no-repeat;
      color: white;
      padding: 100px 20px;
      text-align: center;
    }
    .pricing-card {
      border-radius: 15px;
      transition: transform 0.3s;
    }
    .pricing-card:hover {
      transform: translateY(-10px);
    }
    .feature-icon {
      font-size: 2rem;
      color: #0d6efd;
    }
  </style>
</head>
<body>
  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-light bg-light shadow-sm">
    <div class="container">
      <a class="navbar-brand fw-bold" href="#">SnapEdit Pro</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item"><a class="nav-link" href="#features">Features</a></li>
          <li class="nav-item"><a class="nav-link" href="#pricing">Pricing</a></li>
          <li class="nav-item"><a class="nav-link" href="#contact">Contact</a></li>
        </ul>
      </div>
    </div>
  </nav>  <!-- Hero Section -->  <section class="hero">
    <div class="container">
      <h1 class="display-4 fw-bold">Enhance Your Photos with AI</h1>
      <p class="lead">SnapEdit Pro transforms your images using smart AI-powered enhancements. Perfect for photographers, designers, and social media creators.</p>
      <a href="#pricing" class="btn btn-primary btn-lg mt-3">Get Started</a>
    </div>
  </section>  <!-- Features Section -->  <section id="features" class="py-5">
    <div class="container">
      <div class="row text-center mb-4">
        <h2 class="fw-bold">Why Choose SnapEdit Pro?</h2>
      </div>
      <div class="row g-4 text-center">
        <div class="col-md-4">
          <div class="feature-icon mb-2">📸</div>
          <h5>AI Auto Enhancement</h5>
          <p>One-click photo optimization with professional-level results.</p>
        </div>
        <div class="col-md-4">
          <div class="feature-icon mb-2">🎨</div>
          <h5>Style Filters</h5>
          <p>Apply aesthetic filters and color grading to match your brand.</p>
        </div>
        <div class="col-md-4">
          <div class="feature-icon mb-2">☁️</div>
          <h5>Cloud Storage</h5>
          <p>Save and organize your edits securely in the cloud.</p>
        </div>
      </div>
    </div>
  </section>  <!-- Pricing Section -->  <section id="pricing" class="py-5 bg-light">
    <div class="container">
      <div class="row text-center mb-4">
        <h2 class="fw-bold">Choose Your Plan</h2>
        <p class="text-muted">Flexible pricing to suit everyone.</p>
      </div>
      <div class="row g-4">
        <div class="col-md-4">
          <div class="card pricing-card p-4">
            <h5 class="fw-bold text-center">Free</h5>
            <h2 class="text-center">$0<span class="fs-6">/mo</span></h2>
            <ul class="list-unstyled mt-3 mb-4">
              <li>✓ Basic AI enhancement</li>
              <li>✓ 10 photo exports/month</li>
              <li>✗ No cloud storage</li>
            </ul>
            <div class="d-grid">
              <button class="btn btn-outline-primary">Try Free</button>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card pricing-card p-4 border-primary border-2">
            <h5 class="fw-bold text-center text-primary">Pro</h5>
            <h2 class="text-center">$9.99<span class="fs-6">/mo</span></h2>
            <ul class="list-unstyled mt-3 mb-4">
              <li>✓ Unlimited enhancements</li>
              <li>✓ 100 photo exports/month</li>
              <li>✓ 20 GB cloud storage</li>
            </ul>
            <div class="d-grid">
              <button class="btn btn-primary">Get Pro</button>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card pricing-card p-4">
            <h5 class="fw-bold text-center">Team</h5>
            <h2 class="text-center">$29.99<span class="fs-6">/mo</span></h2>
            <ul class="list-unstyled mt-3 mb-4">
              <li>✓ All Pro features</li>
              <li>✓ Up to 5 users</li>
              <li>✓ Priority support</li>
            </ul>
            <div class="d-grid">
              <button class="btn btn-outline-primary">Start Team Plan</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>  <!-- Contact Section -->  <section id="contact" class="py-5">
    <div class="container">
      <div class="row mb-4 text-center">
        <h2 class="fw-bold">Get in Touch</h2>
        <p class="text-muted">Have questions or need support? We're here to help.</p>
      </div>
      <div class="row justify-content-center">
        <div class="col-md-6">
          <form id="contactForm">
            <div class="mb-3">
              <label for="name" class="form-label">Name</label>
              <input type="text" class="form-control" id="name" required />
            </div>
            <div class="mb-3">
              <label for="email" class="form-label">Email</label>
              <input type="email" class="form-control" id="email" required />
            </div>
            <div class="mb-3">
              <label for="message" class="form-label">Message</label>
              <textarea class="form-control" id="message" rows="4" required></textarea>
            </div>
            <button type="submit" class="btn btn-primary">Send Message</button>
          </form>
        </div>
      </div>
    </div>
  </section>  <!-- Footer -->  <footer class="bg-dark text-white text-center py-3">
    <p class="mb-0">&copy; 2025 SnapEdit Pro. All rights reserved.</p>
  </footer>  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>  <script>
    document.getElementById('contactForm').addEventListener('submit', function (e) {
      e.preventDefault();
      alert('Thank you for contacting us, ' + document.getElementById('name').value + '!');
      this.reset();
    });
  </script></body>
</html>