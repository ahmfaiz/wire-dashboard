<div align="center">
  <h3>Part of:</h3>
  <img width="150" src="https://github.com/ahmfaiz/wire-scraper/blob/main/wire-logo-rounded-small.png" alt="wire-logo" />
  <h1>The <a href="https://github.com/ahmfaiz?tab=repositories&q=wire&type=&language=&sort=">WIRE</a> Project</h1>
  <p>
    Web Info Retrieval Engine
  </p>
  <a href="https://opensource.org/">
    <img src="https://badges.frapsoft.com/os/v3/open-source.svg?v=103" alt="Open Source Love" />
  </a>
  <a href="https://opensource.org/license/gpl-3.0/">
    <img src="https://img.shields.io/badge/license-GPLv3-blue" alt="License" />
  </a>
</div>

![](https://i.imgur.com/waxVImv.png)

<div align="center">
  <h3>Part of:</h3>
  <img width="150" src="https://github.com/ahmfaiz/wire-scraper/blob/main/wire-logo-rounded-small.png" alt="wire-logo" />
  <h1>The <a href="https://github.com/ahmfaiz?tab=repositories&q=wire&type=&language=&sort=">WIRE</a> Project</h1>
  <p>
    Web Info Retrieval Engine
  </p>
  <a href="https://opensource.org/">
    <img src="https://badges.frapsoft.com/os/v3/open-source.svg?v=103" alt="Open Source Love" />
  </a>
  <a href="https://opensource.org/license/gpl-3.0/">
    <img src="https://img.shields.io/badge/license-GPLv3-blue" alt="License" />
  </a>
</div>

![](https://i.imgur.com/waxVImv.png)

<h1>Web Dashboard</h1>


    <h1 id="text" >Your Text</h1>

<a href="https://github.com/nitin611/wire-dashboard" style="text-decoration: none; font-size: 38px;">Github link</a>

  <script>
    const textDisplay = document.getElementById('text')
const phrases = ['Hello my name is Nitin.', 'I am contributing as a web developer.','Thank you😊']
let i = 0
let j = 0 
let currentPhrase = []
let isDeleting = false
let isEnd = false

function loop () {
  isEnd = false
  textDisplay.innerHTML = currentPhrase.join('')

  if (i < phrases.length) {

    if (!isDeleting && j <= phrases[i].length) {
      currentPhrase.push(phrases[i][j])
      j++
      textDisplay.innerHTML = currentPhrase.join('')
    }

    if(isDeleting && j <= phrases[i].length) {
      currentPhrase.pop(phrases[i][j])
      j--
      textDisplay.innerHTML = currentPhrase.join('')
    }

    if (j == phrases[i].length) {
      isEnd = true
      isDeleting = true
    }

    if (isDeleting && j === 0) {
      currentPhrase = []
      isDeleting = false
      i++
      if (i === phrases.length) {
        i = 0
      }
    }
  }
  const spedUp = Math.random() * (80 -50) + 50
  const normalSpeed = Math.random() * (300 -200) + 200
  const time = isEnd ? 2000 : isDeleting ? spedUp : normalSpeed
  setTimeout(loop, time)
}

loop()
  </script>
