# Fishing
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-color: #0b1c2d;
  color: #ffffff;
  line-height: 1.6;
}

/* Header Styles */
header {
  background: linear-gradient(135deg, #001f3f 0%, #003366 100%);
  padding: 1rem 2rem;
  text-align: center;
  position: sticky;
  top: 0;
  z-index: 1000;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
}

header h1 {
  margin: 0;
  font-size: 2.5rem;
  color: #7fdbff;
}

header h1 i {
  margin-right: 10px;
}

nav {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 1.5rem;
  margin-top: 1rem;
}

nav a {
  color: #7fdbff;
  text-decoration: none;
  font-weight: 600;
  padding: 0.5rem 1rem;
  border-radius: 50px;
  transition: all 0.3s ease;
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

nav a:hover {
  background-color: rgba(127, 219, 255, 0.2);
  transform: translateY(-2px);
}

nav a.active {
  background-color: #7fdbff;
  color: #001f3f;
}

/* Hero Section */
.hero {
  padding: 6rem 2rem;
  text-align: center;
  background: linear-gradient(rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0.7)),
              url('https://images.unsplash.com/photo-1507525428034-b723cf961d3e?w=1600&fit=crop');
  background-size: cover;
  background-position: center;
  background-attachment: fixed;
}

.hero h2 {
  font-size: 3rem;
  margin-bottom: 1rem;
  color: #7fdbff;
}

.hero p {
  font-size: 1.2rem;
  max-width: 600px;
  margin: 0 auto 2rem;
  color: #cce6ff;
}

.cta-button {
  display: inline-block;
  background: linear-gradient(135deg, #2c5282 0%, #4299e1 100%);
  color: white;
  padding: 1rem 2rem;
  border-radius: 50px;
  text-decoration: none;
  font-weight: bold;
  transition: all 0.3s ease;
  border: none;
  cursor: pointer;
}

.cta-button:hover {
  transform: translateY(-3px);
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
}

/* Section Styles */
section {
  padding: 4rem 2rem;
  max-width: 1200px;
  margin: 0 auto;
}

section h3 {
  color: #7fdbff;
  margin-bottom: 2rem;
  font-size: 2rem;
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

/* Cards */
.cards {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2rem;
}

.card {
  background: linear-gradient(145deg, #102a43, #0b1c2d);
  padding: 2rem;
  border-radius: 15px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.4);
  transition: all 0.3s ease;
  border: 1px solid #2c5282;
}

.card:hover {
  transform: translateY(-10px);
  box-shadow: 0 15px 40px rgba(0, 0, 0, 0.5);
  border-color: #7fdbff;
}

.card h4 {
  color: #7fdbff;
  margin-bottom: 1rem;
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

/* Gallery */
.gallery-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}

.gallery-grid img {
  width: 100%;
  height: 200px;
  object-fit: cover;
  border-radius: 10px;
  transition: all 0.3s ease;
  border: 3px solid transparent;
}

.gallery-grid img:hover {
  transform: scale(1.05);
  border-color: #7fdbff;
}

/* Contact Form */
.contact-form {
  max-width: 600px;
  margin: 2rem auto;
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.contact-form input,
.contact-form textarea {
  padding: 1rem;
  border: 2px solid #2c5282;
  border-radius: 10px;
  background-color: rgba(16, 42, 67, 0.8);
  color: white;
  font-size: 1rem;
  transition: border-color 0.3s ease;
}

.contact-form input:focus,
.contact-form textarea:focus {
  outline: none;
  border-color: #7fdbff;
}

.contact-form button {
  background: linear-gradient(135deg, #2c5282 0%, #4299e1 100%);
  color: white;
  border: none;
  padding: 1rem;
  border-radius: 10px;
  font-size: 1.1rem;
  font-weight: bold;
  cursor: pointer;
  transition: all 0.3s ease;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
}

.contact-form button:hover {
  transform: translateY(-2px);
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
}

.contact-info {
  text-align: center;
  margin-top: 3rem;
  color: #cce6ff;
}

.contact-info p {
  margin: 0.5rem 0;
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
}

/* Footer */
footer {
  background: linear-gradient(135deg, #001427 0%, #000814 100%);
  text-align: center;
  padding: 2rem;
  color: #cce6ff;
  margin-top: 4rem;
}

footer i {
  color: #ff6b6b;
  margin: 0 0.5rem;
}

/* Mobile Responsive */
@media (max-width: 768px) {
  header h1 {
    font-size: 2rem;
  }
  
  nav {
    gap: 0.5rem;
  }
  
  nav a {
    padding: 0.4rem 0.8rem;
    font-size: 0.9rem;
  }
  
  .hero {
    padding: 4rem 1rem;
  }
  
  .hero h2 {
    font-size: 2rem;
  }
  
  section {
    padding: 3rem 1rem;
  }
  
  .gallery-grid {
    grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
  }
}
