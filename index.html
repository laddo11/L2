const dur = 6 + Math.random() * 5;
  b.style.animationDuration = dur + 's';
  document.body.appendChild(b);
  setTimeout(() => b.remove(), dur * 1000);
}
setInterval(() => { if (s2Active) balloon(); }, 700);

/* ---------- Heart burst ---------- */
function burst(x, y, n = 24) {
  const E = ["💖","💕","💗","💛","✨","🌸","🦋"];
  for (let i = 0; i < n; i++) {
    const h = document.createElement('div');
    h.className = 'float';
    h.textContent = E[Math.floor(Math.random() * E.length)];
    h.style.left = x + 'px'; h.style.top = y + 'px';
    h.style.fontSize = 16 + Math.random() * 22 + 'px';
    document.body.appendChild(h);
    const ang = Math.random() * Math.PI * 2;
    const dist = 80 + Math.random() * 180;
    h.animate([
      { transform: 'translate(-50%,-50%) scale(.3)', opacity: 1 },
      { transform: translate(calc(-50% + ${Math.cos(ang)*dist}px), calc(-50% + ${Math.sin(ang)*dist - 80}px)) scale(1.2), opacity: 0 }
    ], { duration: 1400 + Math.random() * 800, easing: 'cubic-bezier(.2,.8,.3,1)' }).onfinish = () => h.remove();
  }
}
document.addEventListener('pointerdown', e => {
  if (e.target.closest('.card') || e.target.closest('button')) return;
  burst(e.clientX, e.clientY, 10);
});

/* ---------- Surprise card (part 1) ---------- */
const overlay = $('overlay'), cardText = $('card-text');
let typer;
$('open').addEventListener('click', () => {
  overlay.classList.add('show');
  cardText.textContent = "";
  clearInterval(typer);
  let i = 0;
  typer = setInterval(() => {
    cardText.textContent += SURPRISE[i++] || "";
    if (i >= SURPRISE.length) clearInterval(typer);
  }, 45);
  burst(innerWidth / 2, innerHeight / 2, 40);
});
$('close').addEventListener('click', () => overlay.classList.remove('show'));

/* ---------- Navigation between parts ---------- */
$('next').addEventListener('click', () => s2.scrollIntoView({ behavior: 'smooth' }));
$('back').addEventListener('click', () => s1.scrollIntoView({ behavior: 'smooth' }));

/* ---------- Confetti ---------- */
function confettiRain(count = 140) {
  const colors = ["#ff6a88","#ffd54a","#6ee7b7","#60a5fa","#c084fc","#fff","#ff9a3c"];
  for (let i = 0; i < count; i++) {
    const c = document.createElement('div');
    c.className = 'confetti';
    const size = 6 + Math.random() * 8;
    c.style.width = size + 'px';
    c.style.height = size * (Math.random() > .5 ? 1 : 2.2) + 'px';
    c.style.background = colors[Math.floor(Math.random() * colors.length)];
    c.style.borderRadius = Math.random() > .6 ? '50%' : '2px';
    c.style.left = Math.random() * 100 + 'vw';
    c.style.setProperty('--dx', (Math.random() * 240 - 120) + 'px');
    c.style.setProperty('--rot', (Math.random() * 1080 - 540) + 'deg');
    const dur = 2.5 + Math.random() * 3;
    c.style.animationDuration = dur + 's';
    c.style.animationDelay = (Math.random() * 1.2) + 's';
    document.body.appendChild(c);
    setTimeout(() => c.remove(), (dur + 1.5) * 1000);
  }
}
function celebrate() {
  confettiRain(140);
  setTimeout(() => confettiRain(100), 900);
  burst(innerWidth / 2, innerHeight / 2, 40);
}
$('celebrate').addEventListener('click', celebrate);

/* ---------- Detect which part is on screen ---------- */
const io = new IntersectionObserver(entries => {
  entries.forEach(e => {
    const on = e.intersectionRatio > 0.55;
    if (e.target === s2) {
      s2Active = on;
      if (on) {
        s2.classList.add('in');
        if (!celebrated) { celebrated = true; setTimeout(celebrate, 900); }
      }
    } else {
      s1Active = on;
    }
  });
}, { threshold: [0, 0.55, 1] });
io.observe(s1); io.observe(s2);
</script>
</body>
</html>
