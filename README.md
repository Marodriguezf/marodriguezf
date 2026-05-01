
<style>
@import url('https://fonts.googleapis.com/css2?family=Rajdhani:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500;700&family=Noto+Sans+SC:wght@300;400;700&display=swap');
*{box-sizing:border-box;margin:0;padding:0;}
.root{background:#07050f;font-family:'Rajdhani',sans-serif;padding:16px;position:relative;overflow:hidden;}
.root::before{content:'';position:absolute;top:-180px;left:-100px;width:520px;height:520px;background:radial-gradient(circle,rgba(139,92,246,0.18) 0%,transparent 65%);pointer-events:none;}
.root::after{content:'';position:absolute;bottom:-120px;right:-80px;width:420px;height:420px;background:radial-gradient(circle,rgba(192,38,211,0.13) 0%,transparent 65%);pointer-events:none;}
.blob2{position:absolute;top:40%;left:50%;transform:translateX(-50%);width:300px;height:300px;background:radial-gradient(circle,rgba(109,40,217,0.1) 0%,transparent 65%);pointer-events:none;}
.z{position:relative;z-index:2;}

/* GLASS BASE */
.glass{
  background:linear-gradient(135deg,rgba(255,255,255,0.07) 0%,rgba(255,255,255,0.02) 100%);
  backdrop-filter:blur(20px);
  -webkit-backdrop-filter:blur(20px);
  border:1px solid rgba(255,255,255,0.1);
  border-radius:16px;
  position:relative;
  overflow:hidden;
}
.glass::before{
  content:'';position:absolute;
  top:0;left:0;right:0;height:1px;
  background:linear-gradient(90deg,transparent,rgba(255,255,255,0.25),rgba(192,38,211,0.5),rgba(255,255,255,0.25),transparent);
}
.glass::after{
  content:'';position:absolute;
  bottom:0;left:0;right:0;height:1px;
  background:linear-gradient(90deg,transparent,rgba(139,92,246,0.15),transparent);
}
.glass-hero{
  background:linear-gradient(135deg,rgba(109,40,217,0.14) 0%,rgba(192,38,211,0.08) 50%,rgba(255,255,255,0.04) 100%);
  backdrop-filter:blur(24px);
  -webkit-backdrop-filter:blur(24px);
  border:1px solid rgba(255,255,255,0.12);
  border-radius:20px;position:relative;overflow:hidden;
}
.glass-hero::before{
  content:'';position:absolute;top:0;left:0;right:0;height:2px;
  background:linear-gradient(90deg,transparent,rgba(167,139,250,0.7),rgba(232,121,249,0.9),rgba(167,139,250,0.7),transparent);
}
.glass-hero::after{
  content:'';position:absolute;
  top:-60px;right:-60px;
  width:200px;height:200px;
  background:radial-gradient(circle,rgba(192,38,211,0.15) 0%,transparent 65%);
}
.glass-purple{
  background:linear-gradient(135deg,rgba(109,40,217,0.18) 0%,rgba(139,92,246,0.08) 100%);
  backdrop-filter:blur(20px);-webkit-backdrop-filter:blur(20px);
  border:1px solid rgba(167,139,250,0.2);
  border-radius:16px;position:relative;overflow:hidden;
}
.glass-purple::before{
  content:'';position:absolute;top:0;left:0;right:0;height:1px;
  background:linear-gradient(90deg,transparent,rgba(167,139,250,0.5),rgba(232,121,249,0.4),transparent);
}
.glass-pink{
  background:linear-gradient(135deg,rgba(192,38,211,0.14) 0%,rgba(255,255,255,0.03) 100%);
  backdrop-filter:blur(20px);-webkit-backdrop-filter:blur(20px);
  border:1px solid rgba(232,121,249,0.18);
  border-radius:16px;position:relative;overflow:hidden;
}
.glass-pink::before{
  content:'';position:absolute;top:0;left:0;right:0;height:1px;
  background:linear-gradient(90deg,transparent,rgba(232,121,249,0.6),transparent);
}
.glass-dark{
  background:linear-gradient(135deg,rgba(255,255,255,0.05) 0%,rgba(255,255,255,0.01) 100%);
  backdrop-filter:blur(16px);-webkit-backdrop-filter:blur(16px);
  border:1px solid rgba(255,255,255,0.08);
  border-radius:12px;position:relative;overflow:hidden;
}
.glass-dark::before{
  content:'';position:absolute;top:0;left:20%;right:20%;height:1px;
  background:linear-gradient(90deg,transparent,rgba(255,255,255,0.2),transparent);
}
.shine{
  position:absolute;top:0;left:-100%;width:60%;height:100%;
  background:linear-gradient(105deg,transparent 40%,rgba(255,255,255,0.04) 50%,transparent 60%);
  pointer-events:none;
}

/* NAV */
.nav{
  background:linear-gradient(90deg,rgba(109,40,217,0.15),rgba(192,38,211,0.1),rgba(109,40,217,0.15));
  backdrop-filter:blur(30px);-webkit-backdrop-filter:blur(30px);
  border:1px solid rgba(255,255,255,0.1);
  border-radius:50px;
  padding:8px 18px;margin-bottom:14px;
  display:flex;align-items:center;justify-content:space-between;
  box-shadow:0 4px 24px rgba(109,40,217,0.15);
  position:relative;overflow:hidden;
}
.nav::before{
  content:'';position:absolute;top:0;left:0;right:0;height:1px;
  background:linear-gradient(90deg,transparent,rgba(255,255,255,0.3),rgba(232,121,249,0.5),rgba(255,255,255,0.3),transparent);
}
.nav-logo{font-size:15px;font-weight:700;color:#c084fc;letter-spacing:.05em;}
.nav-links{display:flex;gap:14px;}
.nav-lnk{font-size:11px;color:rgba(196,132,252,0.45);letter-spacing:.05em;font-weight:600;}
.nav-lnk.on{color:#e879f9;}
.nbadge{background:rgba(167,139,250,0.15);border:1px solid rgba(167,139,250,0.3);border-radius:20px;padding:2px 9px;font-size:10px;color:#c084fc;font-weight:700;letter-spacing:.04em;}

/* HERO */
.hero-wrap{padding:18px;margin-bottom:12px;}
.hero-top{display:flex;gap:14px;align-items:flex-start;margin-bottom:14px;}
.av{width:70px;height:70px;border-radius:50%;flex-shrink:0;
  background:linear-gradient(135deg,rgba(109,40,217,0.5),rgba(192,38,211,0.4));
  backdrop-filter:blur(10px);
  border:2px solid rgba(255,255,255,0.15);
  display:flex;align-items:center;justify-content:center;position:relative;
  box-shadow:0 0 20px rgba(139,92,246,0.3),inset 0 1px 0 rgba(255,255,255,0.15);}
.av::after{content:'';position:absolute;inset:-5px;border-radius:50%;border:1px solid rgba(192,38,211,0.25);}
.av-i{font-size:22px;font-weight:700;color:#f0e6ff;font-family:'Rajdhani',sans-serif;}
.hi-name{font-size:22px;font-weight:700;color:#f5f0ff;letter-spacing:.02em;line-height:1.1;margin-bottom:2px;}
.hi-role{font-size:10px;color:rgba(167,139,250,0.65);letter-spacing:.18em;font-family:'JetBrains Mono',monospace;margin-bottom:10px;}
.hstats{display:flex;gap:14px;}
.hst{text-align:center;}
.hst-v{font-size:16px;font-weight:700;color:#e879f9;line-height:1;}
.hst-l{font-size:8px;color:rgba(167,139,250,0.45);letter-spacing:.1em;margin-top:1px;}
.sdiv{width:1px;background:rgba(167,139,250,0.2);align-self:stretch;}
.tags{display:flex;flex-wrap:wrap;gap:5px;margin-bottom:12px;}
.tag{font-size:9px;font-weight:600;padding:3px 9px;border-radius:20px;letter-spacing:.05em;font-family:'JetBrains Mono',monospace;}
.tp{background:rgba(109,40,217,0.2);border:1px solid rgba(167,139,250,0.3);color:#c084fc;backdrop-filter:blur(8px);}
.tc{background:rgba(192,38,211,0.15);border:1px solid rgba(232,121,249,0.28);color:#e879f9;backdrop-filter:blur(8px);}
.ti{background:rgba(79,70,229,0.16);border:1px solid rgba(129,140,248,0.28);color:#a5b4fc;backdrop-filter:blur(8px);}
.about{font-size:12px;color:rgba(209,196,255,0.65);line-height:1.75;font-weight:500;margin-bottom:12px;}
.about .hl{color:#e879f9;}.about .hl2{color:#c084fc;}
.xp-meta{display:flex;justify-content:space-between;margin-bottom:5px;}
.xp-lbl{font-size:10px;color:rgba(167,139,250,0.55);letter-spacing:.1em;font-weight:700;}
.xp-v{font-size:10px;color:#c084fc;font-family:'JetBrains Mono',monospace;}
.xp-track{height:5px;background:rgba(255,255,255,0.05);border-radius:10px;overflow:hidden;border:1px solid rgba(255,255,255,0.06);}
.xp-fill{height:100%;border-radius:10px;background:linear-gradient(90deg,#6d28d9,#a855f7,#e879f9);}

/* GRIDS */
.g2{display:grid;grid-template-columns:1fr 1fr;gap:10px;margin-bottom:10px;}
.g3{display:grid;grid-template-columns:1fr 1fr 1fr;gap:8px;margin-bottom:10px;}

/* SECTION HEAD */
.sh{font-size:10px;font-weight:700;color:rgba(192,38,211,0.65);letter-spacing:.2em;margin-bottom:10px;display:flex;align-items:center;gap:8px;font-family:'JetBrains Mono',monospace;}
.sh::after{content:'';flex:1;height:1px;background:linear-gradient(90deg,rgba(167,139,250,0.25),transparent);}

/* SKILL ROWS */
.sk-row{display:flex;align-items:center;gap:8px;padding:6px 0;border-bottom:1px solid rgba(255,255,255,0.04);}
.sk-row:last-child{border-bottom:none;}
.sk-ic{width:26px;height:26px;border-radius:8px;
  background:linear-gradient(135deg,rgba(109,40,217,0.3),rgba(192,38,211,0.2));
  border:1px solid rgba(255,255,255,0.1);
  backdrop-filter:blur(8px);
  display:flex;align-items:center;justify-content:center;font-size:12px;flex-shrink:0;
  box-shadow:inset 0 1px 0 rgba(255,255,255,0.1);}
.sk-nm{font-size:11px;font-weight:600;color:#d8c4f8;flex:1;letter-spacing:.02em;}
.sk-bw{width:72px;}
.sk-b{height:3px;background:rgba(255,255,255,0.04);border-radius:10px;overflow:hidden;}
.sf-p{background:linear-gradient(90deg,#6d28d9,#a855f7);}
.sf-c{background:linear-gradient(90deg,#c026d3,#e879f9);}
.sf-i{background:linear-gradient(90deg,#4f46e5,#818cf8);}
.sk-pct{font-size:9px;color:rgba(167,139,250,0.45);font-family:'JetBrains Mono',monospace;min-width:26px;text-align:right;}

/* MINI STATS */
.mst{padding:12px 8px;text-align:center;position:relative;}
.mst-n{font-size:18px;font-weight:700;line-height:1;margin-bottom:3px;}
.mst-l{font-size:8px;letter-spacing:.12em;color:rgba(167,139,250,0.45);font-weight:700;}
.colp{color:#c084fc;}.colc{color:#e879f9;}.coli{color:#a5b4fc;}

/* LANG BARS */
.lb{margin-bottom:9px;}
.lb:last-child{margin-bottom:0;}
.lb-m{display:flex;justify-content:space-between;margin-bottom:4px;}
.lb-n{font-size:11px;font-weight:600;color:#d8c4f8;}
.lb-p{font-size:9px;color:rgba(167,139,250,0.45);font-family:'JetBrains Mono',monospace;}
.lb-t{height:3px;background:rgba(255,255,255,0.04);border-radius:10px;overflow:hidden;}
.lf-p{background:linear-gradient(90deg,#6d28d9,#c084fc);}
.lf-c{background:linear-gradient(90deg,#c026d3,#e879f9);}
.lf-i{background:linear-gradient(90deg,#4f46e5,#818cf8);}

/* HUMAN LANGS */
.hl-row{display:flex;align-items:center;gap:8px;padding:6px 0;border-bottom:1px solid rgba(255,255,255,0.04);}
.hl-row:last-child{border-bottom:none;}
.hlfg{font-size:14px;width:20px;text-align:center;flex-shrink:0;}
.hlnm{font-size:11px;font-weight:600;color:#d8c4f8;flex:1;}
.hllv{font-size:8px;font-weight:700;padding:2px 6px;border-radius:10px;letter-spacing:.06em;
  background:rgba(109,40,217,0.2);border:1px solid rgba(167,139,250,0.25);color:#c084fc;
  backdrop-filter:blur(6px);font-family:'JetBrains Mono',monospace;}
.hldots{display:flex;gap:3px;}
.hd{width:6px;height:6px;border-radius:50%;background:rgba(167,139,250,0.1);border:1px solid rgba(167,139,250,0.18);}
.hd.on{background:#a855f7;border-color:#a855f7;}
.hd.oc{background:#e879f9;border-color:#e879f9;}

/* PROJECTS */
.pj{padding:14px;position:relative;overflow:hidden;}
.pj-before{position:absolute;top:0;left:0;right:0;height:2px;background:linear-gradient(90deg,#6d28d9,#e879f9);}
.pj-id{font-size:8px;font-weight:700;color:rgba(192,38,211,0.45);letter-spacing:.2em;margin-bottom:5px;font-family:'JetBrains Mono',monospace;}
.pj-nm{font-size:12px;font-weight:700;color:#f0e6ff;margin-bottom:4px;letter-spacing:.02em;}
.pj-dc{font-size:10px;color:rgba(196,132,252,0.45);line-height:1.55;margin-bottom:7px;}
.ptags{display:flex;gap:4px;flex-wrap:wrap;}
.pt{font-size:8px;font-weight:600;padding:2px 6px;border-radius:6px;
  background:rgba(192,38,211,0.12);border:1px solid rgba(232,121,249,0.2);color:#e879f9;
  backdrop-filter:blur(6px);letter-spacing:.04em;font-family:'JetBrains Mono',monospace;}

/* CONTACT */
.ctg{display:grid;grid-template-columns:1fr 1fr 1fr;gap:8px;margin-bottom:8px;}
.ctb{padding:12px 8px;text-align:center;cursor:pointer;}
.ct-ic{font-size:17px;margin-bottom:4px;}
.ct-ll{font-size:8px;color:rgba(167,139,250,0.4);letter-spacing:.12em;font-weight:700;}
.ct-l2{font-size:10px;color:#c084fc;font-weight:700;margin-top:1px;}

/* FOOTER */
.footer{text-align:center;padding:14px 0 2px;border-top:1px solid rgba(167,139,250,0.1);margin-top:4px;}
.fk{font-family:'Noto Sans SC',sans-serif;font-size:10px;color:rgba(167,139,250,0.25);letter-spacing:.3em;margin-bottom:5px;}
.ft{font-size:8px;color:rgba(167,139,250,0.25);letter-spacing:.18em;font-weight:700;font-family:'JetBrains Mono',monospace;}
</style>

<div class="root">
<div class="blob2"></div>
<div class="z">

<!-- NAV -->
<div class="nav">
  <span class="nav-logo">STACKLAYER_</span>
  <div class="nav-links">
    <span class="nav-lnk on">Profile</span>
    <span class="nav-lnk">Projects</span>
    <span class="nav-lnk">Stack</span>
  </div>
  <div style="display:flex;gap:6px;">
    <span class="nbadge">LVL 5+ DEV</span>
    <span class="nbadge">PM PRO</span>
  </div>
</div>

<!-- HERO CARD -->
<div class="glass-hero hero-wrap" style="margin-bottom:12px;">
  <div class="shine"></div>
  <div class="hero-top">
    <div class="av"><span class="av-i">AJ</span></div>
    <div style="flex:1;">
      <div class="hi-name">Alejandra</div>
      <div class="hi-role">SOFTWARE ENGINEER · PROJECT MANAGER</div>
      <div class="hstats">
        <div class="hst"><div class="hst-v">5+</div><div class="hst-l">YRS DEV</div></div>
        <div class="sdiv"></div>
        <div class="hst"><div class="hst-v" style="color:#c084fc;">PM</div><div class="hst-l">PMBOK</div></div>
        <div class="sdiv"></div>
        <div class="hst"><div class="hst-v" style="color:#a5b4fc;">AI</div><div class="hst-l">NATIVE</div></div>
      </div>
    </div>
  </div>
  <div class="tags">
    <span class="tag tp">PMBOK</span><span class="tag tc">React</span>
    <span class="tag tc">WordPress</span><span class="tag tp">Magnolia CMS</span>
    <span class="tag ti">Adobe Suite</span><span class="tag ti">Figma</span>
    <span class="tag tp">UX/UI</span><span class="tag tc">AI Workflow</span>
  </div>
  <div class="about">
    Building products <span class="hl">end-to-end</span> — from stakeholder plan to deployed interface.
    PM by discipline, developer by trade, designer at heart.
    Currently at <span class="hl2">Politécnico Grancolombiano</span> — shipping real PM deliverables like actual projects.
  </div>
  <div class="xp-meta">
    <span class="xp-lbl">CAREER XP</span>
    <span class="xp-v">75 / 100 pts</span>
  </div>
  <div class="xp-track"><div class="xp-fill" style="width:75%;"></div></div>
</div>

<!-- SKILL TRACKER + CODE STATS -->
<div class="g2">
  <!-- SKILL TRACKER -->
  <div class="glass-purple" style="padding:14px;">
    <div class="shine"></div>
    <div class="sh">SKILL TRACKER</div>
    <div class="sk-row">
      <div class="sk-ic">⚙️</div>
      <span class="sk-nm">JavaScript / React</span>
      <div class="sk-bw"><div class="sk-b"><div class="sf-c" style="width:82%;height:100%;border-radius:10px;"></div></div></div>
      <span class="sk-pct">82</span>
    </div>
    <div class="sk-row">
      <div class="sk-ic">🎯</div>
      <span class="sk-nm">Project Mgmt</span>
      <div class="sk-bw"><div class="sk-b"><div class="sf-p" style="width:90%;height:100%;border-radius:10px;"></div></div></div>
      <span class="sk-pct">90</span>
    </div>
    <div class="sk-row">
      <div class="sk-ic">🎨</div>
      <span class="sk-nm">Adobe / Figma</span>
      <div class="sk-bw"><div class="sk-b"><div class="sf-i" style="width:78%;height:100%;border-radius:10px;"></div></div></div>
      <span class="sk-pct">78</span>
    </div>
    <div class="sk-row">
      <div class="sk-ic">🤖</div>
      <span class="sk-nm">AI &amp; Automation</span>
      <div class="sk-bw"><div class="sk-b"><div class="sf-c" style="width:86%;height:100%;border-radius:10px;"></div></div></div>
      <span class="sk-pct">86</span>
    </div>
    <div class="sk-row">
      <div class="sk-ic">🗄️</div>
      <span class="sk-nm">WP / Magnolia</span>
      <div class="sk-bw"><div class="sk-b"><div class="sf-p" style="width:88%;height:100%;border-radius:10px;"></div></div></div>
      <span class="sk-pct">88</span>
    </div>
  </div>

  <!-- CODE STATS + MINI STATS -->
  <div style="display:flex;flex-direction:column;gap:8px;">
    <div class="glass-pink" style="padding:14px;flex:1;">
      <div class="shine"></div>
      <div class="sh">CODE STATS</div>
      <div class="lb">
        <div class="lb-m"><span class="lb-n">HTML / CSS</span><span class="lb-p">88%</span></div>
        <div class="lb-t"><div class="lf-c" style="width:88%;height:100%;border-radius:10px;"></div></div>
      </div>
      <div class="lb">
        <div class="lb-m"><span class="lb-n">JavaScript</span><span class="lb-p">82%</span></div>
        <div class="lb-t"><div class="lf-p" style="width:82%;height:100%;border-radius:10px;"></div></div>
      </div>
      <div class="lb">
        <div class="lb-m"><span class="lb-n">PHP</span><span class="lb-p">65%</span></div>
        <div class="lb-t"><div class="lf-i" style="width:65%;height:100%;border-radius:10px;"></div></div>
      </div>
    </div>
    <div class="g3" style="margin-bottom:0;">
      <div class="glass-dark mst"><div class="mst-n colc">5+</div><div class="mst-l">YEARS</div></div>
      <div class="glass-purple mst"><div class="mst-n colp">PM</div><div class="mst-l">EXPERT</div></div>
      <div class="glass-dark mst"><div class="mst-n coli">AI</div><div class="mst-l">NATIVE</div></div>
    </div>
  </div>
</div>

<!-- FEATURED PROJECTS -->
<div class="glass" style="padding:14px;margin-bottom:10px;">
  <div class="shine"></div>
  <div class="sh">FEATURED PROJECTS</div>
  <div class="g2" style="margin-bottom:0;">
    <div class="glass-purple pj">
      <div class="pj-before"></div>
      <div class="pj-id">PROJ_01</div>
      <div class="pj-nm">Proyecto Destacado</div>
      <div class="pj-dc">Descripción breve — qué construiste y qué problema resuelve.</div>
      <div class="ptags"><span class="pt">React</span><span class="pt">WordPress</span><span class="pt">JS</span></div>
    </div>
    <div class="glass-pink pj">
      <div class="pj-before"></div>
      <div class="pj-id">PROJ_02</div>
      <div class="pj-nm">Proyecto Destacado</div>
      <div class="pj-dc">Descripción breve — qué construiste y qué problema resuelve.</div>
      <div class="ptags"><span class="pt">PMBOK</span><span class="pt">PHP</span><span class="pt">UX/UI</span></div>
    </div>
    <div class="glass-dark pj">
      <div class="pj-before"></div>
      <div class="pj-id">PROJ_03</div>
      <div class="pj-nm">Proyecto Destacado</div>
      <div class="pj-dc">Descripción breve — qué construiste y qué problema resuelve.</div>
      <div class="ptags"><span class="pt">Figma</span><span class="pt">Adobe XD</span></div>
    </div>
    <div class="glass-purple pj">
      <div class="pj-before"></div>
      <div class="pj-id">PROJ_04</div>
      <div class="pj-nm">Proyecto Destacado</div>
      <div class="pj-dc">Descripción breve — qué construiste y qué problema resuelve.</div>
      <div class="ptags"><span class="pt">Magnolia</span><span class="pt">PM</span></div>
    </div>
  </div>
</div>

<!-- LANGUAGE SYSTEM -->
<div class="glass-purple" style="padding:14px;margin-bottom:10px;">
  <div class="shine"></div>
  <div class="sh">LANGUAGE SYSTEM</div>
  <div class="hl-row">
    <span class="hlfg">🇪🇸</span><span class="hlnm">Español</span>
    <span class="hllv">NATIVE</span>
    <div class="hldots"><div class="hd oc"></div><div class="hd oc"></div><div class="hd oc"></div><div class="hd oc"></div><div class="hd oc"></div></div>
  </div>
  <div class="hl-row">
    <span class="hlfg">🇺🇸</span><span class="hlnm">English</span>
    <span class="hllv">B2+ → C1</span>
    <div class="hldots"><div class="hd on"></div><div class="hd on"></div><div class="hd on"></div><div class="hd on"></div><div class="hd"></div></div>
  </div>
  <div class="hl-row">
    <span class="hlfg">🇨🇳</span>
    <span class="hlnm" style="font-family:'Noto Sans SC',sans-serif;">普通话 Mandarin</span>
    <span class="hllv">HSK 1→3</span>
    <div class="hldots"><div class="hd on"></div><div class="hd"></div><div class="hd"></div><div class="hd"></div><div class="hd"></div></div>
  </div>
  <div class="hl-row">
    <span class="hlfg">🇵🇹</span><span class="hlnm">Português</span>
    <span class="hllv">NEXT UP</span>
    <div class="hldots"><div class="hd"></div><div class="hd"></div><div class="hd"></div><div class="hd"></div><div class="hd"></div></div>
  </div>
</div>

<!-- CONTACT -->
<div class="glass-pink" style="padding:14px;margin-bottom:12px;">
  <div class="shine"></div>
  <div class="sh">CONTACT PORTAL</div>
  <div class="ctg">
    <div class="glass-dark ctb">
      <div class="ct-ic">💼</div>
      <div class="ct-ll">CONNECT</div>
      <div class="ct-l2">LinkedIn</div>
    </div>
    <div class="glass-dark ctb">
      <div class="ct-ic">✉️</div>
      <div class="ct-ll">MESSAGE</div>
      <div class="ct-l2">Email</div>
    </div>
    <div class="glass-dark ctb">
      <div class="ct-ic">📲</div>
      <div class="ct-ll">FOLLOW</div>
      <div class="ct-l2">@stacklayer_</div>
    </div>
  </div>
  <div style="text-align:center;margin-top:6px;">
    <span style="font-size:9px;color:rgba(167,139,250,0.3);letter-spacing:.15em;font-family:'JetBrains Mono',monospace;font-weight:700;">
      OPEN TO: FREELANCE · COLLAB · PM CONSULTING
    </span>
  </div>
</div>

<!-- FOOTER -->
<div class="footer">
  <div class="fk">工程师 · 项目经理 · 设计师</div>
  <div class="ft">BOGOTÁ, COLOMBIA · STACKLAYER_ · 2025</div>
</div>

</div>
</div>
