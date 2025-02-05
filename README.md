<br>

<div class="star-container">
  <img src="assets/image.png" width="150" align="center">
  <div class="stars"></div>
</div>

<style>
.star-container {
  position: relative;
  display: block;
  margin-left: auto;
  margin-right: auto;
  width: fit-content;
}

.stars {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  pointer-events: none;
  overflow: hidden;
}

.stars::before, .stars::after {
  content: '✨';
  position: absolute;
  animation: sparkle 2s infinite;
}

.stars::before {
  top: 10%;
  left: 10%;
  animation-delay: 0s;
}

.stars::after {
  bottom: 10%;
  right: 10%;
  animation-delay: 1s;
}

@keyframes sparkle {
  0%, 100% { opacity: 0; transform: scale(0.5); }
  50% { opacity: 1; transform: scale(1); }
}
</style>

<br>

```python
class AboutMe:
  user = 'Chrysanthi'
  occupation  = 'BSc (Hons) Student'
  hobbies = [
    'Watching films',
    'Reading',
    'Playing the drums'
  ]

 def getPronouns():
   return she_her()

 def getLocation():
   return Groningen_Netherlands()
```