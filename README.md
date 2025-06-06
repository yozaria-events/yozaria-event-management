<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Yozaria Event Management</title>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <style>
    :root {
      --primary: #D4AF37; /* Gold */
      --secondary: #FFA500; /* Orange */
      --dark: #000000; /* Black */
      --light: #ffffff; /* White */
    }

    body {
      font-family: 'Montserrat', sans-serif;
      margin: 0;
      padding: 0;
      background-color: var(--light);
      color: var(--dark);
    }

    header {
      background: linear-gradient(135deg, var(--primary), var(--secondary));
      color: var(--light);
      padding: 2rem;
      text-align: center;
    }

    nav {
      display: flex;
      justify-content: center;
      background-color: var(--dark);
    }

    nav a {
      color: var(--light);
      padding: 1rem;
      text-decoration: none;
      transition: background 0.3s;
    }

    nav a:hover {
      background-color: var(--primary);
    }

    section {
      padding: 2rem;
      max-width: 1000px;
      margin: auto;
    }

    .highlight {
      color: var(--secondary);
    }

    .card {
      background-color: var(--light);
      border: 2px solid var(--primary);
      border-radius: 12px;
      padding: 1.5rem;
      margin: 1rem 0;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
    }

    .chart-container {
      width: 100%;
      margin-top: 2rem;
    }

    footer {
      text-align: center;
      padding: 1rem;
      background-color: var(--dark);
      color: var(--light);
    }

    .form-group {
      margin-bottom: 1rem;
    }

    input, textarea {
      width: 100%;
      padding: 0.8rem;
      border: 1px solid var(--primary);
      border-radius: 8px;
    }

    button {
      padding: 0.8rem 1.2rem;
      background-color: var(--secondary);
      border: none;
      color: var(--light);
      border-radius: 8px;
      cursor: pointer;
    }

    button:hover {
      background-color: var(--primary);
    }
  </style>
</head>

<body>
  <header>
    <h1>Yozaria Event Management</h1>
    <p><em>“When You Experience Our Event, It’s Like Tasting the Sweetness of Honey”</em></p>
  </header>

  <nav>
    <a href="#about">About</a>
    <a href="#services">Services</a>
    <a href="#portfolio">Portfolio</a>
    <a href="#testimonials">Testimonials</a>
    <a href="#contact">Contact</a>
  </nav>

  <section id="about">
    <h2>About Us</h2>
    <div class="card">
      <p>Yozaria Event Management is a modern company based in Masaki, Dar es Salaam, Tanzania specializing in Event Conceptualization, Designing, and Planning. We aim to be the most outstanding event management company in East Africa within five years.</p>
    </div>
  </section>

  <section id="services">
    <h2>Our Services</h2>
    <div class="card">
      <ul>
        <li>Event Conceptualization</li>
        <li>Event Designing</li>
        <li>Event Planning</li>
        <li>Event Management Consultancy</li>
        <li>Equipment Rentals</li>
        <li>Theme Advisory</li>
        <li>Tourism-linked Event Packages</li>
        <li>Technology-driven Events</li>
      </ul>
    </div>
  </section>

  <section id="portfolio">
    <h2>Portfolio</h2>
    <div class="card">
      <p>Take a look at some of our past events that captivated hearts and left lasting impressions.</p>
      <img src="https://via.placeholder.com/800x400?text=Event+Showcase+1" alt="Event Example 1" style="width: 100%; border-radius: 8px; margin-top: 1rem;">
    </div>
  </section>

  <section id="testimonials">
    <h2>What Clients Say</h2>
    <div class="card">
      <blockquote>“Yozaria turned our wedding into a magical moment that we’ll never forget. Highly recommended!” – Sarah & James</blockquote>
      <blockquote>“Professionalism at its best. The corporate conference ran flawlessly from start to finish.” – CEO, Global Corp</blockquote>
    </div>
  </section>

  <section class="chart-container">
    <h2>Growth Projection</h2>
    <canvas id="growthChart"></canvas>
    <script>
      const ctx = document.getElementById('growthChart').getContext('2d');
      const growthChart = new Chart(ctx, {
        type: 'line',
        data: {
          labels: ['2025', '2026', '2027', '2028', '2029'],
          datasets: [{
            label: 'Events Managed',
            data: [50, 120, 200, 260, 300],
            borderColor: '#D4AF37',
            backgroundColor: 'rgba(255, 215, 0, 0.2)',
            borderWidth: 3,
            fill: true,
            tension: 0.3
          }]
        },
        options: {
          scales: {
            y: {
              beginAtZero: true
            }
          },
          plugins: {
            legend: {
              labels: {
                color: '#000'
              }
            }
          }
        }
      });
    </script>
  </section>

  <section id="contact">
    <h2>Contact Us</h2>
    <div class="card">
      <form>
        <div class="form-group">
          <label for="name">Full Name</label>
          <input type="text" id="name" name="name" required>
        </div>
        contact 255785460224
        <div class="form-group">
          <label for="email">Email</label> stephanoy99@gmail.com
          <input type="email" id="email" name="email" required>
        </div>
        <div class="form-group">
          <label for="message">Message</label>
          <textarea id="message" name="message" rows="5" required></textarea>
        </div>
        <button type="submit">Send Message</button>
      </form>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 Yozaria Event Management. All rights reserved.</p>
  </footer>
</body>

</html>

