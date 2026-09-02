<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1">
<title>STRAC 経営分析ツール</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Zen+Kaku+Gothic+New:wght@500;700;900&family=Noto+Sans+JP:wght@400;500;700&family=JetBrains+Mono:wght@400;500;700&display=swap" rel="stylesheet">
<style>
  :root{
    --paper:#EDF1E7;
    --paper-alt:#E2E9DA;
    --paper-deep:#D7E0CC;
    --rule:#B5C2A9;
    --ink:#1F2E23;
    --ink-soft:#526354;
    --forest:#1F2E23;
    --forest-2:#14201A;
    --brass:#9C7331;
    --brass-soft:#C99A4B;
    --red-ink:#8B3A2B;
    --focus:#5B7A5E;
  }
  *{box-sizing:border-box;}
  html,body{margin:0;padding:0;}
  body{
    background:var(--paper);
    color:var(--ink);
    font-family:'Noto Sans JP',sans-serif;
    -webkit-font-smoothing:antialiased;
  }
  .mono{font-family:'JetBrains Mono',monospace;}
  h1,h2,h3,.disp{font-family:'Zen Kaku Gothic New',sans-serif;}

  /* ---------- topbar ---------- */
  .topbar{
    background:var(--forest);
    color:var(--paper);
    padding:14px 20px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    flex-wrap:wrap;
    gap:10px;
    border-bottom:3px solid var(--brass);
  }
  .brand{display:flex;align-items:baseline;gap:10px;}
  .brand .mark{
    font-family:'Zen Kaku Gothic New',sans-serif;
    font-weight:900;
    font-size:1.4rem;
    letter-spacing:.04em;
  }
  .brand .sub{
    font-size:.72rem;
    color:var(--brass-soft);
    letter-spacing:.12em;
  }
  .formula-strip{
    font-family:'JetBrains Mono',monospace;
    font-size:.85rem;
    color:var(--paper);
    background:rgba(255,255,255,.06);
    border:1px solid rgba(255,255,255,.18);
    padding:6px 14px;
    border-radius:2px;
    letter-spacing:.03em;
  }
  .formula-strip b{color:var(--brass-soft);}
  .formula-strip .live{color:#E8C589;font-weight:700;}

  /* ---------- layout ---------- */
  .layout{display:flex;min-height:calc(100vh - 62px);}
  .sidebar{
    width:250px;
    flex-shrink:0;
    background:var(--paper-alt);
    border-right:1px solid var(--rule);
    padding:18px 0;
  }
  .side-group{margin-bottom:6px;}
  .side-group-title{
    font-size:.68rem;
    letter-spacing:.14em;
    color:var(--ink-soft);
    padding:10px 20px 6px;
    text-transform:uppercase;
  }
  .side-btn{
    display:block;
    width:100%;
    text-align:left;
    background:none;
    border:none;
    border-left:3px solid transparent;
    padding:9px 20px;
    font-family:'Noto Sans JP',sans-serif;
    font-size:.92rem;
    color:var(--ink);
    cursor:pointer;
  }
  .side-btn .kana{
    display:block;
    font-family:'JetBrains Mono',monospace;
    font-size:.68rem;
    color:var(--ink-soft);
    margin-top:1px;
  }
  .side-btn:hover{background:var(--paper-deep);}
  .side-btn.active{
    background:var(--paper-deep);
    border-left-color:var(--brass);
    font-weight:700;
    color:var(--red-ink);
  }
  .content{flex:1;padding:28px 32px 60px;max-width:820px;}

  .panel{display:none;}
  .panel.active{display:block;}
  .panel h2{margin:0 0 4px;font-size:1.5rem;}
  .panel .desc{color:var(--ink-soft);font-size:.9rem;margin-bottom:22px;line-height:1.6;}
  .note{
    font-size:.8rem;
    color:var(--ink-soft);
    background:var(--paper-alt);
    border-left:3px solid var(--brass);
    padding:8px 12px;
    margin:10px 0 20px;
    line-height:1.6;
  }
  .baseline-box{
    font-family:'JetBrains Mono',monospace;
    font-size:.8rem;
    background:var(--paper-alt);
    border:1px dashed var(--rule);
    padding:10px 14px;
    margin-bottom:20px;
    color:var(--ink-soft);
  }
  .baseline-box.empty{color:var(--red-ink);}
  .link-btn{
    background:none;
    border:none;
    padding:0;
    margin:0;
    font:inherit;
    font-family:'JetBrains Mono',monospace;
    color:var(--red-ink);
    text-decoration:underline;
    cursor:pointer;
  }
  .link-btn:hover{color:var(--brass);}

  fieldset{border:none;padding:0;margin:0 0 18px;}
  legend{
    font-weight:700;
    font-size:.85rem;
    color:var(--forest);
    padding:0 0 8px;
    border-bottom:1px solid var(--rule);
    width:100%;
    margin-bottom:6px;
  }
  .field-row{
    display:flex;
    align-items:baseline;
    justify-content:space-between;
    gap:10px;
    padding:8px 0;
    border-bottom:1px dashed var(--rule);
  }
  .field-row label{font-size:.88rem;}
  .field-row .field-desc{color:var(--ink-soft);font-size:.76rem;display:block;}
  .field-row input[type=number], .field-row input[type=text]{
    width:130px;
    text-align:right;
    font-family:'JetBrains Mono',monospace;
    font-size:.95rem;
    border:none;
    border-bottom:1px solid var(--ink-soft);
    background:transparent;
    padding:4px 2px;
    color:var(--ink);
  }
  .field-row input:focus{outline:none;border-bottom:2px solid var(--focus);}
  .field-row input::placeholder{color:#9AA79B;font-size:.72rem;}
  select{
    font-family:'Noto Sans JP',sans-serif;
    padding:6px 8px;
    border:1px solid var(--ink-soft);
    background:var(--paper);
    color:var(--ink);
  }
  .radio-row{display:flex;gap:18px;padding:8px 0;}
  .radio-row label{display:flex;align-items:center;gap:6px;font-size:.88rem;}

  .btn{
    background:var(--forest);
    color:var(--paper);
    border:none;
    padding:11px 26px;
    font-family:'Zen Kaku Gothic New',sans-serif;
    font-weight:700;
    font-size:.9rem;
    letter-spacing:.04em;
    cursor:pointer;
    border-radius:2px;
    margin-top:6px;
  }
  .btn:hover{background:var(--brass);}
  .btn.secondary{
    background:transparent;
    color:var(--forest);
    border:1px solid var(--forest);
  }
  .btn.secondary:hover{background:var(--paper-deep);}

  .tape{
    font-family:'JetBrains Mono',monospace;
    background:var(--paper-alt);
    border:1px solid var(--rule);
    padding:18px 20px;
    margin-top:22px;
    font-size:.9rem;
  }
  .tape .t-title{
    font-weight:700;
    color:var(--forest);
    margin-bottom:8px;
    letter-spacing:.05em;
  }
  .tape .t-row{display:flex;justify-content:space-between;padding:3px 0;}
  .tape .t-row .lbl{color:var(--ink-soft);}
  .tape .t-row .val{font-weight:700;}
  .tape .t-row.highlight .val{color:var(--red-ink);}
  .tape .t-rule{border-top:1px dashed var(--rule);margin:8px 0;}
  .tape .t-note{color:var(--brass);font-size:.8rem;padding:2px 0;}
  table.grid{
    width:100%;
    border-collapse:collapse;
    font-family:'JetBrains Mono',monospace;
    font-size:.82rem;
    margin-top:10px;
  }
  table.grid th, table.grid td{
    border-bottom:1px solid var(--rule);
    padding:6px 8px;
    text-align:right;
  }
  table.grid th{color:var(--ink-soft);font-weight:700;background:var(--paper-alt);}
  .scroll-x{overflow-x:auto;}
  .hidden{display:none;}
  .btn-row{display:flex;gap:10px;flex-wrap:wrap;}

  @media (max-width:820px){
    .layout{flex-direction:column;}
    .sidebar{
      width:100%;
      display:flex;
      overflow-x:auto;
      padding:8px 4px;
      border-right:none;
      border-bottom:1px solid var(--rule);
    }
    .side-group{display:flex;align-items:center;flex-shrink:0;}
    .side-group-title{padding:0 8px;white-space:nowrap;}
    .side-btn{white-space:nowrap;border-left:none;border-bottom:3px solid transparent;padding:8px 12px;}
    .side-btn.active{border-bottom-color:var(--brass);}
    .side-btn .kana{display:none;}
    .content{padding:20px 16px 50px;}
    .field-row input[type=number]{width:100px;}
  }
</style>
</head>
<body>

<div class="topbar">
  <div class="brand">
    <span class="mark">STRAC</span>
    <span class="sub">戦略会計 意思決定支援ツール</span>
  </div>
  <div class="formula-strip">P − V = M ・ M × Q = <span id="strip-mq" class="live">MQ</span></div>
</div>

<div class="layout">
  <nav class="sidebar" id="sidebar">
    <div class="side-group">
      <div class="side-group-title">基本</div>
      <button class="side-btn" data-mode="strac1">STRAC-1<span class="kana">単一商品の損益分解</span></button>
      <button class="side-btn" data-mode="strac2">STRAC-2<span class="kana">商品3種の損益分解</span></button>
    </div>
    <div class="side-group">
      <div class="side-group-title">比較</div>
      <button class="side-btn" data-mode="t">T-STRAC<span class="kana">目標との差異</span></button>
      <button class="side-btn" data-mode="h">H-STRAC<span class="kana">期間比較</span></button>
    </div>
    <div class="side-group">
      <div class="side-group-title">戦略</div>
      <button class="side-btn" data-mode="mq">MQ戦略<span class="kana">価格・数量シミュレーション</span></button>
    </div>
    <div class="side-group">
      <div class="side-group-title">特殊</div>
      <button class="side-btn" data-mode="f">F-STRAC<span class="kana">販促効果測定</span></button>
      <button class="side-btn" data-mode="cf">CF-STRAC<span class="kana">資金繰り</span></button>
    </div>
    <div class="side-group">
      <div class="side-group-title">経営計画</div>
      <button class="side-btn" data-mode="mgf">MGF<span class="kana">固定費積算</span></button>
      <button class="side-btn" data-mode="k">経営計画(K)<span class="kana">利益計画・必要枚数</span></button>
    </div>
  </nav>

  <main class="content">

    <!-- ============ STRAC-1 ============ -->
    <section class="panel" id="panel-strac1">
      <h2>STRAC-1</h2>
      <p class="desc">P（販売単価）・V（変動費単価）・Q（数量）・F（固定費）・G（目標利益）のうち、算出したい項目を<b>空欄のまま</b>にしてください。他の4項目から自動計算します。</p>
      <div class="note">この結果は「T-STRAC」「H-STRAC」の基準値として保存されます。</div>
      <form id="form-strac1">
        <div class="field-row"><label>P<span class="field-desc">販売単価</span></label><input type="number" step="any" id="s1-P" placeholder="空欄で計算"></div>
        <div class="field-row"><label>V<span class="field-desc">変動費単価</span></label><input type="number" step="any" id="s1-V" placeholder="空欄で計算"></div>
        <div class="field-row"><label>Q<span class="field-desc">数量</span></label><input type="number" step="any" id="s1-Q" placeholder="空欄で計算"></div>
        <div class="field-row"><label>F<span class="field-desc">固定費</span></label><input type="number" step="any" id="s1-F" placeholder="空欄で計算"></div>
        <div class="field-row"><label>G<span class="field-desc">目標利益</span></label><input type="number" step="any" id="s1-G" placeholder="空欄で計算"></div>
        <button type="submit" class="btn">計算する</button>
      </form>
      <div id="s1-result"></div>
    </section>

    <!-- ============ STRAC-2 ============ -->
    <section class="panel" id="panel-strac2">
      <h2>STRAC-2</h2>
      <p class="desc">3つの商品（4・5・6）を持つ場合の損益分解です。P4〜G のうち算出したい1項目だけを空欄にしてください。</p>
      <form id="form-strac2">
        <fieldset>
          <legend>商品4</legend>
          <div class="field-row"><label>P4</label><input type="number" step="any" id="s2-P4" placeholder="空欄で計算"></div>
          <div class="field-row"><label>V4</label><input type="number" step="any" id="s2-V4" placeholder="空欄で計算"></div>
          <div class="field-row"><label>Q4</label><input type="number" step="any" id="s2-Q4" placeholder="空欄で計算"></div>
        </fieldset>
        <fieldset>
          <legend>商品5</legend>
          <div class="field-row"><label>P5</label><input type="number" step="any" id="s2-P5" placeholder="空欄で計算"></div>
          <div class="field-row"><label>V5</label><input type="number" step="any" id="s2-V5" placeholder="空欄で計算"></div>
          <div class="field-row"><label>Q5</label><input type="number" step="any" id="s2-Q5" placeholder="空欄で計算"></div>
        </fieldset>
        <fieldset>
          <legend>商品6</legend>
          <div class="field-row"><label>P6</label><input type="number" step="any" id="s2-P6" placeholder="空欄で計算"></div>
          <div class="field-row"><label>V6</label><input type="number" step="any" id="s2-V6" placeholder="空欄で計算"></div>
          <div class="field-row"><label>Q6</label><input type="number" step="any" id="s2-Q6" placeholder="空欄で計算"></div>
        </fieldset>
        <fieldset>
          <legend>全体</legend>
          <div class="field-row"><label>F<span class="field-desc">固定費</span></label><input type="number" step="any" id="s2-F" placeholder="空欄で計算"></div>
          <div class="field-row"><label>G<span class="field-desc">目標利益</span></label><input type="number" step="any" id="s2-G" placeholder="空欄で計算"></div>
        </fieldset>
        <button type="submit" class="btn">計算する</button>
      </form>
      <div id="s2-result"></div>
    </section>

    <!-- ============ T-STRAC ============ -->
    <section class="panel" id="panel-t">
      <h2>T-STRAC（目標比較）</h2>
      <p class="desc">STRAC-1 の基準値に対して、目標値を入力すると差異を計算します。変更しなかった項目は自動的に釣り合う値を逆算します。</p>
      <div id="t-baseline" class="baseline-box empty">先に <button type="button" class="link-btn" onclick="switchMode('strac1')">STRAC-1</button> を計算して基準値を作成してください。</div>
      <form id="form-t" class="hidden">
        <div class="field-row"><label>PT<span class="field-desc">目標 販売単価</span></label><input type="number" step="any" id="t-PT"></div>
        <div class="field-row"><label>VT<span class="field-desc">目標 変動費単価</span></label><input type="number" step="any" id="t-VT"></div>
        <div class="field-row"><label>QT<span class="field-desc">目標 数量</span></label><input type="number" step="any" id="t-QT"></div>
        <div class="field-row"><label>FT<span class="field-desc">目標 固定費</span></label><input type="number" step="any" id="t-FT"></div>
        <div class="field-row"><label>GT<span class="field-desc">目標 利益</span></label><input type="number" step="any" id="t-GT"></div>
        <button type="submit" class="btn">差異を計算する</button>
      </form>
      <div id="t-result"></div>
    </section>

    <!-- ============ H-STRAC ============ -->
    <section class="panel" id="panel-h">
      <h2>H-STRAC（期間比較）</h2>
      <p class="desc">STRAC-1 の基準値を「前期」として保持したまま、「今期」の実績を入力すると増減（貢献差異）を計算します。</p>
      <div id="h-baseline" class="baseline-box empty">先に <button type="button" class="link-btn" onclick="switchMode('strac1')">STRAC-1</button> を計算して基準値（前期）を作成してください。</div>
      <form id="form-h" class="hidden">
        <p class="desc" style="margin-top:0;">今期の実績（1項目のみ空欄で計算可）</p>
        <div class="field-row"><label>P<span class="field-desc">今期 販売単価</span></label><input type="number" step="any" id="h-P" placeholder="空欄で計算"></div>
        <div class="field-row"><label>V<span class="field-desc">今期 変動費単価</span></label><input type="number" step="any" id="h-V" placeholder="空欄で計算"></div>
        <div class="field-row"><label>Q<span class="field-desc">今期 数量</span></label><input type="number" step="any" id="h-Q" placeholder="空欄で計算"></div>
        <div class="field-row"><label>F<span class="field-desc">今期 固定費</span></label><input type="number" step="any" id="h-F" placeholder="空欄で計算"></div>
        <div class="field-row"><label>G<span class="field-desc">今期 目標利益</span></label><input type="number" step="any" id="h-G" placeholder="空欄で計算"></div>
        <button type="submit" class="btn">増減を計算する</button>
      </form>
      <div id="h-result"></div>
    </section>

    <!-- ============ MQ戦略 ============ -->
    <section class="panel" id="panel-mq">
      <h2>MQ戦略シミュレーション</h2>
      <p class="desc">目標MQ（限界利益総額）を達成するために、価格（P）または数量（Q）をどう振れば良いかを一覧表で確認します。</p>
      <form id="form-mq">
        <div class="field-row"><label>MQ<span class="field-desc">目標限界利益総額</span></label><input type="number" step="any" id="mq-MQ"></div>
        <div class="field-row"><label>V<span class="field-desc">変動費単価（固定）</span></label><input type="number" step="any" id="mq-V"></div>
        <div class="radio-row">
          <label><input type="radio" name="mq-mode" value="PP" checked> P（価格）を振る</label>
          <label><input type="radio" name="mq-mode" value="QQ"> Q（数量）を振る</label>
        </div>
        <div id="mq-pp-fields">
          <div class="field-row"><label>P 開始</label><input type="number" step="any" id="mq-P1"></div>
          <div class="field-row"><label>P 終了</label><input type="number" step="any" id="mq-P2"></div>
        </div>
        <div id="mq-qq-fields" class="hidden">
          <div class="field-row"><label>Q 開始</label><input type="number" step="any" id="mq-Q1"></div>
          <div class="field-row"><label>Q 終了</label><input type="number" step="any" id="mq-Q2"></div>
        </div>
        <div class="field-row"><label>STEP<span class="field-desc">刻み幅</span></label><input type="number" step="any" id="mq-S" value="1"></div>
        <button type="submit" class="btn">一覧表を作成する</button>
      </form>
      <div id="mq-result"></div>
    </section>

    <!-- ============ F-STRAC ============ -->
    <section class="panel" id="panel-f">
      <h2>F-STRAC（販促効果測定）</h2>
      <p class="desc">P・V・Q・F・EH・FM・N・H のうち算出したい1項目を空欄にしてください。</p>
      <form id="form-f">
        <div class="field-row"><label>P<span class="field-desc">販売単価</span></label><input type="number" step="any" id="f-P" placeholder="空欄で計算"></div>
        <div class="field-row"><label>V<span class="field-desc">変動費単価</span></label><input type="number" step="any" id="f-V" placeholder="空欄で計算"></div>
        <div class="field-row"><label>Q<span class="field-desc">数量</span></label><input type="number" step="any" id="f-Q" placeholder="空欄で計算"></div>
        <div class="field-row"><label>F<span class="field-desc">固定費</span></label><input type="number" step="any" id="f-F" placeholder="空欄で計算"></div>
        <div class="field-row"><label>EH<span class="field-desc">見積工数</span></label><input type="number" step="any" id="f-EH" placeholder="空欄で計算"></div>
        <div class="field-row"><label>FM<span class="field-desc">F/M比率(%)</span></label><input type="number" step="any" id="f-FM" placeholder="空欄で計算"></div>
        <div class="field-row"><label>N<span class="field-desc">人数</span></label><input type="number" step="any" id="f-N" placeholder="空欄で計算"></div>
        <div class="field-row"><label>H<span class="field-desc">時間</span></label><input type="number" step="any" id="f-H" placeholder="空欄で計算"></div>
        <button type="submit" class="btn">計算する</button>
      </form>
      <div id="f-result"></div>
    </section>

    <!-- ============ CF-STRAC ============ -->
    <section class="panel" id="panel-cf">
      <h2>CF-STRAC（資金繰り）</h2>
      <p class="desc">14項目のうち算出したい1項目を空欄にしてください。</p>
      <div class="note">T・D・TG・TA は元のプログラムに項目名の意味を示す説明文がなく、意味が分からなかったため記号のまま残しています。正式名称が分かれば置き換えます。</div>
      <form id="form-cf">
        <div class="field-row"><label>PQ<span class="field-desc">売上</span></label><input type="number" step="any" id="cf-PQ" placeholder="空欄で計算"></div>
        <div class="field-row"><label>IN<span class="field-desc">当期IN</span></label><input type="number" step="any" id="cf-IN" placeholder="空欄で計算"></div>
        <div class="field-row"><label>CF<span class="field-desc">キャッシュF</span></label><input type="number" step="any" id="cf-CF" placeholder="空欄で計算"></div>
        <div class="field-row"><label>U1<span class="field-desc">前繰売掛</span></label><input type="number" step="any" id="cf-U1" placeholder="空欄で計算"></div>
        <div class="field-row"><label>U2<span class="field-desc">次繰売掛</span></label><input type="number" step="any" id="cf-U2" placeholder="空欄で計算"></div>
        <div class="field-row"><label>K1<span class="field-desc">前繰買掛</span></label><input type="number" step="any" id="cf-K1" placeholder="空欄で計算"></div>
        <div class="field-row"><label>K2<span class="field-desc">次繰買掛</span></label><input type="number" step="any" id="cf-K2" placeholder="空欄で計算"></div>
        <div class="field-row"><label>T</label><input type="number" step="any" id="cf-T" placeholder="空欄で計算"></div>
        <div class="field-row"><label>D</label><input type="number" step="any" id="cf-D" placeholder="空欄で計算"></div>
        <div class="field-row"><label>L<span class="field-desc">借入</span></label><input type="number" step="any" id="cf-L" placeholder="空欄で計算"></div>
        <div class="field-row"><label>TG</label><input type="number" step="any" id="cf-TG" placeholder="空欄で計算"></div>
        <div class="field-row"><label>TA</label><input type="number" step="any" id="cf-TA" placeholder="空欄で計算"></div>
        <div class="field-row"><label>C1<span class="field-desc">前繰現金</span></label><input type="number" step="any" id="cf-C1" placeholder="空欄で計算"></div>
        <div class="field-row"><label>C2<span class="field-desc">次繰現金</span></label><input type="number" step="any" id="cf-C2" placeholder="空欄で計算"></div>
        <button type="submit" class="btn">計算する</button>
      </form>
      <div id="cf-result"></div>
    </section>

    <!-- ============ MGF ============ -->
    <section class="panel" id="panel-mgf">
      <h2>MGF（固定費積算）</h2>
      <p class="desc">人員・設備などの内訳から固定費（F）を積み上げます。計算後、そのまま「経営計画」へ進めます。</p>
      <form id="form-mgf">
        <div class="field-row"><label>何期<span class="field-desc">KI</span></label><input type="number" step="any" id="mgf-KI" value="1"></div>
        <div class="field-row"><label>人数<span class="field-desc">N</span></label><input type="number" step="any" id="mgf-N" value="0"></div>
        <div class="field-row"><label>倍率<span class="field-desc">RITU</span></label><input type="number" step="any" id="mgf-RITU" value="1"></div>
        <div class="field-row"><label>機械台数<span class="field-desc">D</span></label><input type="number" step="any" id="mgf-D" value="0"></div>
        <div class="field-row"><label>金利<span class="field-desc">F3</span></label><input type="number" step="any" id="mgf-F3" value="0"></div>
        <div class="field-row"><label>倉庫台数<span class="field-desc">SO</span></label><input type="number" step="any" id="mgf-SO" value="0"></div>
        <div class="field-row"><label>チップ枚数<span class="field-desc">CH</span></label><input type="number" step="any" id="mgf-CH" value="0"></div>
        <div class="field-row"><label>特急枚数<span class="field-desc">EX</span></label><input type="number" step="any" id="mgf-EX" value="0"></div>
        <div class="field-row"><label>減価償却<span class="field-desc">F5</span></label><input type="number" step="any" id="mgf-F5" value="10"></div>
        <div class="field-row"><label>その他F<span class="field-desc">FEX</span></label><input type="number" step="any" id="mgf-FEX" value="0"></div>
        <button type="submit" class="btn">Fを積算する</button>
      </form>
      <div id="mgf-result"></div>
    </section>

    <!-- ============ K 経営計画 ============ -->
    <section class="panel" id="panel-k">
      <h2>経営計画（K）</h2>
      <p class="desc">固定費（F）と目標利益（G）から必要なMQ・数量・行数（必要枚数）を計画します。</p>
      <div id="k-from-mgf" class="baseline-box hidden"></div>
      <form id="form-k">
        <div class="field-row"><label>F<span class="field-desc">固定費</span></label><input type="number" step="any" id="k-F" value="0"></div>
        <div class="field-row"><label>G<span class="field-desc">目標利益</span></label><input type="number" step="any" id="k-G" value="0"></div>
        <div class="field-row"><label>V<span class="field-desc">変動費単価</span></label><input type="number" step="any" id="k-V" value="0"></div>
        <div class="field-row"><label>P<span class="field-desc">販売単価</span></label><input type="number" step="any" id="k-P" value="30"></div>
        <div class="field-row"><label>製造能力<span class="field-desc">SEI</span></label><input type="number" step="any" id="k-SEI" value="1"></div>
        <div class="field-row"><label>販売能力<span class="field-desc">HAN</span></label><input type="number" step="any" id="k-HAN" value="2"></div>
        <div class="field-row"><label>繰り枚数<span class="field-desc">JIK</span></label><input type="number" step="any" id="k-JIK" value="0"></div>
        <div class="field-row"><label>リスクカード<span class="field-desc">RI</span></label><input type="number" step="any" id="k-RI" value="0"></div>
        <button type="submit" class="btn">計画する</button>
      </form>
      <div id="k-result"></div>
    </section>

  </main>
</div>

<script>
/* ---------------- helpers ---------------- */
function num(id){
  const el = document.getElementById(id);
  const v = el.value.trim();
  return v === '' ? null : parseFloat(v);
}
function fmt(x){
  if(x===null || x===undefined || !isFinite(x)) return '—';
  const r = Math.round(x*100)/100;
  return r.toLocaleString('ja-JP',{maximumFractionDigits:2});
}
function roundB(x, d=0){ // mimic BASIC INT(x*10^d + .5)/10^d
  const f = Math.pow(10,d);
  return Math.floor(x*f + 0.5)/f;
}
function ceilB(x){ return Math.ceil(x - 1e-9); }

function row(label, value, opts={}){
  return `<div class="t-row ${opts.highlight?'highlight':''}"><span class="lbl">${label}</span><span class="val">${typeof value==='string'?value:fmt(value)}${opts.unit||''}</span></div>`;
}
function rule(){ return `<div class="t-rule"></div>`; }
function tape(title, html){
  return `<div class="tape"><div class="t-title">${title}</div>${html}</div>`;
}
function noteLine(text){ return `<div class="t-note">${text}</div>`; }

/* ---------------- baseline state (shared by T / H) ---------------- */
let baseline = null; // {P,V,Q,F,G,M,PQ,VQ,MQ}

/* ---------------- shared values carried between modes ---------------- */
// STRAC-1 / MGF / K が入力・計算した MQ・V・F・P を、MQ戦略・経営計画(K) で引き継ぐ
let shared = { MQ:null, V:null, F:null, P:null };

function syncSharedIntoForm(mode){
  if(mode === 'mq'){
    if(shared.MQ !== null) document.getElementById('mq-MQ').value = shared.MQ;
    if(shared.V  !== null) document.getElementById('mq-V').value = shared.V;
  }
  if(mode === 'k'){
    if(shared.F !== null) document.getElementById('k-F').value = shared.F;
    if(shared.V !== null) document.getElementById('k-V').value = shared.V;
    if(shared.P !== null) document.getElementById('k-P').value = shared.P;
  }
}

function setBaseline(b){
  baseline = b;
  const html = `基準値 &nbsp; P=${fmt(b.P)} &nbsp; V=${fmt(b.V)} &nbsp; Q=${fmt(b.Q)} &nbsp; M=${fmt(b.M)} &nbsp; F=${fmt(b.F)} &nbsp; G=${fmt(b.G)}`;
  ['t-baseline','h-baseline'].forEach(id=>{
    const el = document.getElementById(id);
    el.className = 'baseline-box';
    el.innerHTML = html;
  });
  document.getElementById('form-t').classList.remove('hidden');
  document.getElementById('form-h').classList.remove('hidden');
  if(baseline){
    document.getElementById('t-PT').value = b.P;
    document.getElementById('t-VT').value = b.V;
    document.getElementById('t-QT').value = b.Q;
    document.getElementById('t-FT').value = b.F;
    document.getElementById('t-GT').value = b.G;
  }
  document.getElementById('strip-mq').textContent = 'MQ = ' + fmt(b.MQ);
}

/* ---------------- STRAC-1 ---------------- */
function calcStrac1(P,V,Q,F,G){
  if(P===null) P = (V*Q+F+G)/Q;
  if(V===null) V = (P*Q-F-G)/Q;
  if(Q===null) Q = (F+G)/(P-V);
  if(F===null) F = P*Q - V*Q - G;
  if(G===null) G = P*Q - V*Q - F;
  const M = P-V, PQ = P*Q, VQ = V*Q, MQ = M*Q;
  return {P,V,Q,F,G,M,PQ,VQ,MQ};
}
document.getElementById('form-strac1').addEventListener('submit', e=>{
  e.preventDefault();
  const r = calcStrac1(num('s1-P'),num('s1-V'),num('s1-Q'),num('s1-F'),num('s1-G'));
  let html = '';
  html += row('P（販売単価）', r.P);
  html += row('V（変動費単価）', r.V);
  html += row('M（限界利益単価）', r.M);
  html += row('Q（数量）', r.Q);
  html += rule();
  html += row('PQ（売上高）', r.PQ);
  html += row('VQ（変動費総額）', r.VQ);
  html += row('MQ（限界利益総額）', r.MQ, {highlight:true});
  html += row('F（固定費）', r.F);
  html += row('G（利益）', r.G, {highlight:true});
  html += rule();
  html += row('V%（変動費率）', r.V/r.P*100, {unit:'%'});
  html += row('FM（損益分岐点比率）', r.F/r.MQ*100, {unit:'%'});
  html += row('Q0（損益分岐点数量）', r.F/r.M);
  document.getElementById('s1-result').innerHTML = tape('STRAC-1 結果', html);
  setBaseline(r);
  shared.MQ = r.MQ; shared.V = r.V; shared.F = r.F; shared.P = r.P;
});

/* ---------------- STRAC-2 ---------------- */
document.getElementById('form-strac2').addEventListener('submit', e=>{
  e.preventDefault();
  let P4=num('s2-P4'),P5=num('s2-P5'),P6=num('s2-P6'),
      V4=num('s2-V4'),V5=num('s2-V5'),V6=num('s2-V6'),
      Q4=num('s2-Q4'),Q5=num('s2-Q5'),Q6=num('s2-Q6'),
      F=num('s2-F'),G=num('s2-G');

  if(P4===null) P4 = ((V4*Q4+V5*Q5+V6*Q6+F+G)-P5*Q5-P6*Q6)/Q4;
  if(P5===null) P5 = ((V4*Q4+V5*Q5+V6*Q6+F+G)-P4*Q4-P6*Q6)/Q5;
  if(P6===null) P6 = ((V4*Q4+V5*Q5+V6*Q6+F+G)-P4*Q4-P5*Q5)/Q6;
  if(V4===null) V4 = (P4*Q4+P5*Q5+P6*Q6-V5*Q5-V6*Q6-F-G)/Q4;
  if(V5===null) V5 = (P4*Q4+P5*Q5+P6*Q6-V4*Q4-V6*Q6-F-G)/Q5;
  if(V6===null) V6 = (P4*Q4+P5*Q5+P6*Q6-V4*Q4-V5*Q5-F-G)/Q6;
  if(Q4===null) Q4 = (F+G-(P5-V5)*Q5-(P6-V6)*Q6)/(P4-V4);
  if(Q5===null) Q5 = (F+G-(P4-V4)*Q4-(P6-V6)*Q6)/(P5-V5);
  if(Q6===null) Q6 = (F+G-(P4-V4)*Q4-(P5-V5)*Q5)/(P6-V6);
  if(F===null) F = (P4*Q4+P5*Q5+P6*Q6)-(V4*Q4+V5*Q5+V6*Q6)-G;
  if(G===null) G = (P4*Q4+P5*Q5+P6*Q6)-(V4*Q4+V5*Q5+V6*Q6)-F;

  const M4=P4-V4, M5=P5-V5, M6=P6-V6;
  const SPQ=(P4*Q4)+(P5*Q5)+(P6*Q6);
  const SVQ=(V4*Q4)+(V5*Q5)+(V6*Q6);
  const SMQ=(M4*Q4)+(M5*Q5)+(M6*Q6);
  const A=roundB(M4*Q4/SMQ*100), B=roundB(M5*Q5/SMQ*100), C=100-(A+B);
  const D=100, E=roundB(F/SMQ*100), H=D-E;
  const I=100, J=roundB(SVQ/SPQ*100), K=100-J;

  let html = '';
  html += row('P4', P4)+row('V4', V4)+row('M4', M4)+rule();
  html += row('P5', P5)+row('V5', V5)+row('M5', M5)+rule();
  html += row('P6', P6)+row('V6', V6)+row('M6', M6)+rule();
  html += row('Q4', Q4)+row('Q5', Q5)+row('Q6', Q6)+rule();
  html += row('MQ4', M4*Q4, {unit:` (${A}%)`});
  html += row('MQ5', M5*Q5, {unit:` (${B}%)`});
  html += row('MQ6', M6*Q6, {unit:` (${C}%)`});
  html += rule();
  html += row('SMQ（限界利益合計）', SMQ, {unit:` (${D}%)`, highlight:true});
  html += row('F（固定費）', F, {unit:` (${E}%)`});
  html += row('G（利益）', G, {unit:` (${H}%)`, highlight:true});
  html += rule();
  html += row('SPQ（総売上高）', SPQ, {unit:` (${I}%)`});
  html += row('SVQ（総変動費）', SVQ, {unit:` (${J}%)`});
  html += row('SMQ（限界利益合計）', SMQ, {unit:` (${K}%)`});
  html += rule();
  html += row('V%', SVQ/SPQ*100, {unit:'%'});
  html += row('FM', F/SMQ*100, {unit:'%'});
  document.getElementById('s2-result').innerHTML = tape('STRAC-2 結果', html);
});

/* ---------------- T-STRAC ---------------- */
document.getElementById('form-t').addEventListener('submit', e=>{
  e.preventDefault();
  if(!baseline){ return; }
  const P=baseline.P, V=baseline.V, Q=baseline.Q, F=baseline.F, G=baseline.G;
  const P3=num('t-PT'), V3=num('t-VT'), Q3=num('t-QT'), F3=num('t-FT'), G3=num('t-GT');
  const eq = (a,b)=> Math.abs(a-b) < 1e-9;

  let PT = (V3*Q3+F3+G3)/Q3, flagP=false;
  if(!eq(P3,P)){ PT=P3; flagP=true; }
  let VT = (P3*Q3-F3-G3)/Q3, flagV=false;
  if(!eq(V3,V)){ VT=V3; flagV=true; }
  let QT = (F3+G3)/(P3-V3), flagQ=false;
  if(!eq(Q3,Q)){ QT=Q3; flagQ=true; }
  let FT = P3*Q3-V3*Q3-G3, flagF=false;
  if(!eq(F3,F)){ FT=F3; flagF=true; }
  let GT = P3*Q3-V3*Q3-F3, flagG=false;
  if(!eq(G3,G)){ GT=G3; flagG=true; }

  const DP=PT-P, DV=VT-V, DQ=QT-Q, DF=FT-F, DG=GT-G;

  let html = '';
  if(flagP) html += noteLine(`※ PT は入力値をそのまま採用: ${fmt(PT)}`);
  if(flagV) html += noteLine(`※ VT は入力値をそのまま採用: ${fmt(VT)}`);
  if(flagQ) html += noteLine(`※ QT は入力値をそのまま採用: ${fmt(QT)}`);
  if(flagF) html += noteLine(`※ FT は入力値をそのまま採用: ${fmt(FT)}`);
  if(flagG) html += noteLine(`※ GT は入力値をそのまま採用: ${fmt(GT)}`);
  html += row('PT', PT)+row('VT', VT)+row('QT', QT)+row('FT', FT)+row('GT', GT);
  html += rule();
  html += row('DP（価格差）', DP)+row('DV（変動費差）', DV)+row('DQ（数量差）', DQ)+row('DF（固定費差）', DF)+row('DG（利益差）', DG, {highlight:true});
  html += rule();
  html += row('DP%', DP/P*100, {unit:'%'});
  html += row('DV%', DV/V*100, {unit:'%'});
  html += row('DQ%', DQ/Q*100, {unit:'%'});
  html += row('DF%', DF/F*100, {unit:'%'});
  if(G!==0) html += row('DG%', DG/G*100, {unit:'%'});
  document.getElementById('t-result').innerHTML = tape('T-STRAC 結果', html);
});

/* ---------------- H-STRAC ---------------- */
document.getElementById('form-h').addEventListener('submit', e=>{
  e.preventDefault();
  if(!baseline){ return; }
  const b0 = baseline; // 前期
  const cur = calcStrac1(num('h-P'),num('h-V'),num('h-Q'),num('h-F'),num('h-G')); // 今期

  const PK=(cur.P-b0.P)*(cur.Q+b0.Q)/2;
  const VK=(cur.V-b0.V)*(cur.Q+b0.Q)/2;
  const MK=(cur.M-b0.M)*(cur.Q+b0.Q)/2;
  const QK=(cur.Q-b0.Q)*(cur.M+b0.M)/2;
  const AK=cur.PQ-b0.P*b0.Q;
  const BK=cur.VQ-b0.V*b0.Q;
  const CK=cur.MQ-b0.M*b0.Q;
  const FK=cur.F-b0.F;
  const GK=CK-FK;

  let html = '';
  html += `<div class="t-title" style="margin-top:0;">今期の実績</div>`;
  html += row('P', cur.P)+row('V', cur.V)+row('M', cur.M)+row('Q', cur.Q)+row('F', cur.F)+row('G', cur.G, {highlight:true});
  html += rule();
  html += `<div class="t-title">前期との増減（貢献差異）</div>`;
  html += row('PK（価格要因）', PK);
  html += row('VK（変動費要因）', VK*-1);
  html += row('MK（限界利益要因）', MK);
  html += row('QK（数量要因）', QK);
  html += rule();
  html += row('PQK（売上高増減）', AK);
  html += row('VQK（変動費増減）', BK*-1);
  html += row('MQK（限界利益増減）', CK, {highlight:true});
  html += row('FK（固定費増減）', FK*-1);
  html += row('GK（利益増減）', GK, {highlight:true});
  document.getElementById('h-result').innerHTML = tape('H-STRAC 結果', html);
  // 前期の基準値は維持する（元プログラムの挙動を再現）
});

/* ---------------- MQ戦略 ---------------- */
document.querySelectorAll('input[name="mq-mode"]').forEach(r=>{
  r.addEventListener('change', ()=>{
    const isPP = document.querySelector('input[name="mq-mode"]:checked').value === 'PP';
    document.getElementById('mq-pp-fields').classList.toggle('hidden', !isPP);
    document.getElementById('mq-qq-fields').classList.toggle('hidden', isPP);
  });
});
document.getElementById('form-mq').addEventListener('submit', e=>{
  e.preventDefault();
  const MQ = num('mq-MQ'), V = num('mq-V'), S = num('mq-S') || 1;
  const mode = document.querySelector('input[name="mq-mode"]:checked').value;
  const rows = [];
  if(mode === 'PP'){
    const P1=num('mq-P1'), P2=num('mq-P2');
    const n = Math.max(0, Math.floor((P2-P1)/S + 1e-9) + 1);
    for(let i=0;i<n;i++){
      const P = P1 + i*S;
      const M = P-V;
      const Q = roundB(MQ/M, 1);
      rows.push({P,V,M,Q,PQ:P*Q,VQ:V*Q,MQr:M*Q});
    }
  } else {
    const Q1=num('mq-Q1'), Q2=num('mq-Q2');
    const n = Math.max(0, Math.floor((Q2-Q1)/S + 1e-9) + 1);
    for(let i=0;i<n;i++){
      const Q = roundB(Q1 + i*S, 1);
      const M = roundB(MQ/Q, 1);
      const P = V+M;
      rows.push({P,V,M,Q,PQ:P*Q,VQ:V*Q,MQr:M*Q});
    }
  }
  let html = `<div class="scroll-x"><table class="grid"><thead><tr><th>P</th><th>V</th><th>M</th><th>Q</th><th>PQ</th><th>VQ</th><th>MQ</th></tr></thead><tbody>`;
  rows.forEach(r=>{
    html += `<tr><td>${fmt(r.P)}</td><td>${fmt(r.V)}</td><td>${fmt(r.M)}</td><td>${fmt(r.Q)}</td><td>${fmt(r.PQ)}</td><td>${fmt(r.VQ)}</td><td>${fmt(r.MQr)}</td></tr>`;
  });
  html += `</tbody></table></div>`;
  document.getElementById('mq-result').innerHTML = tape(`MQ戦略シミュレーション（${mode === 'PP' ? 'P' : 'Q'}を振る）`, html);
});

/* ---------------- F-STRAC ---------------- */
document.getElementById('form-f').addEventListener('submit', e=>{
  e.preventDefault();
  let P=num('f-P'),V=num('f-V'),Q=num('f-Q'),EH=num('f-EH'),F=num('f-F'),FM=num('f-FM'),N=num('f-N'),H=num('f-H');
  if(P===null) P = (V*Q + F*100/FM/N/H*EH)/Q;
  if(V===null) V = (P*Q - F*100/FM/N/H*EH)/Q;
  if(Q===null) Q = (F*100/FM/N/H*EH)/(P-V);
  if(EH===null) EH = (P*Q - V*Q)/(F*100/FM/N/H);
  if(F===null) F = (P*Q - V*Q)/EH*N*H*FM/100;
  if(FM===null) FM = F*100/(P*Q - V*Q)/N/H*EH;
  if(N===null) N = (F*100/FM/H*EH)/(P*Q - V*Q);
  if(H===null) H = (F*100/FM/N*EH)/(P*Q - V*Q);
  const PQ=P*Q, VQ=V*Q, TM=F*100/FM/N/H;
  let html = '';
  html += row('P',P)+row('V',V)+row('Q',Q)+row('EH',EH)+row('F',F)+row('FM',FM)+row('N',N)+row('H',H);
  html += rule();
  html += row('PQ',PQ)+row('VQ',VQ)+row('TM',TM, {highlight:true});
  html += row('V%', V/P*100, {unit:'%'});
  document.getElementById('f-result').innerHTML = tape('F-STRAC 結果', html);
});

/* ---------------- CF-STRAC ---------------- */
document.getElementById('form-cf').addEventListener('submit', e=>{
  e.preventDefault();
  let PQ=num('cf-PQ'),IN=num('cf-IN'),CF=num('cf-CF'),U1=num('cf-U1'),U2=num('cf-U2'),
      K1=num('cf-K1'),K2=num('cf-K2'),T=num('cf-T'),D=num('cf-D'),L=num('cf-L'),
      TG=num('cf-TG'),TA=num('cf-TA'),C1=num('cf-C1'),C2=num('cf-C2');

  if(PQ===null) PQ = C2-C1-(L+TG-D-T-TA)+(IN+K1-K2)+CF-(U1-U2);
  if(IN===null) IN = C1-C2+(L+TG-D-T-TA)+(PQ+U1-U2)-CF-(K1-K2);
  if(CF===null) CF = C1-C2+(L+TG-D-T-TA)+(PQ+U1-U2)-(IN+K1-K2);
  if(U1===null) U1 = C2-C1-(L+TG-D-T-TA)+(IN+K1-K2)+CF-(PQ-U2);
  if(U2===null) U2 = C1-C2+(L+TG-D-T-TA)-(IN+K1-K2)-CF+(PQ+U1);
  if(K1===null) K1 = C1-C2+(L+TG-D-T-TA)-(IN-K2)-CF+(PQ+U1-U2);
  if(K2===null) K2 = C2-C1-(L+TG-D-T-TA)+(IN+K1)+CF-(PQ+U1-U2);
  if(T===null)  T  = C1-C2+(PQ+U1-U2)-(IN+K1-K2)-CF+(L+TG-D-TA);
  if(D===null)  D  = C1-C2+(PQ+U1-U2)-(IN+K1-K2)-CF+(L+TG-T-TA);
  if(L===null)  L  = C2-C1-(PQ+U1-U2)+(IN+K1-K2)+CF-(TG-D-T-TA);
  if(TG===null) TG = C2-C1-(PQ+U1-U2)+(IN+K1-K2)+CF-(L-D-T-TA);
  if(TA===null) TA = C1-C2+(PQ+U1-U2)-(IN+K1-K2)-CF+(L+TG-D-T);
  if(C1===null) C1 = C2-(PQ+U1-U2)+(IN+K1-K2)+CF-(L+TG-D-T-TA);
  if(C2===null) C2 = C1+(PQ+U1-U2)-(IN+K1-K2)-CF+(L+TG-D-T-TA);

  const CPQ=PQ+U1-U2, CVQ=IN+K1-K2, CMQ=CPQ-CVQ;
  const CG=(PQ+U1-U2)-(IN+K1-K2)-CF;

  let html = '';
  html += row('PQ',PQ)+row('IN',IN)+row('CF',CF)+row('U1',U1)+row('U2',U2)+row('K1',K1)+row('K2',K2);
  html += row('T',T)+row('D',D)+row('L',L)+row('TG',TG)+row('TA',TA)+row('C1',C1)+row('C2',C2);
  html += rule();
  html += row('CPQ',CPQ)+row('CVQ',CVQ)+row('CMQ',CMQ, {highlight:true})+row('CF',CF)+row('CG',CG, {highlight:true});
  document.getElementById('cf-result').innerHTML = tape('CF-STRAC 結果', html);
});

/* ---------------- MGF ---------------- */
let mgfF = null;
document.getElementById('form-mgf').addEventListener('submit', e=>{
  e.preventDefault();
  const KI=num('mgf-KI'), N=num('mgf-N'), RITU=num('mgf-RITU'), D=num('mgf-D'), F3=num('mgf-F3'),
        SO=num('mgf-SO'), CH=num('mgf-CH'), EX=num('mgf-EX'), F5=num('mgf-F5'), FEX=num('mgf-FEX');
  const K1 = roundB((20+(KI-1)*2)*RITU);
  const K2 = roundB((10+(KI-1))*RITU);
  const F1 = N*K1;
  const F2 = D*K1 + SO*20 + 25 + N*K2;
  const F4 = CH*20 + EX*40;
  const F = F1+F2+F3+F4+F5+FEX;
  mgfF = F;
  shared.F = F;
  let html = '';
  html += row('F（固定費 合計）', F, {highlight:true});
  html += rule();
  html += row('F1（人件費）', F1);
  html += row('F2（設備・倉庫関連）', F2);
  html += row('F3（金利）', F3);
  html += row('F4（チップ・特急）', F4);
  html += row('F5（減価償却）', F5);
  html += row('FEX（その他）', FEX);
  html += `<div style="margin-top:14px;"><button type="button" class="btn secondary" id="mgf-to-k">この F で経営計画(K)へ進む</button></div>`;
  document.getElementById('mgf-result').innerHTML = tape('MGF 結果', html);
  document.getElementById('mgf-to-k').addEventListener('click', ()=>{
    document.getElementById('k-F').value = F;
    const box = document.getElementById('k-from-mgf');
    box.classList.remove('hidden');
    box.innerHTML = `MGF から引き継いだ F = ${fmt(F)}`;
    switchMode('k');
  });
});

/* ---------------- K 経営計画 ---------------- */
document.getElementById('form-k').addEventListener('submit', e=>{
  e.preventDefault();
  const F=num('k-F'), G=num('k-G'), V=num('k-V'), P=num('k-P');
  const SEI=num('k-SEI'), HAN=num('k-HAN'), JIK=num('k-JIK'), RI=num('k-RI');
  const MQ = F+G;
  const M = P-V;
  const Q = ceilB(MQ/M);
  const PQ = P*Q, VQ = V*Q, MQr = M*Q;
  const Q0 = ceilB(F/M);
  const GYOU = ceilB(Q/SEI)*2 + ceilB(Q/HAN) + JIK + RI;

  let html = '';
  html += row('MQ（必要限界利益）', MQ, {highlight:true});
  html += row('P', P)+row('V', V)+row('M', M)+row('Q（必要数量）', Q, {highlight:true});
  html += rule();
  html += row('PQ（売上高）', PQ)+row('VQ（変動費）', VQ)+row('MQ（限界利益）', MQr)+row('Q0（損益分岐点数量）', Q0);
  html += rule();
  html += row('必要行数（枚数）', GYOU, {unit:'行', highlight:true});
  document.getElementById('k-result').innerHTML = tape('経営計画（K）結果', html);
  shared.MQ = MQ; shared.V = V; shared.F = F; shared.P = P;
});

/* ---------------- nav ---------------- */
function switchMode(mode){
  syncSharedIntoForm(mode);
  document.querySelectorAll('.side-btn').forEach(b=>b.classList.toggle('active', b.dataset.mode===mode));
  document.querySelectorAll('.panel').forEach(p=>p.classList.toggle('active', p.id === 'panel-'+mode));
  window.scrollTo({top:0, behavior:'smooth'});
}
document.querySelectorAll('.side-btn').forEach(b=>{
  b.addEventListener('click', ()=> switchMode(b.dataset.mode));
});
switchMode('strac1');
</script>
</body>
</html>
