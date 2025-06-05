/* Reset e estilos base */
:root {
  --primary-color: #2b8a3e;
  --secondary-color: #37b24d;
  --dark-color: #1a3a20;
  --light-color: #f8f9fa;
  --text-color: #333;
  --text-light: #666;
  --white: #fff;
  --shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  --transition: all 0.3s ease;
}

* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: 'Poppins', sans-serif;
  line-height: 1.6;
  color: var(--text-color);
  background-color: var(--light-color);
}

h1, h2, h3, h4 {
  font-family: 'Montserrat', sans-serif;
  font-weight: 700;
}

a {
  text-decoration: none;
  color: inherit;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

/* Header */
header {
  background-color: var(--white);
  box-shadow: var(--shadow);
  position: sticky;
  top: 0;
  z-index: 100;
}

.header-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px 0;
}

.logo {
  text-align: center;
  margin-bottom: 20px;
}

.logo h1 {
  font-size: 2.5rem;
  color: var(--primary-color);
  margin-bottom: 5px;
}

.logo p {
  font-size: 1rem;
  color: var(--text-light);
  font-style: italic;
}

/* Menu */
.menu {
  display: flex;
  list-style: none;
  gap: 30px;
}

.menu li a {
  font-weight: 600;
  font-size: 1.1rem;
  padding: 10px 0;
  position: relative;
  transition: var(--transition);
  color: var(--dark-color);
}

.menu li a:hover {
  color: var(--primary-color);
}

.menu li a::after {
  content: '';
  position: absolute;
  width: 0;
  height: 2px;
  background-color: var(--primary-color);
  bottom: 0;
  left: 0;
  transition: var(--transition);
}

.menu li a:hover::after {
  width: 100%;
}

/* Hero Section */
.hero {
  background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), 
              url('https://via.placeholder.com/1920x1080?text=Pecuária+Tecnológica');
  background-size: cover;
  background-position: center;
  height: 80vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: var(--white);
  padding: 0 20px;
}

.hero-content h2 {
  font-size: 3rem;
  margin-bottom: 20px;
  line-height: 1.2;
}

.hero-content p {
  font-size: 1.5rem;
  margin-bottom: 30px;
  max-width: 700px;
}

.btn {
  display: inline-block;
  background-color: var(--primary-color);
  color: var(--white);
  padding: 12px 30px;
  border-radius: 50px;
  font-weight: 600;
  transition: var(--transition);
  border: 2px solid var(--primary-color);
}

.btn:hover {
  background-color: transparent;
  color: var(--primary-color);
}

/* Technologies Section */
.technologies {
  padding: 80px 0;
  background-color: var(--white);
}

.technologies h2 {
  text-align: center;
  font-size: 2.5rem;
  margin-bottom: 50px;
  color: var(--dark-color);
  position: relative;
}

.technologies h2::after {
  content: '';
  display: block;
  width: 80px;
  height: 4px;
  background-color: var(--primary-color);
  margin: 15px auto 0;
}

.tech-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 30px;
  margin-top: 40px;
}

.tech-card {
  background-color: var(--light-color);
  border-radius: 10px;
  padding: 30px;
  text-align: center;
  transition: var(--transition);
  box-shadow: var(--shadow);
}

.tech-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
}

.tech-card i {
  font-size: 3rem;
  color: var(--primary-color);
  margin-bottom: 20px;
}

.tech-card h3 {
  font-size: 1.5rem;
  margin-bottom: 15px;
  color: var(--dark-color);
}

.tech-card p {
  color: var(--text-light);
  margin-bottom: 20px;
}

.btn-small {
  display: inline-block;
  background-color: var(--primary-color);
  color: var(--white);
  padding: 8px 20px;
  border-radius: 50px;
  font-size: 0.9rem;
  transition: var(--transition);
}

.btn-small:hover {
  background-color: var(--dark-color);
}

/* About Section */
.about {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 50px;
  padding: 80px 0;
  align-items: center;
}

.about-content h2 {
  font-size: 2.5rem;
  margin-bottom: 20px;
  color: var(--dark-color);
}

.about-content p {
  margin-bottom: 30px;
  font-size: 1.1rem;
  line-height: 1.8;
}

.stats {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 20px;
  margin-top: 40px;
}

.stat-item {
  text-align: center;
}

.stat-number {
  display: block;
  font-size: 2rem;
  font-weight: 700;
  color: var(--primary-color);
  margin-bottom: 5px;
}

.stat-label {
  font-size: 0.9rem;
  color: var(--text-light);
}

.about-image img {
  width: 100%;
  border-radius: 10px;
  box-shadow: var(--shadow);
}

/* Footer */
footer {
  background-color: var(--dark-color);
  color: var(--white);
  padding: 60px 0 0;
}

.footer-container {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 40px;
  margin-bottom: 40px;
}

.footer-logo h3 {
  font-size: 1.8rem;
  margin-bottom: 10px;
  color: var(--white);
}

.footer-logo p {
  color: rgba(255, 255, 255, 0.7);
}

.footer-links h4, .footer-contact h4 {
  font-size: 1.3rem;
  margin-bottom: 20px;
  color: var(--white);
}

.footer-links ul {
  list-style: none;
}

.footer-links li {
  margin-bottom: 10px;
}

.footer-links a {
  color: rgba(255, 255, 255, 0.7);
  transition: var(--transition);
}

.footer-links a:hover {
 
