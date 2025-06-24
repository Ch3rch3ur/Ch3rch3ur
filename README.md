<h1 align="center">Hi, I'm <span style="color:#38bdf8;">Ch3rch3ur</span> 👨‍💻</h1>

<p align="center">
  <em>Un explorateur du code qui transforme la complexité en élégance.</em><br>
  <em>Actuellement en BTS CIEL option Informatique & Réseaux.</em>
</p>

<div align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=38BDF8&width=435&lines=Code+sans+prise+de+t%C3%AAte+;Build.+Test.+Deploy.;Exploring+Java+universes" alt="Typing SVG" />
</div>

---

## 🚀 À propos de moi

🎓 Étudiant en 2ᵉ année de **BTS CIEL IR**, je me spécialise dans les architectures logicielles **N-Tiers** et la manipulation de **Java Enterprise**.  
🧠 J'aime construire des applis efficaces, modulaires et bien pensées, **sans prise de tête**.  
🔍 Toujours à la recherche de nouvelles idées et approches simples pour résoudre des problèmes complexes.

---

## 🛠️ Stack actuelle

| Langages & Outils | Description |
|------------------|-------------|
| ![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=java&logoColor=white) | Back-end solide & objets bien encapsulés |
| ![Maven](https://img.shields.io/badge/Maven-C71A36?style=for-the-badge&logo=apachemaven&logoColor=white) | Build tool de confiance |
| ![NetBeans](https://img.shields.io/badge/NetBeans-1B6AC6?style=for-the-badge&logo=apachenetbeanside&logoColor=white) | IDE maison |
| ![Wildfly](https://img.shields.io/badge/Wildfly-000000?style=for-the-badge&logo=wildfly&logoColor=white) | Serveur JEE |
| N-Tiers 3 niveaux | Physique, Métier, Client — bien séparés |
| Beans & Servlets | L’essence du JEE maîtrisée |

---

## 📊 GitHub Stats

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Ch3rch3ur&show_icons=true&theme=tokyonight&hide_border=true" />
  <br>
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Ch3rch3ur&layout=compact&theme=tokyonight&hide_border=true" />
</p>

---

## 🌀 Petit bonus interactif

```html
<!-- Snack interactif avec la souris -->
<canvas id="canvas"></canvas>
<script>
  const canvas = document.getElementById('canvas');
  const ctx = canvas.getContext('2d');
  let width, height;
  const particles = [];

  function resize() {
    width = canvas.width = window.innerWidth;
    height = canvas.height = window.innerHeight;
  }

  window.addEventListener('resize', resize);
  resize();

  document.addEventListener('mousemove', (e) => {
    for (let i = 0; i < 5; i++) {
      particles.push({
        x: e.clientX,
        y: e.clientY,
        dx: (Math.random() - 0.5) * 2,
        dy: (Math.random() - 0.5) * 2,
        life: 100
      });
    }
  });

  function draw() {
    ctx.fillStyle = 'rgba(0,0,0,0.1)';
    ctx.fillRect(0, 0, width, height);

    for (let i = particles.length - 1; i >= 0; i--) {
      const p = particles[i];
      ctx.beginPath();
      ctx.arc(p.x, p.y, 2, 0, Math.PI * 2);
      ctx.fillStyle = '#38bdf8';
      ctx.fill();
      p.x += p.dx;
      p.y += p.dy;
      p.life -= 1;
      if (p.life <= 0) particles.splice(i, 1);
    }

    requestAnimationFrame(draw);
  }

  draw();
</script>
