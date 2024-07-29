<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Latest Medium Posts</title>
  <style>
    .post {
      border: 1px solid #ddd;
      margin: 10px;
      padding: 10px;
      border-radius: 5px;
    }
    .post h2 {
      margin: 0 0 10px;
    }
    .post p {
      margin: 0 0 10px;
    }
    .post a {
      text-decoration: none;
      color: #007acc;
    }
  </style>
</head>
<body>

<div id="medium-posts"></div>

<script>
  document.addEventListener('DOMContentLoaded', function () {
    fetch('https://api.rss2json.com/v1/api.json?rss_url=https://medium.com/feed/@code2point0')
      .then(response => response.json())
      .then(data => {
        const items = data.items;
        let html = '<div align="center">';
        items.forEach((el, index) => {
          if (index < 4) { // limit to 4 posts
            html += `
              <div class="post">
                <h2>${el.title}</h2>
                <p>${el.description}</p>
                <a href="${el.link}" target="_blank">Read more</a>
              </div>
              <hr />
            `;
          }
        });
        html += '</div>';
        document.getElementById('medium-posts').innerHTML = html;
      });
  });
</script>

<h2 align="left">Hi 👋! My name is ... and I'm a ..., from ....</h2>

###

<div align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=code2point0&hide_title=false&hide_rank=false&show_icons=true&include_all_commits=true&count_private=true&disable_animations=false&theme=dracula&locale=en&hide_border=false" height="150" alt="stats graph"  />
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=code2point0&locale=en&hide_title=false&layout=compact&card_width=320&langs_count=5&theme=dracula&hide_border=false" height="150" alt="languages graph"  />
</div>

###

<img align="right" height="150" src="https://i.imgflip.com/65efzo.gif"  />

###

<div align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="30" alt="javascript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/typescript/typescript-original.svg" height="30" alt="typescript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" height="30" alt="react logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" height="30" alt="html5 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" height="30" alt="css3 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" height="30" alt="python logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" height="30" alt="csharp logo"  />
</div>

###

<div align="left">
  <a href="https://www.youtube.com/channel/UCNcwrHZvqU9UGe8aTaOrGIg" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Youtube&logo=youtube&label=&color=FF0000&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="youtube logo"  />
  </a>
  <a href="mailto:aaziapk6@gmail.com" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Gmail&logo=gmail&label=&color=D14836&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="gmail logo"  />
  </a>
  <a href="https://www.linkedin.com/in/ahmad2point0" target="_blank">
    <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="linkedin logo"  />
  </a>
  <a href="https://www.instagram.com/code2point0/" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Instagram&logo=instagram&label=&color=E4405F&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="instagram logo"  />
  </a>
  <a href="https://medium.com/@code2point0" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Medium&logo=medium&label=&color=12100E&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="medium logo"  />
  </a>
  <a href="https://www.facebook.com/code2point0/" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Facebook&logo=facebook&label=&color=1877F2&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="facebook logo"  />
  </a>
  <a href="https://stackoverflow.com/users/26371590/code2point0" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Stackoverflow&logo=stackoverflow&label=&color=FE7A16&logoColor=white&labelColor=&style=for-the-badge" height="35" alt="stackoverflow logo"  />
  </a>
</div>

###

<br clear="both">

<img src="https://raw.githubusercontent.com/taozhi8833998/taozhi8833998/output/github-contribution-grid-snake-dark.svg" alt="Snake animation" />

###

<div align="center">
  <iframe src="https://medium.com/@code2point0/latest" width="600" height="400"></iframe>
</div>

</body>
</html>
