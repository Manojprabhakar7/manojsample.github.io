-html-

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>My Portfolio</title>
  <link rel="stylesheet" href="style.css"> 
</head>
<body>
  <header>
    <div class="container">
      <h1>MANOJ PRABHAKAR</h1>
      <img src="dp.png" alt="my photo">
      <nav>
        <ul>
          <li><a href="#home">Home</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#portfolio">Portfolio</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </div>
  </header>
  <section id="about">
    <div class="container">
      <h2>About Me</h2>
      <p>Hello, I'm Manoj Prabhakar. Graduating with a degree in Electronics and Communications in 2022 marked the beginning of my journey into the world of technology. Currently, I'm a student at Sacred Heart University, pursuing a course in Computer Science. Alongside my academic pursuits, I've delved into programming languages like C++, HTML, CSS. These languages have empowered me to craft basic websites and kindled my ambition to become a full-stack developer.

        My passion lies in creating immersive digital experiences, whether it's through websites, web applications, or mobile applications. I'm dedicated to honing my skills and knowledge to realize this goal. .</p>
    </div>
  </section>

  <section id="portfolio">
    <div class="container">
      <h2>Portfolio</h2>
      <div class="portfolio-grid">
        <div class="project">
          <img src="./p1r.jpg" alt="Project 1">
          <h3>Project 1- FOG DETECTION AND ELIMINATION BY VIDEO SURVEILLANCE 
            USING RASPBERRY PI.</h3>
          <p>Description:
            An advanced driving assistance system must also consider the weather 
            conditions. One of the most dangerous weather conditions for driving 
            scenarios is the presence of fog. So, an important task for driving 
            assistance system is to detect the presence of fog estimate the fog’s density 
            and determine the visibility of the driver. Our method is an improvement 
            over existing fog detection solutions in terms of speed and accuracy. We 
            can detect daytime fog in a wide range of scenarios. The main objective 
            of this project is to avoid accidents. When there is heavy fog on the road 
            accidents may occur due to non visibility of the moving vehicles and 
            obstacles on the road. In this project we place a single in-vehicle camera
            in front of the car which visualizes and detects the fog, vehicles, and 
            obstacles. We are implementing this project by using raspberry-pi. By 
            using open cv and image
            processing techniques it eliminates the fog up to 75% and assists by 
            displaying the corresponding information to the driver by which accidents 
            may reduce.</p>
        </div>
        <div class="project">
          <img src="./p2 (1).jpg" alt="Project 2">
          <h3>Project 2- Face detection and recognition</h3>
          <p>Surveillance methods that use face detection and recognition are very common. They recognise and examine distinguishing facial features. Face detection using principal component analysis is an effective method. It has multiple uses, such as image compression and object recognition. The primary components of an effective face detection and recognition project include an algorithm that creates a faceprint, a camera to take the image of the face, a database of stored images of faces for comparison, and an algorithm to compare the captured image with the database.

            You can also create a program to detect facial expressions for analysing emotions based on touchpoints of the face and programmed algorithms. .</p>
        </div>
        <div class="project">
          <img src="./p3 (2).jpg" alt="Project 3">
          <h3>Project 3- Online auction system</h3>
          <p>An online auction system allows people to access an auction virtually. Buyers from various places can view the sellers' goods or services, which increases a business's exposure significantly. Ideally, your project will have fraud detection capabilities to create a safe online auction system that allows only authorised users to log in and place bids.</p>
        </div>
      </div>
    </div>
  </section>

  <section id="contact">
    <div class="container">
      <h2>Contact Me</h2>
      <form action="#" method="post">
        <div class="form-group">
          <label for="name">Name:</label>
          <input type="text" id="name" name="name" required>
        </div>
        <div class="form-group">
          <label for="email">Email:</label>
          <input type="email" id="email" name="email" required>
        </div>
        <div class="form-group">
          <label for="message">Message:</label>
          <textarea id="message" name="message" rows="4" required></textarea>
        </div>
        <button type="submit">Send</button>
      </form>
    </div>
  </section>

</body>
</html>

-css-

body {
  margin: 0;
  padding: 0;
  font-family: Arial, sans-serif;
  background-color: #f1eaea; 
  background-image: url(back2.jpg) ;
  

}

.container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
  
}


header {
  background-color: hwb(0 9% 91%);
  color: #fff;
  padding: 20px 0;
}

header h1 {
  margin: 0;
}

nav ul {
  list-style: none;
  padding: 0;
}

nav ul li {
  display: inline;
  margin-right: 20px;
}

nav ul li a {
  text-decoration: none;
  color: #fff;
}

nav ul li a:hover {
  color: #ffd700; 
}

section {
  padding: 40px 0;
}

section h2 {
  margin-top: 1;
}

.portfolio-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  grid-gap: 20px;
  color: #555;
}

.project {
  border: 1px solid #ccc;
  padding: 30px;
  color: black;
}

.form-group {
  margin-bottom: 20px;
}

label {
  display: block;
  margin-bottom: 5px;
}

input,
textarea {
  width: 100%;
  padding: 10px;
  border: 1px solid #ccc;
  border-radius: 5px;
}

button {
  padding: 10px 20px;
  background-color: #333;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

button:hover {
  background-color: #555;
}


@media (max-width: 768px) {
  header {
    text-align: center;
  }

  nav ul li {
    display: block;
    margin-bottom: 10px;
  }

  .portfolio-grid {
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
  }
}

