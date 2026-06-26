[w2_monday_exercise.html](https://github.com/user-attachments/files/29399341/w2_monday_exercise.html)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Week 2 · Monday — Past Simple | English Pocket Planner</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700&display=swap');
  *,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
  :root{
    --cream:#F5F0E8;--paper:#EDE8DF;--rule:#D4CCC0;
    --black:#1A1814;--charcoal:#2D2926;
    --terra:#C2714F;--terra-light:#D4896A;
    --warm:#8B7355;--muted:#6B6357;--white:#FDFAF5;
    --success:#5B9E6B;--error:#C2504F;
  }
  body{font-family:'Inter','Helvetica Neue',sans-serif;background:var(--cream);color:var(--black);min-height:100vh}

  .prog-wrap{position:fixed;top:0;left:0;right:0;height:3px;background:var(--rule);z-index:200}
  .prog-fill{height:100%;background:var(--terra);transition:width .4s ease;width:0%}

  header{background:var(--white);border-bottom:1px solid var(--rule);padding:0 28px;display:flex;align-items:stretch;justify-content:space-between;min-height:52px;position:sticky;top:3px;z-index:100}
  .wordmark{display:flex;align-items:center;font-family:'Arial Black','Helvetica Neue',Helvetica,sans-serif;font-weight:900;font-size:14px;letter-spacing:2px;text-transform:uppercase;border-right:1px solid var(--rule);padding-right:20px;margin-right:20px}
  .wordmark span{color:var(--terra)}
  .hd-meta{display:flex;align-items:center;font-size:10px;letter-spacing:3px;text-transform:uppercase;color:#B5A48A}
  .badge{font-size:10px;letter-spacing:2px;text-transform:uppercase;color:var(--terra);font-weight:700;border:1px solid var(--terra);padding:4px 10px;display:flex;align-items:center}

  .hero{background:var(--black);padding:40px 32px 36px;position:relative;overflow:hidden}
  .hero::before{content:'';position:absolute;top:-50px;right:-50px;width:220px;height:220px;border-radius:50%;border:1px solid rgba(194,113,79,.1)}
  .eyebrow{font-size:10px;letter-spacing:4px;text-transform:uppercase;color:var(--terra);font-weight:700;margin-bottom:14px;display:flex;align-items:center;gap:12px}
  .eyebrow::after{content:'';width:40px;height:1px;background:var(--terra);opacity:.4}
  .hero h1{font-family:'Arial Black','Helvetica Neue',Helvetica,sans-serif;font-weight:900;font-size:36px;letter-spacing:-1.5px;color:var(--white);line-height:1.05;margin-bottom:4px}
  .hero h1 em{font-family:'Georgia',serif;font-weight:400;font-style:italic;color:var(--terra);font-size:34px}
  .hero-goal{font-size:13px;color:#B5A48A;margin-top:14px;line-height:1.6;max-width:500px}
  .hero-goal strong{color:var(--white)}
  .hero-tags{display:flex;gap:8px;margin-top:18px;flex-wrap:wrap}
  .htag{font-size:9px;letter-spacing:2px;text-transform:uppercase;font-weight:700;padding:4px 10px;border:1px solid rgba(255,255,255,.12);color:rgba(255,255,255,.4)}
  .htag.on{border-color:var(--terra);color:var(--terra)}

  .wrap{max-width:700px;margin:0 auto;padding:40px 24px 80px}

  .sec-label{font-size:10px;letter-spacing:4px;text-transform:uppercase;color:var(--terra);font-weight:700;margin-bottom:20px;display:flex;align-items:center;gap:12px}
  .sec-label::after{content:'';flex:1;height:1px;background:var(--rule)}

  .ref-box{background:var(--white);border:1px solid var(--rule);border-left:3px solid var(--terra);padding:22px 26px;margin-bottom:40px}
  .ref-box h3{font-family:'Arial Black',Helvetica,sans-serif;font-size:11px;letter-spacing:1px;text-transform:uppercase;color:var(--black);margin-bottom:14px}
  .ref-grid{display:grid;grid-template-columns:1fr 1fr;gap:0}
  .ref-col{padding:0 16px 0 0}
  .ref-col:last-child{padding:0 0 0 16px;border-left:1px solid var(--rule)}
  .ref-title{font-size:10px;letter-spacing:2px;text-transform:uppercase;color:var(--terra);font-weight:700;margin-bottom:10px}
  .ref-rule{font-size:13px;color:var(--charcoal);line-height:1.7;margin-bottom:6px;display:flex;gap:8px}
  .ref-rule::before{content:'◆';color:var(--terra);font-size:8px;margin-top:4px;flex-shrink:0}
  .ref-ex{background:var(--cream);border:1px solid var(--rule);padding:10px 14px;margin-top:12px;font-size:12px;color:var(--muted);line-height:1.8}
  .ref-ex strong{color:var(--terra)}

  /* EXERCISE CARD */
  .ex-card{background:var(--white);border:1px solid var(--rule);margin-bottom:14px;overflow:hidden}
  .ex-head{background:var(--paper);border-bottom:1px solid var(--rule);padding:11px 20px;display:flex;align-items:center;gap:12px}
  .ex-num{font-family:'Arial Black',Helvetica,sans-serif;font-size:11px;font-weight:900;color:var(--terra);letter-spacing:1px;min-width:24px}
  .ex-tag{font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--muted);border:1px solid var(--rule);padding:2px 8px;font-weight:600}
  .ex-tag.affirm{border-color:#5B9E6B;color:#5B9E6B}
  .ex-tag.neg{border-color:var(--error);color:var(--error)}
  .ex-tag.quest{border-color:#5B8DB8;color:#5B8DB8}
  .ex-tag.irreg{border-color:var(--terra);color:var(--terra)}
  .ex-tag.reorder{border-color:#7B68B5;color:#7B68B5}
  .ex-inst{font-size:12px;color:var(--muted);margin-left:auto;font-style:italic}
  .ex-body{padding:22px}

  /* FILL IN THE BLANK */
  .fitb-sent{font-size:15px;color:var(--black);line-height:2.2;margin-bottom:4px}
  .fitb-hint{font-size:11px;color:var(--muted);margin-bottom:14px;letter-spacing:.2px}
  .fitb-in{border:none;border-bottom:2px solid var(--terra);background:transparent;font-size:15px;font-family:'Inter',sans-serif;color:var(--black);padding:0 6px;width:140px;outline:none;text-align:center;transition:border-color .2s}
  .fitb-in.ok{border-color:var(--success);color:var(--success)}
  .fitb-in.no{border-color:var(--error);color:var(--error)}
  .fitb-in:disabled{opacity:.7;cursor:default}

  .btn-check{background:var(--black);color:var(--cream);border:none;padding:11px 26px;font-size:11px;font-weight:700;letter-spacing:2px;text-transform:uppercase;cursor:pointer;margin-top:14px}
  .btn-check:hover{background:var(--charcoal)}
  .btn-check:disabled{opacity:.4;cursor:default}
  .feedback{display:none;margin-top:12px;padding:10px 14px;font-size:13px;line-height:1.6;border-left:3px solid transparent}
  .feedback.ok{background:#F0F8F2;color:var(--success);border-color:var(--success);display:block}
  .feedback.no{background:#FBF0F0;color:var(--error);border-color:var(--error);display:block}

  /* REORDER */
  .reorder-q{font-size:14px;color:var(--muted);margin-bottom:16px;line-height:1.6;font-style:italic}
  .words-pool{display:flex;flex-wrap:wrap;gap:8px;margin-bottom:16px;min-height:44px;padding:10px;border:1px dashed var(--rule);background:var(--cream)}
  .answer-zone{display:flex;flex-wrap:wrap;gap:8px;margin-bottom:16px;min-height:52px;padding:10px;border:1px solid var(--rule);background:var(--white);position:relative}
  .answer-zone::before{content:'Your answer';position:absolute;top:6px;right:10px;font-size:9px;letter-spacing:2px;text-transform:uppercase;color:var(--rule);font-weight:600}
  .word-chip{padding:8px 14px;font-size:13px;font-weight:600;cursor:pointer;border:1px solid var(--rule);background:var(--white);color:var(--charcoal);transition:all .15s;user-select:none}
  .word-chip:hover{border-color:var(--terra);color:var(--terra)}
  .word-chip.placed{background:var(--black);color:var(--cream);border-color:var(--black)}
  .word-chip.placed:hover{background:var(--charcoal);border-color:var(--charcoal)}
  .word-chip.correct-chip{background:#5B9E6B;color:var(--white);border-color:#5B9E6B;pointer-events:none}
  .word-chip.wrong-chip{background:var(--error);color:var(--white);border-color:var(--error)}
  .reorder-hint{font-size:11px;color:var(--muted);margin-bottom:4px}

  /* MC */
  .mc-q{font-size:15px;font-weight:600;color:var(--black);margin-bottom:16px;line-height:1.5}
  .mc-opts{display:flex;flex-direction:column;gap:8px}
  .mc-opt{display:flex;align-items:center;gap:12px;padding:12px 16px;border:1px solid var(--rule);background:var(--white);cursor:pointer;font-size:14px;color:var(--charcoal);text-align:left;width:100%;transition:all .15s}
  .mc-opt:hover{border-color:var(--terra)}
  .mc-opt.correct{border-color:var(--success);background:#F0F8F2;color:var(--success);pointer-events:none}
  .mc-opt.wrong{border-color:var(--error);background:#FBF0F0;color:var(--error);pointer-events:none}
  .mc-opt.disabled{pointer-events:none;opacity:.55}
  .opt-lt{font-family:'Arial Black',Helvetica,sans-serif;font-size:10px;font-weight:900;letter-spacing:1px;color:var(--terra);min-width:16px}
  .mc-opt.correct .opt-lt{color:var(--success)}
  .mc-opt.wrong .opt-lt{color:var(--error)}

  hr.div{border:none;border-top:1px solid var(--rule);margin:40px 0}

  /* SCORE */
  .score-card{display:none;background:var(--white);border:1px solid var(--rule);padding:36px;text-align:center;margin-top:8px}
  .score-card.show{display:block}
  .score-num{font-family:'Arial Black',Helvetica,sans-serif;font-size:64px;font-weight:900;color:var(--terra);line-height:1;display:block;margin-bottom:6px}
  .score-lbl{font-size:10px;letter-spacing:3px;text-transform:uppercase;color:var(--muted);display:block;margin-bottom:20px}
  .score-msg{font-family:'Georgia',serif;font-style:italic;font-size:17px;color:var(--charcoal);line-height:1.6;max-width:380px;margin:0 auto}

  /* SPEAKING */
  .speaking-card{background:var(--black);padding:36px;margin-top:40px;position:relative;overflow:hidden}
  .speaking-card::before{content:'◉';position:absolute;top:20px;right:24px;font-size:56px;color:rgba(194,113,79,.1);line-height:1}
  .sp-label{font-size:9px;letter-spacing:4px;text-transform:uppercase;color:var(--terra);font-weight:700;margin-bottom:16px}
  .sp-prompt{font-family:'Georgia',serif;font-style:italic;font-size:20px;color:var(--white);line-height:1.5;margin-bottom:20px}
  .sp-tips{display:flex;flex-direction:column;gap:10px}
  .sp-tip{display:flex;gap:10px;font-size:13px;color:#B5A48A;line-height:1.5}
  .sp-tip::before{content:'→';color:var(--terra);flex-shrink:0}

  .btn-result{background:var(--black);color:var(--cream);border:none;padding:13px 32px;font-size:11px;font-weight:700;letter-spacing:2px;text-transform:uppercase;cursor:pointer}
  .btn-reset{background:transparent;color:var(--muted);border:1px solid var(--rule);padding:12px 22px;font-size:10px;font-weight:700;letter-spacing:2px;text-transform:uppercase;cursor:pointer;margin-left:10px}

  @media(max-width:600px){
    .hero{padding:28px 20px}
    .hero h1{font-size:26px}
    .hero h1 em{font-size:24px}
    .wrap{padding:28px 16px 60px}
    header{padding:0 16px}
    .ref-grid{grid-template-columns:1fr}
    .ref-col:last-child{padding:16px 0 0;border-left:none;border-top:1px solid var(--rule);margin-top:12px}
    .score-num{font-size:48px}
  }
</style>
</head>
<body>

<div class="prog-wrap"><div class="prog-fill" id="prog"></div></div>

<header>
  <div style="display:flex;align-items:center">
    <div class="wordmark">Renata<span>em</span>Inglês</div>
    <span class="hd-meta">English Pocket Planner</span>
  </div>
  <div style="display:flex;align-items:center">
    <span class="badge">Week 2 · Monday</span>
  </div>
</header>

<div class="hero">
  <div class="eyebrow">Week 2 · Monday</div>
  <h1>Past Simple<br><em>Practice</em></h1>
  <p class="hero-goal"><strong>Goal:</strong> Use Past Simple correctly in affirmative, negative and question forms — and nail those irregular verbs.</p>
  <div class="hero-tags">
    <span class="htag on">Affirmative</span>
    <span class="htag on">Negative</span>
    <span class="htag on">Questions</span>
    <span class="htag on">Irregular Verbs</span>
    <span class="htag on">Reorder</span>
  </div>
</div>

<div class="wrap">

  <!-- QUICK REFERENCE -->
  <div class="sec-label">Quick Reference</div>
  <div class="ref-box">
    <h3>◆ Past Simple — The 4 forms</h3>
    <div class="ref-grid">
      <div class="ref-col">
        <div class="ref-title">Affirmative & Negative</div>
        <div class="ref-rule">Regular: verb + <strong style="color:var(--terra)">-ed</strong> → She <strong style="color:var(--terra)">worked</strong> late.</div>
        <div class="ref-rule">Irregular: must memorize → I <strong style="color:var(--terra)">went</strong>, she <strong style="color:var(--terra)">saw</strong>, we <strong style="color:var(--terra)">had</strong>.</div>
        <div class="ref-rule">Negative: <strong style="color:var(--terra)">didn't</strong> + base verb → He <strong style="color:var(--terra)">didn't call</strong>.</div>
        <div class="ref-ex">
          <strong>I watched</strong> that show last night.<br>
          <strong>She didn't go</strong> to the party.<br>
          <strong>We met</strong> at a coffee shop in 2021.
        </div>
      </div>
      <div class="ref-col">
        <div class="ref-title">Questions</div>
        <div class="ref-rule"><strong style="color:var(--terra)">Did</strong> + subject + base verb?</div>
        <div class="ref-rule">Wh- questions: <strong style="color:var(--terra)">What/Where/When + did</strong> + subject + base verb?</div>
        <div class="ref-rule">⚠️ Never: <em style="color:var(--error)">Did she went?</em> → Always base verb after did.</div>
        <div class="ref-ex">
          <strong>Did you see</strong> that movie?<br>
          <strong>Where did they go</strong> last summer?<br>
          <strong>What did she say</strong> to you?
        </div>
      </div>
    </div>
  </div>

  <!-- EXERCISES -->
  <div class="sec-label">Exercises</div>

  <!-- EX 1 — FITB Affirmative Regular -->
  <div class="ex-card">
    <div class="ex-head">
      <span class="ex-num">01</span>
      <span class="ex-tag affirm">Affirmative · Regular</span>
      <span class="ex-inst">Fill in the blank with the correct Past Simple form.</span>
    </div>
    <div class="ex-body">
      <p class="fitb-sent">Last night, she <input class="fitb-in" id="f1a" placeholder="watch"/> a documentary about climate change for 2 hours.</p>
      <p class="fitb-hint">💡 watch → regular verb, add -ed</p>
      <p class="fitb-sent">The band <input class="fitb-in" id="f1b" placeholder="play"/> three sold-out shows in Brazil last year.</p>
      <p class="fitb-hint">💡 play → regular verb, add -ed</p>
      <p class="fitb-sent">I <input class="fitb-in" id="f1c" placeholder="finish"/> the entire series in one weekend. No regrets.</p>
      <p class="fitb-hint">💡 finish → regular verb, add -ed</p>
      <button class="btn-check" onclick="checkFITB('g1', {f1a:['watched'], f1b:['played'], f1c:['finished']}, 'fb1')">Check →</button>
      <div class="feedback" id="fb1"></div>
    </div>
  </div>

  <!-- EX 2 — FITB Irregular -->
  <div class="ex-card">
    <div class="ex-head">
      <span class="ex-num">02</span>
      <span class="ex-tag irreg">Irregular Verbs</span>
      <span class="ex-inst">Fill in the blank with the correct irregular Past Simple form.</span>
    </div>
    <div class="ex-body">
      <p class="fitb-sent">She <input class="fitb-in" id="f2a" placeholder="go"/> to New York for the first time and absolutely loved it.</p>
      <p class="fitb-hint">💡 go → went</p>
      <p class="fitb-sent">I <input class="fitb-in" id="f2b" placeholder="see"/> that movie everyone was talking about. It was incredible.</p>
      <p class="fitb-hint">💡 see → saw</p>
      <p class="fitb-sent">We <input class="fitb-in" id="f2c" placeholder="have"/> the most amazing dinner at that new Italian place downtown.</p>
      <p class="fitb-hint">💡 have → had</p>
      <p class="fitb-sent">He <input class="fitb-in" id="f2d" placeholder="tell"/> me the whole story and I couldn't believe it.</p>
      <p class="fitb-hint">💡 tell → told</p>
      <button class="btn-check" onclick="checkFITB('g2', {f2a:['went'], f2b:['saw'], f2c:['had'], f2d:['told']}, 'fb2')">Check →</button>
      <div class="feedback" id="fb2"></div>
    </div>
  </div>

  <!-- EX 3 — FITB Negative -->
  <div class="ex-card">
    <div class="ex-head">
      <span class="ex-num">03</span>
      <span class="ex-tag neg">Negative</span>
      <span class="ex-inst">Rewrite using didn't + base verb.</span>
    </div>
    <div class="ex-body">
      <p class="fitb-sent">She called me. → She <input class="fitb-in" id="f3a" placeholder="didn't..."/> me.</p>
      <p class="fitb-hint">💡 didn't + base verb (call)</p>
      <p class="fitb-sent">They enjoyed the concert. → They <input class="fitb-in" id="f3b" placeholder="didn't..."/> the concert.</p>
      <p class="fitb-hint">💡 didn't + base verb (enjoy)</p>
      <p class="fitb-sent">He knew the answer. → He <input class="fitb-in" id="f3c" placeholder="didn't..."/> the answer.</p>
      <p class="fitb-hint">💡 didn't + base verb (know) — never "didn't knew"!</p>
      <button class="btn-check" onclick="checkFITB('g3', {f3a:["didn't call","did not call"], f3b:["didn't enjoy","did not enjoy"], f3c:["didn't know","did not know"]}, 'fb3')">Check →</button>
      <div class="feedback" id="fb3"></div>
    </div>
  </div>

  <!-- EX 4 — FITB Questions -->
  <div class="ex-card">
    <div class="ex-head">
      <span class="ex-num">04</span>
      <span class="ex-tag quest">Questions</span>
      <span class="ex-inst">Complete the questions with the correct form.</span>
    </div>
    <div class="ex-body">
      <p class="fitb-sent"><input class="fitb-in" id="f4a" placeholder="did/was"/> you watch the game last night?</p>
      <p class="fitb-hint">💡 Yes/No question with Past Simple = Did + subject + base verb</p>
      <p class="fitb-sent">Where <input class="fitb-in" id="f4b" placeholder="did they go"/> they go for their honeymoon?</p>
      <p class="fitb-hint">💡 Wh- question: Where + did + subject + base verb</p>
      <p class="fitb-sent">What <input class="fitb-in" id="f4c" placeholder="did she say"/> she say when you told her the news?</p>
      <p class="fitb-hint">💡 Wh- question: What + did + subject + base verb</p>
      <button class="btn-check" onclick="checkFITB('g4', {f4a:['did'], f4b:['did'], f4c:['did']}, 'fb4')">Check →</button>
      <div class="feedback" id="fb4"></div>
    </div>
  </div>

  <!-- EX 5 — REORDER Affirmative -->
  <div class="ex-card">
    <div class="ex-head">
      <span class="ex-num">05</span>
      <span class="ex-tag reorder">Reorder</span>
      <span class="ex-inst">Tap the words in the correct order to form a sentence.</span>
    </div>
    <div class="ex-body">
      <p class="reorder-hint">Affirmative — tap words in order, tap again to remove:</p>
      <div class="words-pool" id="pool5"></div>
      <div class="answer-zone" id="zone5"></div>
      <button class="btn-check" onclick="checkReorder('r5', 'she went to the concert alone and loved every second', 'fb5')">Check →</button>
      <div class="feedback" id="fb5"></div>
    </div>
  </div>

  <!-- EX 6 — REORDER Negative -->
  <div class="ex-card">
    <div class="ex-head">
      <span class="ex-num">06</span>
      <span class="ex-tag reorder">Reorder</span>
      <span class="ex-inst">Tap the words in the correct order.</span>
    </div>
    <div class="ex-body">
      <p class="reorder-hint">Negative — remember: didn't + BASE verb:</p>
      <div class="words-pool" id="pool6"></div>
      <div class="answer-zone" id="zone6"></div>
      <button class="btn-check" onclick="checkReorder('r6', 'he didn\'t know about the surprise party', 'fb6')">Check →</button>
      <div class="feedback" id="fb6"></div>
    </div>
  </div>

  <!-- EX 7 — REORDER Question -->
  <div class="ex-card">
    <div class="ex-head">
      <span class="ex-num">07</span>
      <span class="ex-tag reorder">Reorder</span>
      <span class="ex-inst">Tap the words in the correct order.</span>
    </div>
    <div class="ex-body">
      <p class="reorder-hint">Question — remember: Did + subject + BASE verb + ?</p>
      <div class="words-pool" id="pool7"></div>
      <div class="answer-zone" id="zone7"></div>
      <button class="btn-check" onclick="checkReorder('r7', 'what did you do after the show ended', 'fb7')">Check →</button>
      <div class="feedback" id="fb7"></div>
    </div>
  </div>

  <!-- EX 8 — REORDER Irregular -->
  <div class="ex-card">
    <div class="ex-head">
      <span class="ex-num">08</span>
      <span class="ex-tag reorder">Reorder</span>
      <span class="ex-inst">Tap the words in the correct order.</span>
    </div>
    <div class="ex-body">
      <p class="reorder-hint">Irregular verbs — put the story in order:</p>
      <div class="words-pool" id="pool8"></div>
      <div class="answer-zone" id="zone8"></div>
      <button class="btn-check" onclick="checkReorder('r8', 'they met fell in love and got married in the same year', 'fb8')">Check →</button>
      <div class="feedback" id="fb8"></div>
    </div>
  </div>

  <hr class="div">

  <div style="text-align:center">
    <button class="btn-result" onclick="showScore()">Ver meu resultado →</button>
    <button class="btn-reset" onclick="resetAll()">↺ Recomeçar</button>
  </div>

  <div class="score-card" id="scoreCard">
    <span class="score-num" id="scoreNum">—</span>
    <span class="score-lbl" id="scoreLbl">exercícios corretos</span>
    <p class="score-msg" id="scoreMsg"></p>
  </div>

  <!-- SPEAKING SPRINT -->
  <div class="speaking-card">
    <p class="sp-label">Speaking Sprint · 2 min</p>
    <p class="sp-prompt">"Tell me about a time something unexpected happened to you. Where were you? What did you do?"</p>
    <div class="sp-tips">
      <div class="sp-tip">Grave 1–2 minutos respondendo o prompt — sem parar para traduzir.</div>
      <div class="sp-tip">Use pelo menos 3 irregular verbs: went, saw, told, met, had, felt, knew…</div>
      <div class="sp-tip">Organize com connectors: first… then… after that… suddenly… in the end…</div>
    </div>
  </div>

</div>

<script>
// ── State ──
const st = {
  g1: false, g2: false, g3: false, g4: false,
  r5: false, r6: false, r7: false, r8: false
};

// ── REORDER setup ──
const REORDER_DATA = {
  r5: { pool: 'pool5', zone: 'zone5', sentence: 'she went to the concert alone and loved every second' },
  r6: { pool: 'pool6', zone: 'zone6', sentence: "he didn't know about the surprise party" },
  r7: { pool: 'pool7', zone: 'zone7', sentence: 'what did you do after the show ended' },
  r8: { pool: 'pool8', zone: 'zone8', sentence: 'they met fell in love and got married in the same year' },
};

function shuffle(arr){ return arr.sort(()=>Math.random()-.5) }

function initReorder(id){
  const d = REORDER_DATA[id];
  const words = shuffle(d.sentence.split(' ').map(w=>w));
  const pool = document.getElementById(d.pool);
  pool.innerHTML = '';
  document.getElementById(d.zone).innerHTML = '';
  words.forEach(w => {
    const chip = document.createElement('div');
    chip.className = 'word-chip';
    chip.textContent = w;
    chip.onclick = () => moveToZone(chip, d.zone, d.pool);
    pool.appendChild(chip);
  });
}

function moveToZone(chip, zoneId, poolId){
  const zone = document.getElementById(zoneId);
  chip.classList.add('placed');
  chip.onclick = () => moveToPool(chip, poolId, zoneId);
  zone.appendChild(chip);
  updateProg();
}

function moveToPool(chip, poolId, zoneId){
  const pool = document.getElementById(poolId);
  chip.classList.remove('placed');
  chip.onclick = () => moveToZone(chip, zoneId, poolId);
  pool.appendChild(chip);
}

function checkReorder(id, correct, fbId){
  const d = REORDER_DATA[id];
  const zone = document.getElementById(d.zone);
  const chips = zone.querySelectorAll('.word-chip');
  const answer = Array.from(chips).map(c=>c.textContent).join(' ').toLowerCase();
  const fb = document.getElementById(fbId);

  chips.forEach(c => c.classList.remove('correct-chip','wrong-chip','placed'));

  if(answer === correct.toLowerCase()){
    chips.forEach(c => c.classList.add('correct-chip'));
    fb.className = 'feedback ok';
    fb.textContent = '✓ Perfect! The sentence is correct.';
    st[id] = true;
  } else {
    chips.forEach(c => c.classList.add('wrong-chip'));
    fb.className = 'feedback no';
    fb.textContent = `✗ Not quite. Correct order: "${correct.charAt(0).toUpperCase()+correct.slice(1)}." Tap words to rearrange and try again.`;
    setTimeout(()=>{
      chips.forEach(c=>{c.classList.remove('wrong-chip','correct-chip');c.classList.add('placed');});
    },1800);
  }
  updateProg();
}

// ── FILL IN THE BLANK ──
function checkFITB(groupId, answers, fbId){
  let allCorrect = true, anyFilled = false;

  Object.keys(answers).forEach(id => {
    const inp = document.getElementById(id);
    if(!inp) return;
    const val = inp.value.trim().toLowerCase();
    if(!val) return;
    anyFilled = true;
    const correct = answers[id].map(a=>a.toLowerCase());
    if(correct.includes(val)){
      inp.classList.remove('no'); inp.classList.add('ok');
    } else {
      inp.classList.remove('ok'); inp.classList.add('no');
      allCorrect = false;
    }
    inp.disabled = allCorrect;
  });

  const fb = document.getElementById(fbId);
  if(!anyFilled){
    fb.className='feedback no'; fb.textContent='✗ Fill in at least one blank before checking.'; return;
  }
  if(allCorrect){
    fb.className='feedback ok'; fb.textContent='✓ All correct! Great work.';
    st[groupId] = true;
    document.querySelectorAll(`[id^="${groupId.replace('g','')}"]`).forEach(i=>i.disabled=true);
  } else {
    fb.className='feedback no'; fb.textContent='✗ Some answers need a fix — check the highlighted blanks and try again.';
  }
  updateProg();
}

// ── PROGRESS ──
function updateProg(){
  const done = Object.values(st).filter(Boolean).length;
  document.getElementById('prog').style.width = (done/8*100)+'%';
}

// ── SCORE ──
function showScore(){
  const done = Object.values(st).filter(Boolean).length;
  document.getElementById('scoreNum').textContent = done;
  document.getElementById('scoreLbl').textContent = `de 8 exercícios corretos`;
  const msgs = [
    "Keep going! Review the Quick Reference and try the exercises again.",
    "You're getting there! Focus on the negative and question forms.",
    "Good progress! Review the ones you missed — you're almost there.",
    "Getting stronger! A few more to nail.",
    "Almost perfect! One more push.",
    "Really solid work! Review any mistakes and do the Speaking Sprint.",
    "Excellent! You've got Past Simple down. Time to speak! 🎉",
    "Outstanding! You dominated this exercise. Go crush that Speaking Sprint! 🔥",
    "Perfect score! 🏆 Past Simple is yours — now tell your story out loud."
  ];
  document.getElementById('scoreMsg').textContent = msgs[Math.min(done,8)];
  const card = document.getElementById('scoreCard');
  card.classList.add('show');
  card.scrollIntoView({behavior:'smooth',block:'center'});
}

// ── RESET ──
function resetAll(){
  Object.keys(st).forEach(k => st[k]=false);
  document.querySelectorAll('.fitb-in').forEach(i=>{i.value='';i.classList.remove('ok','no');i.disabled=false;});
  document.querySelectorAll('.feedback').forEach(f=>f.className='feedback');
  document.getElementById('scoreCard').classList.remove('show');
  document.getElementById('prog').style.width='0%';
  ['r5','r6','r7','r8'].forEach(id=>initReorder(id));
  window.scrollTo({top:0,behavior:'smooth'});
}

// ── INIT ──
['r5','r6','r7','r8'].forEach(id=>initReorder(id));
</script>
</body>
</html>
