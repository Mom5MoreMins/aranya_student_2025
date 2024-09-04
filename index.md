---
layout: base
title: Student Home 
description: Home Page
hide: true
---

# The History of Boxing

Boxing, often referred to as the "Sweet Science," has a rich and varied history that spans thousands of years. From its ancient origins to the modern-day spectacle, the sport has evolved significantly.

## Ancient Origins

Boxing is believed to have originated in ancient civilizations, with evidence of the sport appearing in ancient Egypt and Mesopotamia. The earliest depiction of boxing comes from the Sumerian civilization, around 3000 BCE.

![Ancient Egyptian Boxer](https://upload.wikimedia.org/wikipedia/commons/4/49/Ancient_Egyptian_boxer.jpg)
*Ancient Egyptian boxing relief.*

### Greece and Rome

Boxing was formalized in Ancient Greece, with the sport becoming part of the Olympic Games in 688 BCE. The Greeks introduced rules and protective gear, such as the "cestus," a leather strap worn on the hands. The Romans later adopted boxing but incorporated it into their gladiatorial games.

![Ancient Greek Boxing](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a2/Boxing_mosaic.jpg/1024px-Boxing_mosaic.jpg)
*Roman mosaic depicting boxing.*

## The Birth of Modern Boxing

The transition to modern boxing began in the 17th century in England. In 1681, the first recorded boxing match was held, and by the 18th century, the sport began to gain popularity. The Marquis of Queensberry rules, introduced in 1867, formalized the sport and introduced the use of gloves.

![Marquis of Queensberry](https://upload.wikimedia.org/wikipedia/commons/6/60/Marquess_of_Queensberry.jpg)
*John Sholto Douglas, the Marquess of Queensberry.*

### 19th Century Growth

During the 19th century, boxing saw significant growth, with many notable champions emerging. One of the most famous was John L. Sullivan, the first heavyweight champion under the Queensberry rules.

![John L. Sullivan](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a4/John_L._Sullivan_-_full_length_portrait.jpg/800px-John_L._Sullivan_-_full_length_portrait.jpg)
*John L. Sullivan, the first heavyweight champion.*

## 20th Century to Present

The 20th century brought about even more significant changes. Boxing gained international fame with legendary figures like Muhammad Ali, Mike Tyson, and Floyd Mayweather Jr. The sport has become a global phenomenon, with high-profile matches broadcasted worldwide.

### Notable Boxers

#### Muhammad Ali

Known as "The Greatest," Muhammad Ali was famous for his quick footwork and charismatic personality. His fights against Sonny Liston, Joe Frazier, and George Foreman are legendary.

![Muhammad Ali](https://upload.wikimedia.org/wikipedia/commons/thumb/5/54/Muhammad_Ali%2C_1966.jpg/800px-Muhammad_Ali%2C_1966.jpg)
*Muhammad Ali in 1966.*

#### Mike Tyson

Mike Tyson became the youngest heavyweight champion in history at the age of 20. Known for his knockout power, Tyson dominated the sport in the late 1980s.

![Mike Tyson](https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Mike_Tyson_2016.jpg/800px-Mike_Tyson_2016.jpg)
*Mike Tyson in 2016.*

#### Floyd Mayweather Jr.

Floyd Mayweather Jr. is renowned for his defensive skills and undefeated record. He is considered one of the best pound-for-pound fighters in history.

![Floyd Mayweather Jr.](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6c/Floyd_Mayweather_Jr_%2830315188201%29.jpg/800px-Floyd_Mayweather_Jr_%2830315188201%29.jpg)
*Floyd Mayweather Jr. in 2013.*

## The Future of Boxing

As boxing continues to evolve, new technologies, training methods, and emerging stars shape the future of the sport. With its deep history and ongoing developments, boxing remains a dynamic and thrilling sport.

![Modern Boxing](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a7/2017_Mayweather_McGregor.jpg/800px-2017_Mayweather_McGregor.jpg)
*Modern boxing match between Floyd Mayweather Jr. and Conor McGregor.*

---

**Sources:**
- [Ancient Egypt Boxing](https://en.wikipedia.org/wiki/Boxing)
- [Marquis of Queensberry](https://en.wikipedia.org/wiki/Marquess_of_Queensberry)
- [Muhammad Ali](https://en.wikipedia.org/wiki/Muhammad_Ali)
- [Mike Tyson](https://en.wikipedia.org/wiki/Mike_Tyson)
- [Floyd Mayweather Jr.](https://en.wikipedia.org/wiki/Floyd_Mayweather_Jr.)

# Mario Stomping Animation

<div id="container">
  <img id="mario" src="https://e7.pngegg.com/pngimages/517/871/png-clipart-8-bit-super-mario-illustration-super-mario-bros-new-super-mario-bros-video-game-sprite-angle-super-mario-bros-thumbnail.png" alt="Mario" />
  <img id="goomba" src="https://toppng.com/uploads/preview/oomba-8-bit-goomba-11562923680chnjskwjpc.png" alt="Goomba" />
</div>

<style>
  #container {
    position: relative;
    width: 100%;
    height: 200px; /* Adjust as needed */
    overflow: hidden;
    background-color: #87CEEB; /* Sky blue background */
  }
  #mario {
    position: absolute;
    bottom: 0;
    width: 50px;
    transition: transform 0.1s ease-in-out;
  }
  #goomba {
    position: absolute;
    bottom: 0;
    left: 80%;
    width: 50px;
    transition: transform 0.1s ease-in-out, opacity 0.5s ease-in-out;
  }
  .jump {
    transform: translateY(-50px);
  }
  .squish {
    transform: scaleY(0.5);
    opacity: 0;
  }
</style>

<script>
  const mario = document.getElementById('mario');
  const goomba = document.getElementById('goomba');
  let marioPosition = 0;
  let marioDirection = 1;
  const marioJumpHeight = 50;
  const stompInterval = 2000; // Time between stomps (in milliseconds)
  
  function moveMario() {
    marioPosition += 5 * marioDirection;
    if (marioPosition > window.innerWidth || marioPosition < -50) {
      marioDirection *= -1;
    }
    mario.style.transform = `translateX(${marioPosition}px)`;
    
    // Check if Mario is stomping on the Goomba
    if (marioPosition > goomba.offsetLeft - 50 && marioPosition < goomba.offsetLeft + 50) {
      mario.src = "https://e7.pngegg.com/pngimages/771/724/png-clipart-super-mario-bros-3-mario-kart-8-mario-angle-heroes.png"; // Jumping Mario
      mario.classList.add('jump');
      setTimeout(() => {
        mario.classList.remove('jump');
        mario.src = "https://e7.pngegg.com/pngimages/517/871/png-clipart-8-bit-super-mario-illustration-super-mario-bros-new-super-mario-bros-video-game-sprite-angle-super-mario-bros-thumbnail.png"; // Regular Mario
        goomba.classList.add('squish');
        setTimeout(() => {
          goomba.style.display = 'none'; // Hide the Goomba after squishing
        }, 500); // Delay for the squish animation
      }, 100); // Time for Mario's jump
    }
  }
  
  setInterval(moveMario, 50); // Update Mario's position every 50ms
</script>
