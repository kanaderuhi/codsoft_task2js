<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Personal Portfolio</title>
      <style>
        body
        {
          background-color: beige;
          font-family: Arial, sans-serif;
          margin: 0;
          padding: 0;
        }
          
        header 
        {
          background-color: #e0b90d;
          color: #000000;
          padding: 1em;
          text-align: center;
        }
          
        nav ul 
        {
          list-style: none;
          margin: 0;
          padding: 0;
          display: flex;
          justify-content: space-between;
        }
          
        nav li 
        {
          margin-right: 20px;
        }
          
        nav a 
        {
          color: #000000;
          text-decoration: none;
        }
          
        main 
        {
          display: flex;
          flex-direction: column;  
          align-items: center;
          padding: 2em;
        }
          
        section 
        {
          background-color: bisque;
          padding: 2em;
          margin-bottom: 20px;
          box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
          
        h1 
        {
          font-size: 24px;
          margin-top: 0;
        }
          
        #projects ul 
        {
          list-style: none;
          margin: 0;
          padding: 0;
        }
          
        #projects li 
        {
          margin-bottom: 20px;
        }
          
        #skills ul 
        {
          list-style: none;
          margin: 0;
          padding: 0;
        }
          
        #skills li 
        {
          margin-bottom: 10px;
        }
          
        #skills li:before 
        {
          content: "\2713";
          font-size: 18px;
          color: #333;
          margin-right: 10px;
        }
          
        #contact 
        {
          background-color: bisque;
          padding: 2em;
          margin-bottom: 20px;
          box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }
          
          #contact h2 
          {
            margin-top: 0;
          }
          
          #contact p 
          {
            margin-bottom: 20px;
          }
          
          #contact a 
          {
            color: #337ab7;
            text-decoration: none;
          }
          
          #contact a:hover
           {
            color: #23527c;
          }
          
          
          @media (max-width: 768px) 
          {
            main 
            {
              flex-direction: column;
            }
            nav ul {
              flex-direction: column;
            }
            nav li {
              margin-right: 0;
            }
            #projects ul {
              flex-direction: column;
            }
            #projects li {
              margin-bottom: 20px;
            }
          }
          
          
      </style>
    </head>
<body>
  <header>
    <nav>
      <ul>
        <li><a href="#about">About</a></li>
        <li><a href="#projects">Projects</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>
  <main>
    <section id="about">
      <h1><u>ABOUT ME</u></h1>
      <p>HELLO!!!<br>
        I am a student currently pursuing Bachelors' in Information Technology.<br> 
        I am also looking forward to extend my knowledge in web developing hence have been looking up for various internships online as well as offline.
      </p>
    </section>
    <section id="projects">
      <h1><u>PROJECTS</u></h1>
      <ul>
        <li>
          <h2>Project 1</h2>
          <p>Following is my first task of a web-based "TO-DO-LIST"<br>
            Here,the user can manage his tasks that are to be carried throughout the day.<br>
          </p>
          
          <a href="https://github.com/kanaderuhi/codsoft_task1js">View on GitHub</a>
        </li>
        <li>
          <h2>Project 2</h2>
          <p>This project is a digital clock that updates in real time</p>
          <a href="https://github.com/kanaderuhi/codsoft_task2js">View on GitHub</a>
        </li>
      </ul>
    </section>
    <section id="skills">
      <h1><u>SKILLS</u></h1>
      <ul>
        <li>HTML</li>
        <li>CSS</li>
        <li>JavaScript</li>
        <li>Python</li>
        <li>Java</li>
      </ul>
    </section>
    <section id="contact">
      <h1><U>CONTACT</U></h1>
      <form>
        <label for="name">Name:</label>
        <input type="text" id="name" name="name"><br><br>
        <label for="email">Email:</label>
        <input type="email" id="email" name="email"><br><br>
        <label for="message">Message:</label>
        <textarea id="message" name="message"></textarea><br><br>
        <input type="submit" value="Send">
      </form>
    </section>
  </main>
  <script>
    function animateOnScroll() {
      sections.forEach(section => {
        const sectionTop = section.offsetTop;
        const sectionHeight = section.offsetHeight;
        const windowHeight = window.innerHeight;
        const windowScrollTop = window.scrollY;
    
        if (windowScrollTop > (sectionTop + sectionHeight - windowHeight)) {
          section.classList.add(animationClass);
        } else {
          section.classList.remove(animationClass);
        }
      });
    }
    
    window.addEventListener('scroll', animateOnScroll);
    
    const form = document.querySelector('form');
    const nameInput = document.querySelector('#name');
    const emailInput = document.querySelector('#email');
    const messageInput = document.querySelector('#message');
    
  </script>
</body>
</html>s
