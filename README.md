<style>
/* Эффект печатной машинки */
.typewriter {
  overflow: hidden;
  border-right: .15em solid orange;
  white-space: nowrap;
  animation:
    typing 3.5s steps(22, end),
    blink-caret .75s step-end infinite;
  font-family: monospace;
  font-size: 24px;
  color: #f90;
}

/* Анимация печати */
@keyframes typing {
  from { width: 0 }
  to { width: 22ch }
}

/* Мигающий курсор */
@keyframes blink-caret {
  from, to { border-color: transparent }
  50% { border-color: orange; }
}

/* Стирание текста */
.erase {
  animation: erase 1.5s forwards;
  animation-delay: 3.5s;
  white-space: nowrap;
  border-right: none;
  font-family: monospace;
  font-size: 24px;
  color: #f90;
}

@keyframes erase {
  from { width: 22ch; opacity: 1; }
  to { width: 0; opacity: 0; }
}

/* Эффект глитча */
.glitch {
  font-family: 'Courier New', Courier, monospace;
  font-size: 28px;
  color: #0ff;
  position: relative;
  animation: glitch-anim 1s infinite;
  animation-delay: 5s;
  opacity: 0;
  animation-fill-mode: forwards;
}

@keyframes glitch-anim {
  0% {
    opacity: 0;
    text-shadow: none;
  }
  10% {
    opacity: 1;
    text-shadow:
      2px 0 red,
      -2px 0 cyan;
  }
  20% {
    text-shadow:
      -2px 0 red,
      2px 0 cyan;
  }
  30% {
    text-shadow:
      2px 2px red,
      -2px -2px cyan;
  }
  40% {
    text-shadow:
      -2px -2px red,
      2px 2px cyan;
  }
  50% {
    text-shadow:
      2px 0 red,
      -2px 0 cyan;
  }
  60% {
    text-shadow:
      -2px 0 red,
      2px 0 cyan;
  }
  70% {
    text-shadow:
      2px 2px red,
      -2px -2px cyan;
  }
  80% {
    text-shadow:
      -2px -2px red,
      2px 2px cyan;
  }
  90% {
    opacity: 1;
    text-shadow:
      2px 0 red,
      -2px 0 cyan;
  }
  100% {
    opacity: 1;
    text-shadow: none;
  }
}
</style>

<div class="typewriter">Welcome to My Profile</div>
<div class="erase">Welcome to My Profile</div>
<div class="glitch">I am xfau1ty</div>
