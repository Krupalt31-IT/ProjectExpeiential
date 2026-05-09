<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Growth Hackers Consulting | Premium Business Scaling</title>

<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">

<style>
:root {
  --primary-blue: #6366f1;
  --dark-bg: #0f172a;
  --glass-white: rgba(255, 255, 255, 0.95);
}

html { scroll-behavior: smooth; }

body {
  background: linear-gradient(135deg, #f8fafc 0%, #e2e8f0 100%);
  color: #1e293b;
  font-family: 'Inter', sans-serif;
}

/* NAVBAR */
.navbar { background-color: var(--dark-bg); }

/* HERO */
.hero {
  background: linear-gradient(rgba(15, 23, 42, 0.8), rgba(99, 102, 241, 0.4)),
              url('https://images.unsplash.com/photo-1521737604893-d14cc237f11d?auto=format&fit=crop&q=80');
  background-size: cover;
  background-position: center;
  color: white;
  height: 90vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  clip-path: polygon(0 0, 100% 0, 100% 90%, 0% 100%);
}

.stats { 
  background: var(--dark-bg); 
  color: #6366f1; 
  padding: 60px 0;
  margin-top: -50px;
}
.stats h2 { font-weight: 800; color: white; }

/* CARDS */
.service-card, .price-card, .review-card {
  transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
  border: none;
  background: var(--glass-white);
  border-radius: 20px;
}
.service-card:hover, .price-card:hover, .review-card:hover {
  transform: translateY(-15px);
  box-shadow: 0 20px 40px rgba(99, 102, 241, 0.2) !important;
  cursor: pointer;
}

.service-img { height: 200px; object-fit: cover; border-radius: 20px 20px 0 0; }
.plan-icon { width: 60px; margin-bottom: 15px; }

/* REVIEWS */
.review-card { background: #1e293b; color: white; border: 1px solid rgba(255,255,255,0.1); }
.avatar {
    width: 70px;
    height: 70px;
    border-radius: 50%;
    object-fit: cover;
    border: 3px solid var(--primary-blue);
    margin-bottom: 15px;
}

/* FAQ */
.accordion-item { border: none; margin-bottom: 1rem; border-radius: 15px !important; overflow: hidden; }
.accordion-button:not(.collapsed) { background-color: var(--primary-blue); color: white; }

/* BUTTONS */
.btn-primary {
  background-color: var(--primary-blue);
  border: none;
  padding: 12px 30px;
  border-radius: 50px;
  font-weight: 600;
}

/* VIEWS */
#enquiry-view, #payment-view { display: none; min-height: 80vh; padding-top: 100px; }
.payment-card {
    background: white;
    padding: 40px;
    border-radius: 30px;
    max-width: 500px;
    margin: auto;
    box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.25);
}
</style>
</head>

<body>

<nav class="navbar navbar-expand-lg navbar-dark sticky-top">
  <div class="container">
    <a class="navbar-brand fw-bold" onclick="showView('home')">GROWTH<span class="text-primary">HACKERS</span></a>
    <button class="navbar-toggler" data-bs-toggle="collapse" data-bs-target="#nav"><span class="navbar-toggler-icon"></span></button>
    <div class="collapse navbar-collapse" id="nav">
      <ul class="navbar-nav ms-auto">
        <li class="nav-item"><a onclick="showView('home')" class="nav-link">Home</a></li>
        <li class="nav-item"><a href="#services" class="nav-link">Services</a></li>
        <li class="nav-item"><a href="#pricing" class="nav-link">Pricing</a></li>
        <li class="nav-item"><a href="#faq" class="nav-link">FAQ</a></li>
        <li class="nav-item"><a onclick="showView('enquiries')" class="nav-link fw-bold text-warning">Enquiries <span id="count-badge" class="badge bg-danger">0</span></a></li>
      </ul>
    </div>
  </div>
</nav>

<div id="main-site">
    <section class="hero">
      <div class="container">
        <h1 class="display-2 fw-bold mb-3 text-white">Scale Your <span class="text-primary">Vision</span></h1>
        <p class="lead mb-5 opacity-75">Engineered strategies for Nagpur's high-growth businesses.</p>
        <a href="#contact" class="btn btn-primary btn-lg">Start Today</a>
      </div>
    </section>

    <section class="stats text-center shadow">
        <div class="container"><div class="row">
          <div class="col-md-4"><h2>500+</h2><p class="small">Active Clients</p></div>
          <div class="col-md-4"><h2>1200%</h2><p class="small">Revenue Growth</p></div>
          <div class="col-md-4"><h2>10+</h2><p class="small">Expert Years</p></div>
        </div></div>
    </section>

    <section id="services" class="container py-5 mt-5">
      <h2 class="text-center mb-5 fw-bold">Our Expertise</h2>
      <div class="row g-4 text-center">
        <div class="col-md-4">
          <div class="card service-card shadow-sm h-100">
            <img src="https://images.unsplash.com/photo-1517245386807-bb43f82c33c4?auto=format&fit=crop&w=500" class="service-img">
            <div class="card-body"><h4>Business Consulting</h4><p class="text-muted">Strategic auditing for enterprises.</p></div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card service-card shadow-sm h-100">
            <img src="https://images.unsplash.com/photo-1460925895917-afdab827c52f?auto=format&fit=crop&w=500" class="service-img">
            <div class="card-body"><h4>Marketing Strategy</h4><p class="text-muted">High-converting digital funnels.</p></div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="card service-card shadow-sm h-100">
            <img src="https://images.unsplash.com/photo-1554224155-6726b3ff858f?auto=format&fit=crop&w=500" class="service-img">
            <div class="card-body"><h4>Financial Advisory</h4><p class="text-muted">Capital & profit management.</p></div>
          </div>
        </div>
      </div>
    </section>

    <section id="pricing" class="container py-5">
        <h2 class="text-center mb-5 fw-bold">Select Your Package</h2>
        <div class="row g-4 text-center">
          <div class="col-md-4">
              <div class="card p-5 price-card shadow-sm bg-white" onclick="goToPayment('Starter', '4,999')">
                  <img src="https://cdn-icons-png.flaticon.com/512/1532/1532616.png" class="plan-icon mx-auto">
                  <h5>Starter</h5><h2 class="fw-bold my-4">₹4,999</h2><button class="btn btn-outline-primary w-100">Choose</button>
              </div>
          </div>
          <div class="col-md-4">
              <div class="card p-5 price-card shadow-lg bg-dark text-white" onclick="goToPayment('Professional', '9,999')">
                  <img src="https://cdn-icons-png.flaticon.com/512/1162/1162464.png" class="plan-icon mx-auto">
                  <h5 class="text-primary">Professional</h5><h2 class="fw-bold my-4 text-white">₹9,999</h2><button class="btn btn-primary w-100 shadow">Popular</button>
              </div>
          </div>
          <div class="col-md-4">
              <div class="card p-5 price-card shadow-sm bg-white" onclick="goToPayment('Enterprise', '19,999')">
                  <img src="https://cdn-icons-png.flaticon.com/512/3135/3135661.png" class="plan-icon mx-auto">
                  <h5>Enterprise</h5><h2 class="fw-bold my-4">₹19,999</h2><button class="btn btn-outline-primary w-100">Choose</button>
              </div>
          </div>
        </div>
    </section>

    <section id="faq" class="container py-5">
        <h2 class="text-center fw-bold mb-5">Frequently Asked Questions</h2>
        <div class="accordion mx-auto" id="faqSection" style="max-width: 800px;">
            <div class="accordion-item shadow-sm">
                <h2 class="accordion-header"><button class="accordion-button" data-bs-toggle="collapse" data-bs-target="#q1">How do you guarantee growth?</button></h2>
                <div id="q1" class="accordion-collapse collapse show" data-bs-parent="#faqSection"><div class="accordion-body">We utilize data-driven frameworks to identify and fix revenue leaks.</div></div>
            </div>
            <div class="accordion-item shadow-sm">
                <h2 class="accordion-header"><button class="accordion-button collapsed" data-bs-toggle="collapse" data-bs-target="#q2">What industries do you work with?</button></h2>
                <div id="q2" class="accordion-collapse collapse" data-bs-parent="#faqSection"><div class="accordion-body">Specializing in Tech, Real Estate, and Nagpur-based services.</div></div>
            </div>
            <div class="accordion-item shadow-sm">
                <h2 class="accordion-header"><button class="accordion-button collapsed" data-bs-toggle="collapse" data-bs-target="#q3">Is ad spend included?</button></h2>
                <div id="q3" class="accordion-collapse collapse" data-bs-parent="#faqSection"><div class="accordion-body">Ad spend is separate from our strategic consulting fees.</div></div>
            </div>
            <div class="accordion-item shadow-sm">
                <h2 class="accordion-header"><button class="accordion-button collapsed" data-bs-toggle="collapse" data-bs-target="#q4">Can I visit your office?</button></h2>
                <div id="q4" class="accordion-collapse collapse" data-bs-parent="#faqSection"><div class="accordion-body">Yes! Visit IT Preneur in Sadar for a face-to-face strategy session.</div></div>
            </div>
        </div>
    </section>

    <section id="location" class="container py-5">
        <div class="row align-items-center bg-white rounded-5 shadow-lg overflow-hidden mx-1">
            <div class="col-md-5 p-5 bg-dark text-white">
                <h2 class="fw-bold mb-4">Nagpur Hub</h2>
                <p><strong>IT Preneur Nagpur</strong><br>Sadar, MH 440013</p>
                <a href="#" class="btn btn-primary mt-3">Get Location</a>
            </div>
            <div class="col-md-7 p-0"><iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3721.14486663523!2d79.0805!3d21.1466!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x0!2zMjHCsDA4JzQ3LjgiTiA3OcKwMDQnNDkuOCJF!5e0!3m2!1sen!2sin!4v16250000000008" width="100%" height="400" style="border:0;"></iframe></div>
        </div>
    </section>

    <section id="contact" class="container py-5">
        <div class="row justify-content-center">
            <div class="col-md-6 bg-white p-5 rounded-5 shadow-lg">
              <h2 class="text-center fw-bold mb-4">Request Consultation</h2>
              <form id="growthForm">
                  <input class="form-control mb-3 py-3 rounded-pill px-4" id="userName" placeholder="Your Name" required>
                  <input class="form-control mb-3 py-3 rounded-pill px-4" id="userEmail" type="email" placeholder="Email Address" required>
                  <textarea class="form-control mb-3 py-3 rounded-4 px-4" id="userMsg" placeholder="Goals..." rows="4" required></textarea>
                  <button type="submit" class="btn btn-primary w-100 py-3 rounded-pill shadow">Send Message</button>
              </form>
            </div>
        </div>
    </section>

    <section id="reviews" class="container py-5 mb-5">
        <h2 class="text-center mb-5 fw-bold">Client Testimonials</h2>
        <div class="row g-4 text-center">
            <div class="col-md-4"><div class="card review-card p-4 h-100"><img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?auto=format&fit=crop&w=150&q=80" class="avatar mx-auto"><h6 class="fw-bold mt-2">Arjun Mehta</h6><p class="fst-italic opacity-75 small">"Revenue tripled in 6 months!"</p></div></div>
            <div class="col-md-4"><div class="card review-card p-4 h-100"><img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?auto=format&fit=crop&w=150&q=80" class="avatar mx-auto"><h6 class="fw-bold mt-2">Sana Khan</h6><p class="fst-italic opacity-75 small">"Game changer for finance."</p></div></div>
            <div class="col-md-4"><div class="card review-card p-4 h-100"><img src="https://images.unsplash.com/photo-1500648767791-00dcc994a43e?auto=format&fit=crop&w=150&q=80" class="avatar mx-auto"><h6 class="fw-bold mt-2">Rahul Deshmukh</h6><p class="fst-italic opacity-75 small">"Best strategy in Sadar."</p></div></div>
        </div>
    </section>
</div>

<div id="payment-view" class="container py-5">
    <div class="payment-card">
        <h3 class="fw-bold text-center mb-2">Secure Checkout</h3>
        <p class="text-center text-muted mb-4">Package: <span id="selected-plan-name" class="text-primary fw-bold"></span> | <span id="selected-plan-price" class="fw-bold"></span></p>
        <form onsubmit="event.preventDefault(); alert('Payment Successful!'); showView('home')">
            <div class="mb-3"><label class="small fw-bold">NAME ON CARD</label><input type="text" class="form-control" placeholder="John Doe" required></div>
            <div class="mb-3"><label class="small fw-bold">CARD NUMBER</label><input type="text" class="form-control" placeholder="1234 5678 9101 1121" maxlength="16" required></div>
            <div class="row">
                <div class="col-6 mb-3"><label class="small fw-bold">EXPIRY (MM/YY)</label><input type="text" class="form-control" placeholder="12/26" required></div>
                <div class="col-6 mb-3"><label class="small fw-bold">CVV</label><input type="password" class="form-control" placeholder="***" maxlength="3" required></div>
            </div>
            <button class="btn btn-success w-100 btn-lg rounded-pill mt-3">Confirm Payment</button>
        </form>
        <button class="btn btn-link w-100 mt-2 text-muted" onclick="showView('home')">Cancel</button>
    </div>
</div>

<div id="enquiry-view" class="container py-5">
    <div class="d-flex justify-content-between mb-4"><h2>Enquiries</h2><button class="btn btn-danger btn-sm" onclick="clearAllData()">Clear All</button></div>
    <div class="table-responsive bg-white rounded-4 shadow p-4"><table class="table"><thead><tr><th>Date</th><th>Client</th><th>Email</th><th>Message</th></tr></thead><tbody id="table-body"></tbody></table></div>
    <div class="text-center mt-5"><button class="btn btn-dark px-5" onclick="showView('home')">Back</button></div>
</div>

<footer class="bg-dark text-white text-center p-5">
    <h3>GROWTH<span class="text-primary">HACKERS</span></h3>
    <p class="opacity-50 small">© 2026 Growth Hackers | Sadar, Nagpur</p>
</footer>

<script>
  function showView(view) {
    document.getElementById('main-site').style.display = 'none';
    document.getElementById('enquiry-view').style.display = 'none';
    document.getElementById('payment-view').style.display = 'none';
    if (view === 'home') document.getElementById('main-site').style.display = 'block';
    else if (view === 'enquiries') { document.getElementById('enquiry-view').style.display = 'block'; renderTable(); }
    window.scrollTo(0,0);
  }

  function goToPayment(plan, price) {
    document.getElementById('main-site').style.display = 'none';
    document.getElementById('payment-view').style.display = 'block';
    document.getElementById('selected-plan-name').innerText = plan;
    document.getElementById('selected-plan-price').innerText = '₹' + price;
  }

  document.getElementById('growthForm').addEventListener('submit', function(e) {
    e.preventDefault();
    const entry = { name: document.getElementById('userName').value, email: document.getElementById('userEmail').value, message: document.getElementById('userMsg').value, date: new Date().toLocaleDateString() };
    const current = JSON.parse(localStorage.getItem('gh_enquiries') || '[]');
    current.push(entry);
    localStorage.setItem('gh_enquiries', JSON.stringify(current));
    this.reset(); renderTable(); alert("Inquiry Sent!");
  });

  function renderTable() {
    const data = JSON.parse(localStorage.getItem('gh_enquiries') || '[]');
    document.getElementById('count-badge').innerText = data.length;
    const tableBody = document.getElementById('table-body');
    tableBody.innerHTML = data.length ? data.map(item => `<tr><td>${item.date}</td><td>${item.name}</td><td>${item.email}</td><td>${item.message}</td></tr>`).reverse().join('') : '<tr><td colspan="4" class="text-center">No records.</td></tr>';
  }

  function clearAllData() { if(confirm("Clear All?")) { localStorage.removeItem('gh_enquiries'); renderTable(); } }
  window.onload = renderTable;
</script>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
