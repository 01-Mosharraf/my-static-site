# Hosting a Static Website on GitHub Pages

This project demonstrates how to create and host a **static HTML & CSS website** for free using **GitHub Pages**.

---

## 📌 How It’s Done (Setup Steps)

1. **Create Project Files**
   - Make a folder for your project.
   - Create an `index.html` file:
     ```html
     <!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Stand-Out Website</title>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap" rel="stylesheet">
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <header>
    <h1>Welcome to My Stand-Out Website 🚀</h1>
    <p>Hosted for free on GitHub Pages</p>
  </header>

  <main>
    <section class="card">
      <h2>About Me</h2>
      <p>
        I'm passionate about web development and love creating beautiful, functional websites. 
        This project is my GitHub Pages showcase — fully static designed.
      </p>
    </section>

    <section class="card">
      <h2>My Projects</h2>
      <ul>
        <li>Portfolio Website</li>
        <li>Weather App</li>
        <li>Blog Template</li>
      </ul>
    </section>
  </main>

  <footer>
    <p>© 2025 My Stand-Out Website | Built with GitHub Pages</p>
  </footer>
</body>
</html>
     ```
   - Create a `style.css` file:
    ```css
     /* Global styles */
body {
    margin: 0;
    font-family: 'Poppins', sans-serif;
    background: #f0f0f0;
    color: #333;
  }
  
  /* Header styles */
  header {
    background: linear-gradient(to right, #ff6f61, #d72638);
    color: white;
    text-align: center;
    padding: 60px 20px;
  }
  header h1 {
    font-size: 2.5rem;
    margin: 0;
    animation: fadeInDown 1.5s ease;
  }
  header p {
    margin-top: 10px;
    font-size: 1.2rem;
  }
  
  /* Fade-in animation */
  @keyframes fadeInDown {
    0% {opacity: 0; transform: translateY(-50px);}
    100% {opacity: 1; transform: translateY(0);}
  }
  
  /* Card styles */
  main {
    max-width: 1000px;
    margin: auto;
    padding: 20px;
  }
  .card {
    background: white;
    border-radius: 10px;
    padding: 20px;
    margin: 20px 0;
    box-shadow: 0px 4px 20px rgba(0,0,0,0.1);
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }
  .card:hover {
    transform: translateY(-5px);
    box-shadow: 0px 8px 25px rgba(0,0,0,0.15);
  }
  
  /* Footer */
  footer {
    background: #222;
    color: white;
    text-align: center;
    padding: 15px 10px;
    margin-top: 40px;
  }
  
  /* Responsive design */
  @media (max-width: 600px) {
    header h1 {
      font-size: 1.8rem;
    }
    .card {
      padding: 15px;
    }
  }
    ```

2. **Push Files to GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<repo-name>.git
   git push -u origin main
