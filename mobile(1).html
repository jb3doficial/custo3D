<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1, viewport-fit=cover" />
  <meta name="theme-color" content="#111827" />
  <meta name="application-name" content="JB3D Cost Studio">
  <meta name="apple-mobile-web-app-capable" content="yes">
  <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
  <meta name="apple-mobile-web-app-title" content="JB3D Cost Studio">
  <meta name="mobile-web-app-capable" content="yes">
  <link rel="manifest" href="manifest-mobile.webmanifest">
  <link rel="icon" type="image/png" sizes="192x192" href="icons/icon-192.png">
  <link rel="icon" type="image/png" sizes="512x512" href="icons/icon-512.png">
  <link rel="apple-touch-icon" href="icons/icon-192.png">
  <title>JB3D Cost Studio</title>

  <style>
    :root{
      color-scheme:dark;
      --bg:#080b11;
      --sidebar:#0c1018;
      --workspace:#0f141e;
      --panel:#151c28;
      --panel-2:#192230;
      --panel-3:#101722;
      --line:#263246;
      --line-soft:rgba(151,174,212,.11);
      --text:#f3f6fb;
      --muted:#8491a8;
      --muted-2:#5f6c81;
      --accent:#7c6cff;
      --accent-2:#32c7f2;
      --green:#39d99a;
      --yellow:#f7c95d;
      --red:#ff6d7f;
      --shadow:0 18px 44px rgba(0,0,0,.28);
      --radius:16px;
      --sidebar-w:248px;
      --topbar-h:78px;
    }

    *{box-sizing:border-box}
    html,body{width:100%;height:100%;margin:0}
    html{background:var(--bg);scroll-behavior:smooth}
    body{
      overflow:hidden;
      color:var(--text);
      font-family:"Segoe UI Variable","Segoe UI",Inter,system-ui,-apple-system,sans-serif;
      background:var(--workspace);
    }

    button,input,select{font:inherit}
    button{cursor:pointer}
    button:focus-visible,input:focus-visible,select:focus-visible,summary:focus-visible{
      outline:2px solid var(--accent-2);
      outline-offset:2px;
    }

    @keyframes panelIn{
      from{opacity:0;transform:translateY(8px)}
      to{opacity:1;transform:none}
    }
    @keyframes headTravel{
      0%,100%{transform:translateX(-42px)}
      50%{transform:translateX(42px)}
    }
    @keyframes modelPulse{
      50%{filter:brightness(1.25);transform:scaleY(1.025)}
    }
    @keyframes printScan{
      from{transform:translateY(0);opacity:0}
      20%,80%{opacity:.85}
      to{transform:translateY(45px);opacity:0}
    }
    @keyframes spoolSpin{to{transform:rotate(360deg)}}
    @keyframes statusPulse{
      50%{box-shadow:0 0 0 7px rgba(57,217,154,0)}
    }
    @keyframes numberBump{50%{transform:scale(1.025)}}

    .app-shell{
      display:grid;
      grid-template-columns:var(--sidebar-w) minmax(0,1fr);
      width:100vw;
      height:100vh;
      background:var(--workspace);
    }

    /* Sidebar */
    .app-sidebar{
      position:relative;
      z-index:20;
      display:flex;
      min-height:0;
      flex-direction:column;
      padding:18px 14px 14px;
      border-right:1px solid #202a3a;
      background:
        radial-gradient(circle at 20% 0,rgba(124,108,255,.12),transparent 30%),
        var(--sidebar);
      box-shadow:12px 0 32px rgba(0,0,0,.14);
    }

    .brand{
      display:flex;
      align-items:center;
      gap:11px;
      min-height:48px;
      padding:0 8px 14px;
    }
    .brand-mark{
      position:relative;
      display:grid;
      width:39px;height:39px;
      flex:none;
      place-items:center;
      overflow:hidden;
      border:1px solid rgba(74,216,255,.28);
      border-radius:11px;
      background:linear-gradient(145deg,#6e67ff,#2dbfe9);
      box-shadow:0 9px 24px rgba(77,92,255,.25);
    }
    .brand-mark svg{width:24px;height:24px}
    .brand-name{font-size:.94rem;font-weight:850;letter-spacing:-.02em}
    .brand-sub{margin-top:2px;color:var(--muted-2);font-size:.65rem;font-weight:750;letter-spacing:.08em}

    .printer-monitor{
      position:relative;
      min-height:154px;
      margin:5px 2px 18px;
      overflow:hidden;
      border:1px solid var(--line);
      border-radius:15px;
      background:
        linear-gradient(145deg,rgba(124,108,255,.08),transparent 48%),
        #101722;
    }
    .monitor-head{
      display:flex;
      align-items:center;
      justify-content:space-between;
      padding:11px 12px 0;
      color:#b8c2d2;
      font-size:.68rem;
      font-weight:800;
    }
    .monitor-status{
      display:flex;align-items:center;gap:6px;
      color:#8be9c5;
    }
    .monitor-status::before{
      content:"";
      width:7px;height:7px;border-radius:50%;
      background:var(--green);
      box-shadow:0 0 0 0 rgba(57,217,154,.4);
      animation:statusPulse 1.8s infinite;
    }
    .mini-printer{
      position:absolute;
      left:50%;bottom:13px;
      width:145px;height:100px;
      margin-left:-72px;
      border:4px solid #38465b;
      border-bottom-width:8px;
      border-radius:5px 5px 10px 10px;
      background:rgba(5,9,15,.38);
    }
    .mini-printer::before,.mini-printer::after{
      content:"";
      position:absolute;
      top:-7px;bottom:-10px;
      width:7px;
      border-radius:4px;
      background:linear-gradient(90deg,#202b3c,#65738b,#263246);
    }
    .mini-printer::before{left:-7px}
    .mini-printer::after{right:-7px}
    .mini-gantry{
      position:absolute;
      left:10px;right:10px;top:28px;
      height:6px;border-radius:5px;
      background:#56647a;
    }
    .mini-head{
      position:absolute;
      left:50%;top:-8px;
      width:26px;height:23px;margin-left:-13px;
      border-radius:5px;
      background:#26344a;
      border:1px solid #53637c;
      animation:headTravel 3.2s ease-in-out infinite;
    }
    .mini-head::after{
      content:"";
      position:absolute;
      left:10px;top:21px;
      width:6px;height:11px;
      background:linear-gradient(#f2b95f,#916120);
      clip-path:polygon(15% 0,85% 0,100% 70%,50% 100%,0 70%);
    }
    .mini-bed{
      position:absolute;
      left:15px;right:15px;bottom:14px;
      height:8px;border-radius:3px;
      background:#344257;
      box-shadow:0 5px 10px rgba(0,0,0,.4);
    }
    .mini-model{
      position:absolute;
      left:50%;bottom:22px;
      width:48px;height:42px;margin-left:-24px;
      transform-origin:bottom;
      clip-path:polygon(22% 0,78% 0,100% 25%,92% 100%,8% 100%,0 25%);
      background:
        repeating-linear-gradient(to bottom,rgba(255,255,255,.18) 0 1px,transparent 1px 5px),
        linear-gradient(135deg,#8e66ff,#31c9ef);
      animation:modelPulse 2.5s ease-in-out infinite;
    }
    .mini-model::after{
      content:"";
      position:absolute;
      top:0;left:6px;right:6px;
      height:2px;border-radius:9px;
      background:#d5fbff;
      box-shadow:0 0 8px #4ad8ff;
      animation:printScan 2.6s linear infinite;
    }
    .mini-spool{
      position:absolute;
      right:-14px;top:-16px;
      width:37px;height:37px;
      border:7px solid #28354a;
      border-radius:50%;
      background:conic-gradient(#8a67ff,#33caf1,#8a67ff);
      animation:spoolSpin 9s linear infinite;
    }

    .nav-label{
      padding:0 11px 7px;
      color:#536077;
      font-size:.62rem;
      font-weight:850;
      letter-spacing:.13em;
      text-transform:uppercase;
    }
    .tabs{
      display:flex;
      flex-direction:column;
      gap:5px;
      margin:0;
      padding:0;
    }
    .tab-btn{
      position:relative;
      display:grid;
      grid-template-columns:34px minmax(0,1fr);
      align-items:center;
      min-height:52px;
      padding:7px 10px;
      border:1px solid transparent;
      border-radius:11px;
      color:#8d9ab0;
      text-align:left;
      background:transparent;
      font-size:.79rem;
      font-weight:750;
      transition:.18s ease;
    }
    .tab-icon{
      display:grid;
      width:30px;height:30px;
      place-items:center;
      border-radius:8px;
      color:#8795ad;
      background:rgba(255,255,255,.025);
      transition:.18s ease;
    }
    .tab-icon svg{width:17px;height:17px}
    .tab-copy strong{display:block;color:inherit;font-size:.78rem}
    .tab-copy small{display:block;margin-top:2px;color:#536077;font-size:.61rem;font-weight:650}
    .tab-btn:hover{
      color:#dce4f2;
      background:rgba(255,255,255,.035);
    }
    .tab-btn.active{
      color:white;
      border-color:rgba(83,200,240,.14);
      background:linear-gradient(90deg,rgba(124,108,255,.18),rgba(50,199,242,.075));
    }
    .tab-btn.active::before{
      content:"";
      position:absolute;
      left:-1px;top:11px;bottom:11px;
      width:3px;border-radius:5px;
      background:linear-gradient(var(--accent-2),var(--accent));
      box-shadow:0 0 12px rgba(50,199,242,.35);
    }
    .tab-btn.active .tab-icon{
      color:white;
      background:linear-gradient(145deg,rgba(124,108,255,.55),rgba(50,199,242,.25));
    }

    .sidebar-footer{
      margin-top:auto;
      padding:13px 10px 3px;
      border-top:1px solid rgba(151,174,212,.08);
    }
    .machine-line{
      display:flex;align-items:center;justify-content:space-between;gap:8px;
      color:#7f8da3;font-size:.65rem;
    }
    .machine-line strong{color:#b6c0d1;font-weight:800}
    .machine-chip{
      display:inline-flex;
      margin-top:9px;
      padding:6px 8px;
      border:1px solid rgba(57,217,154,.12);
      border-radius:8px;
      color:#7fdcb9;
      background:rgba(57,217,154,.045);
      font-size:.61rem;font-weight:800;
    }

    /* Workspace */
    .app-workspace{
      display:grid;
      grid-template-rows:var(--topbar-h) minmax(0,1fr);
      min-width:0;
      min-height:0;
      background:
        linear-gradient(rgba(110,132,170,.025) 1px,transparent 1px),
        linear-gradient(90deg,rgba(110,132,170,.025) 1px,transparent 1px),
        var(--workspace);
      background-size:32px 32px,32px 32px,auto;
    }
    .app-header{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:20px;
      padding:0 25px;
      border-bottom:1px solid #202a39;
      background:rgba(15,20,30,.94);
      backdrop-filter:blur(16px);
    }
    .page-kicker{
      display:block;
      margin-bottom:3px;
      color:#66748a;
      font-size:.61rem;
      font-weight:850;
      letter-spacing:.13em;
      text-transform:uppercase;
    }
    .page-title{
      margin:0;
      color:#f4f7fb;
      font-size:1.16rem;
      font-weight:820;
      letter-spacing:-.025em;
    }
    .header-actions{
      display:flex;
      align-items:center;
      gap:9px;
    }
    .save-status{
      display:flex;
      align-items:center;
      gap:7px;
      min-height:34px;
      padding:0 11px;
      border:1px solid var(--line-soft);
      border-radius:9px;
      color:#7f8ca1;
      background:rgba(255,255,255,.025);
      font-size:.67rem;
      font-weight:700;
    }
    .save-status::before{
      content:"";
      width:6px;height:6px;border-radius:50%;
      background:var(--green);
      box-shadow:0 0 8px rgba(57,217,154,.55);
    }
    .install-app-btn{
      display:none;
      align-items:center;
      gap:7px;
      min-height:36px;
      padding:0 12px;
      border:1px solid rgba(91,199,237,.2);
      border-radius:9px;
      color:#eafaff;
      background:linear-gradient(135deg,rgba(124,108,255,.7),rgba(50,199,242,.45));
      font-size:.68rem;
      font-weight:820;
    }
    .install-app-btn.show{display:flex}
    .install-app-btn.installed{display:none!important}

    .app-content{
      min-width:0;
      min-height:0;
      overflow:auto;
      padding:20px 22px 35px;
      scrollbar-color:#344156 transparent;
      scrollbar-width:thin;
    }
    .app-content::-webkit-scrollbar{width:9px}
    .app-content::-webkit-scrollbar-track{background:transparent}
    .app-content::-webkit-scrollbar-thumb{
      border:2px solid transparent;
      border-radius:10px;
      background:#354158;
      background-clip:padding-box;
    }

    .tab-panel{display:none;animation:panelIn .2s ease both}
    .tab-panel.active{display:block}

    .layout{
      display:grid;
      grid-template-columns:minmax(0,1.2fr) minmax(340px,.8fr);
      gap:18px;
      align-items:start;
      max-width:1260px;
      margin:0 auto;
    }
    .stack{display:grid;gap:16px}

    .card{
      overflow:hidden;
      border:1px solid var(--line);
      border-radius:var(--radius);
      background:rgba(21,28,40,.96);
      box-shadow:var(--shadow);
    }
    .card-inner{padding:21px}
    .card-title{
      display:flex;
      align-items:flex-start;
      justify-content:space-between;
      gap:15px;
      margin-bottom:20px;
      padding-bottom:15px;
      border-bottom:1px solid rgba(151,174,212,.09);
    }
    .card-title h2,.card-title h3{
      margin:0;
      color:#eef2f8;
      font-size:.98rem;
      font-weight:820;
      letter-spacing:-.018em;
    }
    .card-title .hint{margin-top:5px}
    .badge{
      display:inline-flex;
      align-items:center;
      gap:6px;
      min-height:25px;
      padding:0 8px;
      border:1px solid rgba(57,217,154,.13);
      border-radius:7px;
      color:#83dfbd;
      background:rgba(57,217,154,.045);
      font-size:.59rem;
      font-weight:850;
      white-space:nowrap;
    }
    .badge::before{
      content:"";
      width:5px;height:5px;border-radius:50%;
      background:var(--green);
    }

    .grid{
      display:grid;
      grid-template-columns:repeat(2,minmax(0,1fr));
      gap:14px 15px;
    }
    .field{display:grid;min-width:0;gap:7px}
    .field.full{grid-column:1/-1}
    label{
      color:#bdc7d7;
      font-size:.72rem;
      font-weight:750;
    }
    .hint{
      color:#68768d;
      font-size:.65rem;
      line-height:1.42;
    }
    .input-wrap{
      display:flex;
      align-items:center;
      min-height:48px;
      overflow:hidden;
      border:1px solid #2b374a;
      border-radius:10px;
      background:#101722;
      transition:.16s ease;
    }
    .input-wrap:hover{border-color:#394961}
    .input-wrap:focus-within{
      border-color:rgba(50,199,242,.7);
      box-shadow:0 0 0 3px rgba(50,199,242,.07);
    }
    .prefix,.suffix{
      padding:0 11px;
      color:#75839a;
      font-size:.72rem;
      font-weight:800;
      white-space:nowrap;
    }
    input,select{
      width:100%;
      min-width:0;
      padding:13px 11px;
      border:0;
      outline:0;
      color:#f5f7fb;
      background:transparent;
      font-size:.82rem;
      font-weight:760;
    }
    input::placeholder{color:#536078}
    select option{color:#111;background:#fff}
    input::-webkit-outer-spin-button,input::-webkit-inner-spin-button{margin:0}

    details{
      margin-top:16px;
      overflow:hidden;
      border:1px solid #283448;
      border-radius:11px;
      background:#121925;
    }
    summary{
      position:relative;
      padding:14px 41px 14px 14px;
      list-style:none;
      color:#b9c4d6;
      font-size:.72rem;
      font-weight:780;
      cursor:pointer;
    }
    summary::-webkit-details-marker{display:none}
    summary::after{
      content:"+";
      position:absolute;
      top:50%;right:14px;
      color:#728099;
      font-size:1rem;
      transform:translateY(-50%);
      transition:.16s ease;
    }
    details[open] summary{border-bottom:1px solid #283448}
    details[open] summary::after{transform:translateY(-50%) rotate(45deg)}
    .advanced{padding:15px}

    .machine-profile{
      grid-column:1/-1;
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:12px;
      padding:13px;
      border:1px solid rgba(50,199,242,.13);
      border-radius:10px;
      background:linear-gradient(90deg,rgba(124,108,255,.07),rgba(50,199,242,.035));
    }
    .machine-profile strong{display:block;color:#dfe6f1;font-size:.75rem}
    .machine-profile small{display:block;margin-top:4px;color:#68768c;font-size:.63rem;line-height:1.4}
    .profile-tag{
      flex:none;
      padding:6px 8px;
      border:1px solid rgba(50,199,242,.13);
      border-radius:7px;
      color:#79d8f3;
      background:rgba(50,199,242,.045);
      font-size:.56rem;
      font-weight:850;
    }

    .result-card{
      position:sticky;
      top:0;
      border-color:#2b3a50;
    }
    .result-top{
      position:relative;
      overflow:hidden;
      padding:22px 21px 19px;
      border-bottom:1px solid #29364a;
      background:
        radial-gradient(circle at 100% 0,rgba(50,199,242,.12),transparent 42%),
        linear-gradient(135deg,rgba(124,108,255,.10),transparent);
    }
    .result-label{
      color:#78869c;
      font-size:.61rem;
      font-weight:850;
      letter-spacing:.11em;
      text-transform:uppercase;
    }
    .big-value{
      margin-top:7px;
      color:#f7f9fc;
      font-size:clamp(2.25rem,4.5vw,3.65rem);
      line-height:1;
      font-weight:900;
      letter-spacing:-.055em;
      overflow-wrap:anywhere;
      transition:.14s ease;
    }
    .big-value.bump{animation:numberBump .18s ease}
    .sub-value{margin-top:9px;color:#718097;font-size:.68rem}
    .breakdown{display:grid;padding:9px 18px 17px}
    .row{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:17px;
      padding:10px 2px;
      border-bottom:1px solid rgba(151,174,212,.07);
      color:#8e9bb0;
      font-size:.7rem;
    }
    .row strong{color:#dce3ee;text-align:right}
    .row:last-child{border-bottom:0}
    .row.total{
      margin-top:9px;
      padding:12px;
      border:1px solid rgba(57,217,154,.13);
      border-radius:9px;
      color:#a4e9d0;
      background:rgba(57,217,154,.04);
    }
    .row.negative strong{color:var(--red)}
    .row.positive strong{color:var(--green)}

    .actions{
      display:flex;
      flex-wrap:wrap;
      gap:8px;
      margin-top:16px;
    }
    .btn{
      min-height:40px;
      padding:0 13px;
      border:1px solid #304057;
      border-radius:9px;
      color:#cbd5e3;
      background:#192230;
      font-size:.68rem;
      font-weight:800;
      transition:.16s ease;
    }
    .btn:hover{
      border-color:#435570;
      color:white;
      background:#202b3b;
      transform:translateY(-1px);
    }
    .btn.primary{
      border-color:transparent;
      color:white;
      background:linear-gradient(135deg,#7669fa,#536ff1 55%,#36b9df);
      box-shadow:0 8px 18px rgba(71,85,210,.18);
    }
    .btn.danger{color:#ff9daa}

    /* Controle ROAS estilo plataforma */
    .roas-control{
      padding:14px;
      border:1px solid #2d3b50;
      border-radius:12px;
      background:#111925;
    }
    .roas-title-line{
      display:flex;
      align-items:center;
      justify-content:space-between;
      gap:12px;
      margin-bottom:11px;
    }
    .roas-title-line label{font-size:.75rem}
    .shopee-style-chip{
      padding:5px 7px;
      border:1px solid rgba(247,201,93,.15);
      border-radius:7px;
      color:#e9c66a;
      background:rgba(247,201,93,.045);
      font-size:.55rem;
      font-weight:850;
    }
    .roas-layout{
      display:grid;
      grid-template-columns:minmax(190px,.55fr) minmax(0,1fr);
      gap:11px;
    }
    .roas-input-wrap{
      min-height:58px;
      border-color:rgba(124,108,255,.35);
      background:linear-gradient(135deg,rgba(124,108,255,.12),rgba(16,23,34,.9));
    }
    .roas-input-wrap .prefix{
      color:#c7c0ff;
      font-size:.68rem;
      letter-spacing:.06em;
    }
    .roas-input-wrap input{
      font-size:1.12rem;
      font-weight:880;
      text-align:center;
    }
    .roas-input-wrap .suffix{
      color:#9d91ff;
      font-size:.86rem;
    }
    .roas-metrics{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:8px;
    }
    .roas-metric{
      display:flex;
      min-width:0;
      flex-direction:column;
      justify-content:center;
      padding:9px 11px;
      border:1px solid #29364a;
      border-radius:9px;
      background:#0f1621;
    }
    .roas-metric span{
      color:#647187;
      font-size:.57rem;
      font-weight:750;
      text-transform:uppercase;
      letter-spacing:.06em;
    }
    .roas-metric strong{
      margin-top:5px;
      color:#e5ebf4;
      font-size:.78rem;
      overflow-wrap:anywhere;
    }
    .roas-help{
      margin-top:10px;
      color:#69778d;
      font-size:.64rem;
      line-height:1.45;
    }
    .roas-help strong{color:#aeb9ca}

    .profit-meter{
      height:7px;
      margin-top:15px;
      overflow:hidden;
      border-radius:99px;
      background:#242f40;
    }
    .profit-meter>span{
      display:block;
      width:0;height:100%;
      border-radius:inherit;
      background:linear-gradient(90deg,var(--red),var(--yellow),var(--green));
      transition:width .35s ease;
    }

    .notice{
      margin-top:13px;
      padding:11px 12px;
      border:1px solid rgba(247,201,93,.11);
      border-radius:9px;
      color:#9e9479;
      background:rgba(247,201,93,.03);
      font-size:.63rem;
      line-height:1.45;
    }

    .products-toolbar{
      display:grid;
      grid-template-columns:minmax(0,1fr) auto;
      gap:12px;
      align-items:end;
      margin-bottom:16px;
    }
    .search-icon{padding-left:11px;color:#748198;font-size:.75rem}
    .clear-search{
      display:none;padding:11px;border:0;
      color:#718097;background:transparent;font-weight:850;
    }
    .clear-search.show{display:block}
    .products-summary{padding-bottom:3px;color:#69778d;font-size:.64rem;text-align:right}
    .saved-products{display:grid;gap:9px}
    .saved-empty{
      padding:29px 16px;
      border:1px dashed #2b384c;
      border-radius:11px;
      color:#66748b;
      text-align:center;
      background:#111823;
      font-size:.72rem;
    }
    .product-item{
      display:grid;
      grid-template-columns:minmax(0,1fr) auto;
      gap:13px;
      align-items:center;
      padding:12px 13px;
      border:1px solid #29364a;
      border-radius:10px;
      background:#121a26;
      transition:.15s ease;
    }
    .product-item:hover{border-color:#3b4c66;background:#151e2b}
    .product-name{color:#dce3ee;font-size:.75rem;font-weight:820;overflow-wrap:anywhere}
    .product-meta{margin-top:3px;color:#657289;font-size:.59rem}
    .product-value{margin-top:5px;color:#72ddb5;font-size:.83rem;font-weight:860}
    .product-actions{display:flex;flex-wrap:wrap;gap:6px;justify-content:flex-end}
    .mini-btn{
      min-height:34px;padding:0 9px;
      border:1px solid #304057;border-radius:8px;
      color:#b9c4d4;background:#192230;
      font-size:.59rem;font-weight:800;
    }
    .mini-btn:hover{border-color:#435570;color:white}
    .mini-btn.delete{color:#ff9ba8}

    .modal-backdrop{
      position:fixed;inset:0;z-index:100;
      display:none;place-items:center;padding:18px;
      background:rgba(4,7,12,.74);
      backdrop-filter:blur(9px);
    }
    .modal-backdrop.show{display:grid;animation:panelIn .16s ease both}
    .modal{
      width:min(440px,100%);
      overflow:hidden;
      border:1px solid #314059;
      border-radius:15px;
      background:#151d29;
      box-shadow:0 30px 90px rgba(0,0,0,.48);
    }
    .modal-header{padding:19px 20px 9px}
    .modal-header h3{margin:0 0 5px;font-size:.95rem}
    .modal-header p{margin:0;color:#748197;font-size:.67rem;line-height:1.45}
    .modal-body{padding:9px 20px 20px}
    .modal-cost{
      display:flex;justify-content:space-between;gap:13px;
      margin:13px 0;padding:12px;
      border:1px solid rgba(57,217,154,.12);
      border-radius:9px;color:#8f9cb0;
      background:rgba(57,217,154,.035);
      font-size:.69rem;
    }
    .modal-cost strong{color:#70ddb4}
    .modal-actions{display:flex;gap:8px;margin-top:15px}
    .modal-actions .btn{flex:1}

    .toast{
      position:fixed;
      left:50%;bottom:21px;z-index:120;
      max-width:min(90vw,480px);
      padding:10px 14px;
      border:1px solid rgba(57,217,154,.2);
      border-radius:9px;
      color:#c9f5e4;background:#17372d;
      box-shadow:0 15px 40px rgba(0,0,0,.35);
      font-size:.68rem;font-weight:820;
      opacity:0;pointer-events:none;
      transform:translate(-50%,18px);
      transition:.18s ease;
    }
    .toast.show{opacity:1;transform:translate(-50%,0)}

    @media(max-width:1050px){
      :root{--sidebar-w:215px}
      .layout{grid-template-columns:1fr}
      .result-card{position:relative}
      .roas-layout{grid-template-columns:1fr}
    }

    @media(max-width:760px){
      body{overflow:auto}
      .app-shell{
        display:block;
        min-height:100vh;
        height:auto;
      }
      .app-sidebar{
        position:sticky;top:0;
        min-height:auto;
        padding:8px 9px;
        border-right:0;border-bottom:1px solid #202a3a;
      }
      .brand,.printer-monitor,.nav-label,.sidebar-footer{display:none}
      .tabs{
        display:grid;
        grid-template-columns:repeat(3,minmax(0,1fr));
        gap:5px;
      }
      .tab-btn{
        display:flex;
        min-height:45px;
        justify-content:center;
        padding:6px;
        text-align:center;
      }
      .tab-icon{display:none}
      .tab-copy strong{font-size:.68rem}
      .tab-copy small{display:none}
      .tab-btn.active::before{
        left:11px;right:11px;top:auto;bottom:-1px;
        width:auto;height:3px;
      }
      .app-workspace{display:block}
      .app-header{
        min-height:67px;
        padding:0 14px;
      }
      .page-title{font-size:1rem}
      .save-status{display:none}
      .app-content{
        overflow:visible;
        padding:13px 11px 85px;
      }
      .grid{grid-template-columns:1fr}
      .field.full{grid-column:auto}
      .card-inner{padding:17px}
      .machine-profile{align-items:flex-start;flex-direction:column}
      .products-toolbar{grid-template-columns:1fr}
      .products-summary{text-align:left}
      .product-item{grid-template-columns:1fr}
      .product-actions{justify-content:flex-start}
      .roas-metrics{grid-template-columns:1fr 1fr}
    }

    @media(max-width:450px){
      .header-actions{gap:5px}
      .install-app-btn{padding:0 9px;font-size:.61rem}
      .roas-metrics{grid-template-columns:1fr}
      .btn{flex:1}
    }

    @media(prefers-reduced-motion:reduce){
      *,*::before,*::after{animation:none!important;transition:none!important;scroll-behavior:auto!important}
    }

    .sync-layout{
      display:grid;
      grid-template-columns:minmax(0,1fr) minmax(0,1fr);
      gap:18px;
      max-width:1260px;
      margin:0 auto;
    }
    .sync-status-card{
      max-width:1260px;
      margin:18px auto 0;
    }
    .sync-device-row{
      display:grid;
      grid-template-columns:minmax(0,1fr) auto;
      gap:12px;
      align-items:end;
    }
    .sync-data-summary{
      display:flex;
      min-height:48px;
      align-items:center;
      gap:12px;
      padding:0 12px;
      border:1px solid #2b374a;
      border-radius:10px;
      color:#77859b;
      background:#101722;
      font-size:.64rem;
      white-space:nowrap;
    }
    .sync-data-summary strong{color:#dce5f2}
    .sync-options{
      display:flex;
      flex-wrap:wrap;
      gap:9px;
      margin-top:13px;
    }
    .sync-check{
      display:flex;
      align-items:center;
      gap:8px;
      min-height:37px;
      padding:0 10px;
      border:1px solid #2b374a;
      border-radius:9px;
      color:#a7b2c3;
      background:#111925;
      font-size:.66rem;
      cursor:pointer;
    }
    .sync-check input{
      width:15px;
      accent-color:var(--accent);
    }
    .sync-qr-stage{
      display:grid;
      min-height:392px;
      margin-top:16px;
      place-items:center;
      padding:17px;
      border:1px solid #29364a;
      border-radius:13px;
      background:
        linear-gradient(rgba(151,174,212,.025) 1px,transparent 1px),
        linear-gradient(90deg,rgba(151,174,212,.025) 1px,transparent 1px),
        #101722;
      background-size:22px 22px;
    }
    .sync-qr-empty{
      display:grid;
      max-width:270px;
      place-items:center;
      gap:7px;
      color:#68768c;
      text-align:center;
    }
    .sync-qr-empty-icon{
      display:grid;
      width:57px;height:57px;
      place-items:center;
      border:1px solid #344158;
      border-radius:16px;
      color:#7785a0;
      background:#151e2b;
      font-size:1.6rem;
    }
    .sync-qr-empty strong{color:#9aa7ba;font-size:.75rem}
    .sync-qr-empty small{font-size:.63rem;line-height:1.4}
    .sync-qr-active{width:100%;text-align:center}
    .sync-qr-paper{
      display:inline-grid;
      place-items:center;
      padding:15px;
      border-radius:15px;
      background:white;
      box-shadow:0 17px 45px rgba(0,0,0,.34);
    }
    .sync-qr-code{
      width:280px;
      height:280px;
    }
    .sync-qr-code img,.sync-qr-code canvas{
      display:block!important;
      width:280px!important;
      height:280px!important;
    }
    .sync-frame-info{
      display:grid;
      gap:3px;
      margin-top:13px;
      color:#7c8aa1;
      font-size:.64rem;
    }
    .sync-frame-info strong{color:#d6deea;font-size:.72rem}
    .sync-frame-controls{
      display:flex;
      justify-content:center;
      flex-wrap:wrap;
      gap:7px;
      margin-top:11px;
    }
    .sync-reader-actions{
      display:flex;
      flex-wrap:wrap;
      gap:8px;
    }
    .sync-file-button{
      display:inline-flex;
      align-items:center;
      justify-content:center;
    }
    .sync-scanner-shell{
      position:relative;
      min-height:315px;
      margin-top:15px;
      overflow:hidden;
      border:1px solid #29364a;
      border-radius:13px;
      background:#090e16;
    }
    .sync-scanner{
      position:relative;
      min-height:315px;
      overflow:hidden;
      background:#060a10;
    }
    .sync-scanner video{
      display:none;
      width:100%!important;
      height:315px;
      min-height:315px;
      object-fit:cover;
      background:#060a10;
    }
    .sync-scanner video.active{display:block}
    .sync-scanner-fallback{
      display:none;
      min-height:315px;
    }
    .sync-scanner-fallback.active{display:block}
    .sync-scanner-fallback video{
      display:block!important;
      width:100%!important;
      min-height:315px!important;
      object-fit:cover!important;
    }
    .sync-camera-guide{
      position:absolute;
      inset:50% auto auto 50%;
      z-index:5;
      width:min(68%,250px);
      aspect-ratio:1;
      pointer-events:none;
      transform:translate(-50%,-50%);
    }
    .sync-camera-guide span{
      position:absolute;
      width:42px;
      height:42px;
      border-color:#72e4ff;
      filter:drop-shadow(0 0 5px rgba(50,199,242,.45));
    }
    .sync-camera-guide span:nth-child(1){
      left:0;top:0;
      border-left:4px solid;
      border-top:4px solid;
      border-radius:12px 0 0 0;
    }
    .sync-camera-guide span:nth-child(2){
      right:0;top:0;
      border-right:4px solid;
      border-top:4px solid;
      border-radius:0 12px 0 0;
    }
    .sync-camera-guide span:nth-child(3){
      left:0;bottom:0;
      border-left:4px solid;
      border-bottom:4px solid;
      border-radius:0 0 0 12px;
    }
    .sync-camera-guide span:nth-child(4){
      right:0;bottom:0;
      border-right:4px solid;
      border-bottom:4px solid;
      border-radius:0 0 12px 0;
    }
    .sync-camera-diagnostic{
      margin-top:10px;
      padding:10px 11px;
      border:1px solid #29364a;
      border-radius:9px;
      color:#718097;
      background:#111925;
      font-size:.61rem;
      line-height:1.45;
    }
    .sync-camera-diagnostic.error{
      border-color:rgba(255,109,127,.18);
      color:#d79aa4;
      background:rgba(255,109,127,.04);
    }
    .sync-camera-diagnostic.success{
      border-color:rgba(57,217,154,.16);
      color:#84cdb1;
      background:rgba(57,217,154,.04);
    }
    .sync-scanner-placeholder{
      position:absolute;
      inset:0;
      display:grid;
      place-content:center;
      gap:7px;
      padding:20px;
      color:#647188;
      text-align:center;
      pointer-events:none;
    }
    .sync-scanner-placeholder span{
      color:#7b89a2;
      font-size:2.1rem;
    }
    .sync-scanner-placeholder strong{color:#919eb1;font-size:.75rem}
    .sync-scanner-placeholder small{max-width:260px;font-size:.62rem;line-height:1.4}
    .sync-progress-card{
      margin-top:13px;
      padding:12px;
      border:1px solid #29364a;
      border-radius:10px;
      background:#111925;
    }
    .sync-progress-head{
      display:flex;
      justify-content:space-between;
      gap:12px;
      color:#718097;
      font-size:.61rem;
    }
    .sync-progress-head strong{color:#aeb9c9}
    .sync-progress-track{
      height:6px;
      margin-top:9px;
      overflow:hidden;
      border-radius:99px;
      background:#263246;
    }
    .sync-progress-track span{
      display:block;
      width:0;
      height:100%;
      border-radius:inherit;
      background:linear-gradient(90deg,var(--accent),var(--accent-2));
      transition:width .25s ease;
    }
    .sync-scan-message{
      margin-top:8px;
      color:#65738a;
      font-size:.61rem;
      line-height:1.35;
    }
    .sync-text-details{margin-top:13px}
    .sync-textarea{
      width:100%;
      min-height:105px;
      resize:vertical;
      padding:11px;
      border:1px solid #2d3a4e;
      border-radius:9px;
      outline:0;
      color:#c8d2e1;
      background:#0c121c;
      font:600 .62rem/1.45 ui-monospace,SFMono-Regular,Consolas,monospace;
    }
    .sync-textarea:focus{
      border-color:rgba(50,199,242,.65);
      box-shadow:0 0 0 3px rgba(50,199,242,.06);
    }
    .sync-note{
      margin-top:13px;
      padding:10px 11px;
      border:1px solid rgba(247,201,93,.11);
      border-radius:9px;
      color:#988e73;
      background:rgba(247,201,93,.03);
      font-size:.61rem;
      line-height:1.45;
    }
    .sync-import-preview{
      display:grid;
      grid-template-columns:38px minmax(0,1fr) auto;
      gap:11px;
      align-items:center;
      margin-top:13px;
      padding:12px;
      border:1px solid rgba(57,217,154,.16);
      border-radius:11px;
      background:rgba(57,217,154,.04);
    }
    .sync-import-icon{
      display:grid;
      width:36px;height:36px;
      place-items:center;
      border-radius:10px;
      color:#0e251d;
      background:var(--green);
      font-weight:900;
    }
    .sync-import-copy{display:grid;gap:3px;min-width:0}
    .sync-import-copy strong{color:#d9eee6;font-size:.7rem}
    .sync-import-copy span{color:#759286;font-size:.61rem;line-height:1.35}
    .sync-status-grid{
      display:grid;
      grid-template-columns:repeat(3,minmax(0,1fr));
      gap:14px;
    }
    .sync-status-grid>div{
      display:grid;
      gap:5px;
      padding:11px 12px;
      border:1px solid #29364a;
      border-radius:9px;
      background:#111925;
    }
    .sync-status-grid span{
      color:#647188;
      font-size:.57rem;
      font-weight:750;
      text-transform:uppercase;
      letter-spacing:.06em;
    }
    .sync-status-grid strong{
      color:#cbd4e1;
      font-size:.68rem;
      overflow-wrap:anywhere;
    }

    @media(max-width:1050px){
      .sync-layout{grid-template-columns:1fr}
    }
    @media(max-width:760px){
      .tabs{grid-template-columns:repeat(4,minmax(0,1fr))}
      .sync-device-row{grid-template-columns:1fr}
      .sync-data-summary{white-space:normal}
      .sync-qr-stage{min-height:370px;padding:12px}
      .sync-qr-code,.sync-qr-code img,.sync-qr-code canvas{
        width:min(74vw,280px)!important;
        height:min(74vw,280px)!important;
      }
      .sync-status-grid{grid-template-columns:1fr}
      .sync-import-preview{grid-template-columns:38px minmax(0,1fr)}
      .sync-import-preview .btn{grid-column:1/-1}
    }

  </style>


  <style id="mobile-app-style">
    body.mobile-app{
      overflow:hidden;
      background:#0b1018;
      overscroll-behavior:none;
    }
    .mobile-app .app-shell{
      display:block;
      width:100%;
      height:100dvh;
      min-height:100dvh;
    }
    .mobile-app .app-sidebar{
      position:fixed;
      inset:auto 0 0 0;
      z-index:80;
      display:block;
      min-height:0;
      height:calc(72px + env(safe-area-inset-bottom));
      padding:7px 8px env(safe-area-inset-bottom);
      border:0;
      border-top:1px solid #283448;
      background:rgba(12,16,24,.96);
      box-shadow:0 -12px 35px rgba(0,0,0,.34);
      backdrop-filter:blur(18px);
    }
    .mobile-app .brand,
    .mobile-app .printer-monitor,
    .mobile-app .nav-label,
    .mobile-app .sidebar-footer{
      display:none!important;
    }
    .mobile-app .tabs{
      display:grid;
      grid-template-columns:repeat(4,minmax(0,1fr));
      gap:4px;
      height:100%;
    }
    .mobile-app .tab-btn{
      display:flex;
      min-width:0;
      min-height:56px;
      flex-direction:column;
      justify-content:center;
      gap:3px;
      padding:4px 2px;
      border:0;
      border-radius:11px;
      text-align:center;
    }
    .mobile-app .tab-btn::before{
      left:50%;
      top:0;
      bottom:auto;
      width:24px;
      height:3px;
      transform:translateX(-50%);
    }
    .mobile-app .tab-icon{
      display:grid;
      width:25px;height:25px;
      flex:none;
      place-items:center;
      padding:0;
      border-radius:7px;
    }
    .mobile-app .tab-icon svg{width:15px;height:15px}
    .mobile-app .tab-copy strong{
      display:block;
      max-width:76px;
      overflow:hidden;
      font-size:.56rem;
      line-height:1.15;
      text-overflow:ellipsis;
      white-space:nowrap;
    }
    .mobile-app .tab-copy small{display:none}
    .mobile-app .app-workspace{
      display:grid;
      width:100%;
      height:100dvh;
      min-height:0;
      grid-template-rows:calc(63px + env(safe-area-inset-top)) minmax(0,1fr);
    }
    .mobile-app .app-header{
      position:relative;
      z-index:30;
      min-height:0;
      padding:env(safe-area-inset-top) 13px 0;
      border-bottom:1px solid #263246;
      background:rgba(15,20,30,.96);
      backdrop-filter:blur(18px);
    }
    .mobile-app .page-kicker{font-size:.52rem}
    .mobile-app .page-title{font-size:.96rem}
    .mobile-app .header-actions{gap:6px}
    .mobile-app .save-status{display:none}
    .mobile-app .desktop-version-link{
      display:inline-flex;
      min-height:31px;
      align-items:center;
      padding:0 9px;
      border:1px solid #2d3a4e;
      border-radius:8px;
      color:#8997ac;
      background:#151d29;
      font-size:.56rem;
      font-weight:800;
      text-decoration:none;
    }
    .mobile-app .install-app-btn{
      min-height:31px;
      padding:0 9px;
      border-radius:8px;
      font-size:.56rem;
    }
    .mobile-app .app-content{
      min-height:0;
      overflow:auto;
      padding:12px 10px calc(88px + env(safe-area-inset-bottom));
      scrollbar-width:none;
      -webkit-overflow-scrolling:touch;
    }
    .mobile-app .app-content::-webkit-scrollbar{display:none}
    .mobile-app .layout,
    .mobile-app .sync-layout{
      display:grid;
      grid-template-columns:1fr;
      gap:12px;
      width:100%;
      margin:0;
    }
    .mobile-app .stack{gap:12px}
    .mobile-app .card{
      border-radius:14px;
      box-shadow:0 10px 28px rgba(0,0,0,.22);
    }
    .mobile-app .card-inner{padding:15px}
    .mobile-app .card-title{
      margin-bottom:15px;
      padding-bottom:12px;
    }
    .mobile-app .card-title h2,
    .mobile-app .card-title h3{
      font-size:.88rem;
    }
    .mobile-app .badge{font-size:.52rem}
    .mobile-app .grid{grid-template-columns:1fr;gap:12px}
    .mobile-app .field.full{grid-column:auto}
    .mobile-app label{font-size:.67rem}
    .mobile-app .input-wrap{min-height:51px;border-radius:11px}
    .mobile-app input,.mobile-app select{font-size:.88rem}
    .mobile-app .hint{font-size:.61rem}
    .mobile-app .machine-profile{
      align-items:flex-start;
      flex-direction:column;
    }
    .mobile-app .result-card{
      position:relative;
      top:auto;
      order:-1;
    }
    .mobile-app .result-top{padding:19px 17px}
    .mobile-app .big-value{font-size:2.65rem}
    .mobile-app .breakdown{padding:7px 15px 15px}
    .mobile-app .row{font-size:.67rem}
    .mobile-app .actions{
      display:grid;
      grid-template-columns:repeat(2,minmax(0,1fr));
      gap:8px;
    }
    .mobile-app .actions .btn{
      width:100%;
      min-height:44px;
      padding:0 8px;
      font-size:.62rem;
    }
    .mobile-app .roas-layout{grid-template-columns:1fr}
    .mobile-app .roas-metrics{grid-template-columns:1fr 1fr}
    .mobile-app .products-toolbar{grid-template-columns:1fr}
    .mobile-app .products-summary{text-align:left}
    .mobile-app .product-item{grid-template-columns:1fr}
    .mobile-app .product-actions{justify-content:flex-start}
    .mobile-app .sync-device-row{grid-template-columns:1fr}
    .mobile-app .sync-options{
      display:grid;
      grid-template-columns:1fr 1fr;
    }
    .mobile-app .sync-check{
      justify-content:center;
      padding:0 7px;
      text-align:center;
    }
    .mobile-app .sync-qr-stage{
      min-height:348px;
      padding:11px;
    }
    .mobile-app .sync-qr-paper{padding:11px}
    .mobile-app .sync-qr-code,
    .mobile-app .sync-qr-code img,
    .mobile-app .sync-qr-code canvas{
      width:min(72vw,275px)!important;
      height:min(72vw,275px)!important;
    }
    .mobile-app .sync-frame-controls{
      display:grid;
      grid-template-columns:repeat(3,minmax(0,1fr));
    }
    .mobile-app .sync-frame-controls .mini-btn{
      padding:0 5px;
      font-size:.54rem;
    }
    .mobile-app .sync-reader-actions{
      display:grid;
      grid-template-columns:repeat(3,minmax(0,1fr));
    }
    .mobile-app .sync-reader-actions .btn{padding:0 5px}
    .mobile-app .sync-scanner-shell,
    .mobile-app .sync-scanner,
    .mobile-app .sync-scanner video{
      min-height:285px;
    }
    .mobile-app .sync-import-preview{
      grid-template-columns:35px minmax(0,1fr);
    }
    .mobile-app .sync-import-preview .btn{grid-column:1/-1}
    .mobile-app .sync-status-grid{grid-template-columns:1fr}
    .mobile-app .sync-status-card{margin-top:12px}
    .mobile-app .modal{border-radius:16px}
    .mobile-app .toast{
      bottom:calc(82px + env(safe-area-inset-bottom));
    }
  </style>

</head>
<body class="mobile-app">
  <div class="app-shell">
    <aside class="app-sidebar">
      <div class="brand">
        <div class="brand-mark" aria-hidden="true">
          <svg viewBox="0 0 24 24" fill="none">
            <path d="M12 2.8 20 7.2v9.6L12 21.2 4 16.8V7.2L12 2.8Z" stroke="currentColor" stroke-width="1.7"/>
            <path d="m4.4 7.4 7.6 4.2 7.6-4.2M12 11.6v9" stroke="currentColor" stroke-width="1.7"/>
          </svg>
        </div>
        <div>
          <div class="brand-name">JB3D Cost Studio</div>
          <div class="brand-sub">PRODUCTION DESKTOP</div>
        </div>
      </div>

      <div class="printer-monitor" aria-hidden="true">
        <div class="monitor-head">
          <span>CREALITY K2 PLUS</span>
          <span class="monitor-status">ONLINE</span>
        </div>
        <div class="mini-printer">
          <div class="mini-spool"></div>
          <div class="mini-gantry"><div class="mini-head"></div></div>
          <div class="mini-model"></div>
          <div class="mini-bed"></div>
        </div>
      </div>

      <div class="nav-label">Ferramentas</div>
      <nav class="tabs" aria-label="Navegação">
        <button class="tab-btn active" data-tab="producao" data-title="Custo de impressão" data-kicker="Produção 3D">
          <span class="tab-icon">
            <svg viewBox="0 0 24 24" fill="none">
              <path d="M5 3h14v14H5V3Zm3 14v4m8-4v4M8 21h8M8 7h8M9 10h6v4H9v-4Z" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"/>
            </svg>
          </span>
          <span class="tab-copy"><strong>Custo de impressão</strong><small>Produção e máquina</small></span>
        </button>

        <button class="tab-btn" data-tab="shopee" data-title="Venda na Shopee" data-kicker="Preço e rentabilidade">
          <span class="tab-icon">
            <svg viewBox="0 0 24 24" fill="none">
              <path d="M4 9h16l-1.2 11H5.2L4 9Zm4 0V7a4 4 0 0 1 8 0v2M8 13v1m8-1v1" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"/>
            </svg>
          </span>
          <span class="tab-copy"><strong>Venda na Shopee</strong><small>Taxas, ROAS e lucro</small></span>
        </button>

        <button class="tab-btn" data-tab="produtos" data-title="Produtos salvos" data-kicker="Biblioteca de custos">
          <span class="tab-icon">
            <svg viewBox="0 0 24 24" fill="none">
              <path d="m4 7 8-4 8 4-8 4-8-4Zm0 0v10l8 4 8-4V7M12 11v10" stroke="currentColor" stroke-width="1.6" stroke-linejoin="round"/>
            </svg>
          </span>
          <span class="tab-copy"><strong>Produtos salvos</strong><small>Pesquisar e reutilizar</small></span>
        </button>

        <button class="tab-btn" data-tab="sync" data-title="Sincronizar aparelhos" data-kicker="Transferência segura por QR">
          <span class="tab-icon">
            <svg viewBox="0 0 24 24" fill="none">
              <path d="M8 3H5a2 2 0 0 0-2 2v3m13-5h3a2 2 0 0 1 2 2v3M8 21H5a2 2 0 0 1-2-2v-3m13 5h3a2 2 0 0 0 2-2v-3M8 8h3v3H8V8Zm5 0h3v3h-3V8Zm-5 5h3v3H8v-3Zm5 0h1m2 0v3h-3v-1" stroke="currentColor" stroke-width="1.6" stroke-linecap="round" stroke-linejoin="round"/>
            </svg>
          </span>
          <span class="tab-copy"><strong>Sincronizar</strong><small>QR, câmera e importação</small></span>
        </button>
      </nav>

      <div class="sidebar-footer">
        <div class="machine-line"><span>Perfil ativo</span><strong>K2 Plus</strong></div>
        <span class="machine-chip">● Dados locais protegidos</span>
      </div>
    </aside>

    <section class="app-workspace">
      <header class="app-header">
        <div>
          <span class="page-kicker" id="pageKicker">Produção 3D</span>
          <h1 class="page-title" id="pageTitle">Custo de impressão</h1>
        </div>
        <div class="header-actions"><a class="desktop-version-link" href="./index.html?desktop=1">Desktop</a>
          <div class="save-status" id="saveStatus">Dados salvos neste computador</div>
          <button class="install-app-btn" id="installAppBtn" type="button">
            Instalar
          </button>
        </div>
      </header>

      <main class="app-content">
    <section class="tab-panel active" id="producao">
      <div class="layout">
        <div class="stack">
          <article class="card">
            <div class="card-inner">
              <div class="card-title">
                <h2>Dados da produção</h2>
                <span class="badge">Cálculo automático</span>
              </div>

              <div class="grid">
                <div class="field">
                  <label for="filamentGrams">Filamento utilizado</label>
                  <div class="input-wrap"><input id="filamentGrams" type="number" min="0" step="0.1" value="100"><span class="suffix">g</span></div>
                </div>

                <div class="field">
                  <label for="batchQty">Quantidade produzida</label>
                  <div class="input-wrap"><input id="batchQty" type="number" min="1" step="1" value="1"><span class="suffix">un.</span></div>
                  <span class="hint">Quantidade de peças feitas nessa impressão.</span>
                </div>

                <div class="field">
                  <label for="printHours">Tempo de impressão</label>
                  <div class="input-wrap"><input id="printHours" type="number" min="0" step="1" value="5"><span class="suffix">h</span></div>
                </div>

                <div class="field">
                  <label for="printMinutes">Minutos adicionais</label>
                  <div class="input-wrap"><input id="printMinutes" type="number" min="0" max="59" step="1" value="0"><span class="suffix">min</span></div>
                </div>

                <div class="field full">
                  <label for="extraProduction">Valor adicional de consumíveis</label>
                  <div class="input-wrap"><span class="prefix">R$</span><input id="extraProduction" type="number" min="0" step="0.01" value="0"></div>
                  <span class="hint">Argola, ímã, cola, adesivo, MDF, embalagem interna, mão de obra ou acabamento.</span>
                </div>
              </div>

              <details>
                <summary>⚙️ Custos avançados e dados da máquina</summary>
                <div class="advanced">
                  <div class="grid">
                    <div class="machine-profile">
                      <div>
                        <strong>🖨️ Perfil: Creality K2 Plus</strong>
                        <small>Os valores abaixo ficam armazenados automaticamente neste navegador e serão reutilizados nos próximos cálculos.</small>
                      </div>
                      <span class="profile-tag">SALVAMENTO AUTOMÁTICO</span>
                    </div>

                    <div class="field">
                      <label for="filamentKg">Valor do kg do filamento</label>
                      <div class="input-wrap"><span class="prefix">R$</span><input id="filamentKg" type="number" min="0" step="0.01" value="85"></div>
                    </div>

                    <div class="field">
                      <label for="printerValue">Valor da Creality K2 Plus</label>
                      <div class="input-wrap"><span class="prefix">R$</span><input id="printerValue" type="number" min="0" step="0.01" value="10000"></div>
                      <span class="hint">Coloque o valor real pago pela máquina.</span>
                    </div>

                    <div class="field">
                      <label for="printerLife">Vida útil estimada</label>
                      <div class="input-wrap"><input id="printerLife" type="number" min="1" step="1" value="10000"><span class="suffix">horas</span></div>
                      <span class="hint">Usada para calcular a depreciação por hora.</span>
                    </div>

                    <div class="field">
                      <label for="powerW">Consumo médio durante a impressão</label>
                      <div class="input-wrap"><input id="powerW" type="number" min="0" step="1" value="500"><span class="suffix">W</span></div>
                    </div>

                    <div class="field">
                      <label for="energyRate">Valor da energia elétrica</label>
                      <div class="input-wrap"><span class="prefix">R$</span><input id="energyRate" type="number" min="0" step="0.01" value="0.95"><span class="suffix">/kWh</span></div>
                    </div>

                    <div class="field">
                      <label for="maintenancePct">Reserva para manutenção</label>
                      <div class="input-wrap"><input id="maintenancePct" type="number" min="0" step="0.1" value="10"><span class="suffix">%</span></div>
                      <span class="hint">Percentual aplicado sobre a depreciação da máquina.</span>
                    </div>

                    <div class="field">
                      <label for="lossPct">Margem para perdas e falhas</label>
                      <div class="input-wrap"><input id="lossPct" type="number" min="0" step="0.1" value="5"><span class="suffix">%</span></div>
                    </div>
                  </div>

                  <div class="actions">
                    <button class="btn" id="saveAdvanced" type="button">Salvar custos fixos</button>
                    <button class="btn danger" id="resetAdvanced" type="button">Restaurar perfil K2 Plus</button>
                  </div>
                </div>
              </details>

              <div class="actions">
                <button class="btn primary" id="sendToShopee">Usar custo na Shopee →</button>
                <button class="btn" id="saveProduct">💾 Salvar produto</button>
                <button class="btn" id="copyProduction">Copiar resumo</button>
                <button class="btn danger" id="resetProduction">Limpar cálculo</button>
              </div>
            </div>
          </article>

        </div>

        <aside class="card result-card">
          <div class="result-top">
            <div class="result-label">Custo por unidade</div>
            <div class="big-value" id="unitCost">R$ 0,00</div>
            <div class="sub-value" id="batchCostText">Custo total do lote: R$ 0,00</div>
          </div>
          <div class="breakdown">
            <div class="row"><span>Filamento</span><strong id="rFilament">R$ 0,00</strong></div>
            <div class="row"><span>Depreciação da máquina</span><strong id="rMachine">R$ 0,00</strong></div>
            <div class="row"><span>Consumo estimado</span><strong id="rEnergyKwh">0,00 kWh</strong></div>
            <div class="row"><span>Custo da energia elétrica</span><strong id="rEnergy">R$ 0,00</strong></div>
            <div class="row"><span>Reserva de manutenção</span><strong id="rMaintenance">R$ 0,00</strong></div>
            <div class="row"><span>Acabamento e consumíveis</span><strong id="rExtras">R$ 0,00</strong></div>
            <div class="row"><span>Margem de perdas</span><strong id="rLoss">R$ 0,00</strong></div>
            <div class="row total"><span>Total do lote</span><strong id="rBatch">R$ 0,00</strong></div>
          </div>
        </aside>
      </div>
    </section>

    <section class="tab-panel" id="shopee">
      <div class="layout">
        <div class="stack">
          <article class="card">
            <div class="card-inner">
              <div class="card-title">
                <h2>Venda na Shopee</h2>
                <span class="badge">Taxas editáveis</span>
              </div>

              <div class="grid">
                <div class="field">
                  <label for="salePrice">Preço de venda</label>
                  <div class="input-wrap"><span class="prefix">R$</span><input id="salePrice" type="number" min="0" step="0.01" value="39.90"></div>
                </div>

                <div class="field">
                  <label for="productionCost">Custo do produto</label>
                  <div class="input-wrap"><span class="prefix">R$</span><input id="productionCost" type="number" min="0" step="0.01" value="0"></div>
                </div>

                <div class="field">
                  <label for="packagingCost">Embalagem</label>
                  <div class="input-wrap"><span class="prefix">R$</span><input id="packagingCost" type="number" min="0" step="0.01" value="1"></div>
                </div>

                <div class="field">
                  <label for="otherSaleCosts">Outros custos por venda</label>
                  <div class="input-wrap"><span class="prefix">R$</span><input id="otherSaleCosts" type="number" min="0" step="0.01" value="0"></div>
                </div>

                <div class="field">
                  <label for="shopeeFeePct">Taxa percentual Shopee</label>
                  <div class="input-wrap"><input id="shopeeFeePct" type="number" min="0" max="100" step="0.1" value="22.5"><span class="suffix">%</span></div>
                </div>

                <div class="field">
                  <label for="campaignFeePct">Taxa extra de campanha</label>
                  <div class="input-wrap"><input id="campaignFeePct" type="number" min="0" max="100" step="0.1" value="2.5"><span class="suffix">%</span></div>
                </div>

                <div class="field">
                  <label for="fixedFee">Taxa fixa por item/pedido</label>
                  <div class="input-wrap"><span class="prefix">R$</span><input id="fixedFee" type="number" min="0" step="0.01" value="4"></div>
                </div>

                <div class="field">
                  <label for="taxPct">Impostos adicionais</label>
                  <div class="input-wrap"><input id="taxPct" type="number" min="0" max="100" step="0.1" value="0"><span class="suffix">%</span></div>
                </div>

                <div class="field full roas-control">
                  <div class="roas-title-line">
                    <label for="adsValue">ROAS desejado no GMV Max</label>
                    <span class="shopee-style-chip">MESMA LÓGICA DA SHOPEE</span>
                  </div>

                  <div class="roas-layout">
                    <div class="input-wrap roas-input-wrap">
                      <span class="prefix">ROAS</span>
                      <input id="adsValue" type="number" min="0.1" step="0.1" value="6" inputmode="decimal">
                      <span class="suffix">x</span>
                    </div>

                    <div class="roas-metrics">
                      <div class="roas-metric">
                        <span>ADS nesta venda</span>
                        <strong id="roasAdsPreview">R$ 0,00</strong>
                      </div>
                      <div class="roas-metric">
                        <span>Percentual equivalente</span>
                        <strong id="roasEquivalentPct">0,00%</strong>
                      </div>
                    </div>
                  </div>

                  <div class="roas-help" id="roasExample">
                    Informe o mesmo ROAS configurado na campanha da Shopee.
                  </div>
                </div>

                <div class="field full">
                  <label for="desiredProfit">Lucro desejado por unidade</label>
                  <div class="input-wrap"><span class="prefix">R$</span><input id="desiredProfit" type="number" min="0" step="0.01" value="10"></div>
                </div>
              </div>

              <div class="actions">
                <button class="btn primary" id="applySuggested">Aplicar preço recomendado</button>
                <button class="btn" id="copyShopee">Copiar resumo</button>
                <button class="btn danger" id="resetShopee">Limpar</button>
              </div>

              <div class="notice">
                As taxas variam conforme categoria, programa, campanha e regras da conta. Os campos são editáveis para você manter o cálculo atualizado.
              </div>
            </div>
          </article>
        </div>

        <aside class="card result-card">
          <div class="result-top">
            <div class="result-label">Lucro líquido por venda</div>
            <div class="big-value" id="profitValue">R$ 0,00</div>
            <div class="sub-value" id="marginText">Margem líquida: 0,00%</div>
            <div class="profit-meter"><span id="profitMeter"></span></div>
          </div>
          <div class="breakdown">
            <div class="row"><span>Taxas percentuais</span><strong id="rFeesPct">R$ 0,00</strong></div>
            <div class="row"><span>Taxa fixa</span><strong id="rFixedFee">R$ 0,00</strong></div>
            <div class="row"><span>ROAS configurado</span><strong id="rRoas">6,00x</strong></div>
            <div class="row"><span>ADS</span><strong id="rAds">R$ 0,00</strong></div>
            <div class="row"><span>Produto + embalagem + extras</span><strong id="rSaleCosts">R$ 0,00</strong></div>
            <div class="row"><span>Valor líquido após taxas</span><strong id="rNetRevenue">R$ 0,00</strong></div>
            <div class="row" id="profitRow"><span>Lucro líquido</span><strong id="rProfit">R$ 0,00</strong></div>
            <div class="row"><span>Markup sobre o custo</span><strong id="rMarkup">0,00x</strong></div>
            <div class="row total"><span>Preço recomendado</span><strong id="rSuggested">R$ 0,00</strong></div>
          </div>
        </aside>
      </div>
    </section>

    <section class="tab-panel" id="produtos">
      <article class="card">
        <div class="card-inner">
          <div class="card-title">
            <div>
              <h2>Produtos salvos</h2>
              <div class="hint">Pesquise pelo nome e use o custo unitário diretamente na calculadora da Shopee.</div>
            </div>
            <span class="badge" id="savedCount">0 produtos</span>
          </div>

          <div class="products-toolbar">
            <div class="field search-box">
              <label for="productSearch">Pesquisar produto</label>
              <div class="input-wrap">
                <span class="search-icon">🔎</span>
                <input id="productSearch" type="search" autocomplete="off" placeholder="Digite o nome do produto">
                <button class="clear-search" id="clearProductSearch" type="button" aria-label="Limpar pesquisa">✕</button>
              </div>
            </div>
            <div class="products-summary" id="productsSummary">Todos os produtos salvos</div>
          </div>

          <div class="saved-products" id="savedProductsList">
            <div class="saved-empty">Nenhum produto salvo ainda.</div>
          </div>
        </div>
      </article>
    </section>


    <section class="tab-panel" id="sync">
      <div class="sync-layout">
        <article class="card">
          <div class="card-inner">
            <div class="card-title">
              <div>
                <h2>Gerar código de sincronização</h2>
                <div class="hint">Mostre este QR na tela do computador e leia com a câmera do celular.</div>
              </div>
              <span class="badge">SEM CONTA</span>
            </div>

            <div class="sync-device-row">
              <div class="field">
                <label for="syncDeviceName">Nome deste aparelho</label>
                <div class="input-wrap">
                  <input id="syncDeviceName" type="text" maxlength="40" placeholder="Ex.: Computador da loja">
                </div>
              </div>
              <div class="sync-data-summary">
                <span><strong id="syncProductCount">0</strong> produtos</span>
                <span>Custos e configurações</span>
              </div>
            </div>

            <div class="sync-options">
              <label class="sync-check">
                <input type="checkbox" id="syncIncludeSettings" checked>
                <span>Custos e configurações</span>
              </label>
              <label class="sync-check">
                <input type="checkbox" id="syncIncludeProducts" checked>
                <span>Produtos salvos</span>
              </label>
            </div>

            <div class="actions">
              <button class="btn primary" id="generateSyncCode" type="button">Gerar QR atualizado</button>
              <button class="btn" id="copyFullSyncCode" type="button">Copiar código textual</button>
            </div>

            <div class="sync-qr-stage" id="syncQrStage">
              <div class="sync-qr-empty" id="syncQrEmpty">
                <span class="sync-qr-empty-icon">⌁</span>
                <strong>Nenhum código gerado</strong>
                <small>O QR inclui apenas os dados selecionados acima.</small>
              </div>

              <div class="sync-qr-active" id="syncQrActive" hidden>
                <div class="sync-qr-paper">
                  <div id="syncQrCode" class="sync-qr-code"></div>
                </div>

                <div class="sync-frame-info">
                  <strong id="syncFrameLabel">Parte 1 de 1</strong>
                  <span id="syncFrameHint">Mantenha a câmera apontada para o código.</span>
                </div>

                <div class="sync-frame-controls">
                  <button class="mini-btn" id="syncPrevFrame" type="button">← Anterior</button>
                  <button class="mini-btn" id="syncAutoFrames" type="button">Pausar rotação</button>
                  <button class="mini-btn" id="syncNextFrame" type="button">Próxima →</button>
                </div>
              </div>
            </div>

            <details class="sync-text-details">
              <summary>Código textual para copiar manualmente</summary>
              <div class="advanced">
                <textarea id="syncTextCode" class="sync-textarea" readonly placeholder="Gere um código para visualizar"></textarea>
              </div>
            </details>

            <div class="sync-note">
              O QR faz uma sincronização pontual. Para atualizar depois, gere e leia um novo código.
            </div>
          </div>
        </article>

        <article class="card">
          <div class="card-inner">
            <div class="card-title">
              <div>
                <h2>Ler código de outro aparelho</h2>
                <div class="hint">Use a câmera ou selecione uma imagem contendo o QR.</div>
              </div>
              <span class="badge">CÂMERA</span>
            </div>

            <div class="sync-reader-actions">
              <button class="btn primary" id="startSyncScanner" type="button">Abrir câmera</button>
              <button class="btn" id="stopSyncScanner" type="button" disabled>Parar câmera</button>
              <label class="btn sync-file-button" for="syncQrFile">Ler imagem</label>
              <input id="syncQrFile" type="file" accept="image/*" hidden>
            </div>

            <div class="sync-scanner-shell">
              <div id="syncScanner" class="sync-scanner">
                <video id="syncCameraVideo" autoplay muted playsinline></video>
                <canvas id="syncCameraCanvas" hidden></canvas>
                <div id="syncScannerFallback" class="sync-scanner-fallback"></div>
                <div class="sync-camera-guide" id="syncCameraGuide" hidden>
                  <span></span><span></span><span></span><span></span>
                </div>
              </div>
              <div class="sync-scanner-placeholder" id="syncScannerPlaceholder">
                <span>▦</span>
                <strong>Câmera desativada</strong>
                <small>O navegador solicitará permissão quando você abrir a câmera.</small>
              </div>
            </div>

            <div class="sync-camera-diagnostic" id="syncCameraDiagnostic">
              Toque em “Abrir câmera” e autorize o acesso quando o navegador solicitar.
            </div>

            <div class="sync-progress-card">
              <div class="sync-progress-head">
                <span>Leitura do código</span>
                <strong id="syncScanProgressText">0 de 0 partes</strong>
              </div>
              <div class="sync-progress-track"><span id="syncScanProgressBar"></span></div>
              <div class="sync-scan-message" id="syncScanMessage">Aguardando leitura.</div>
            </div>

            <details class="sync-text-details">
              <summary>Colar código textual</summary>
              <div class="advanced">
                <textarea id="syncPasteCode" class="sync-textarea" placeholder="Cole aqui o código copiado do outro aparelho"></textarea>
                <div class="actions">
                  <button class="btn primary" id="readPastedSyncCode" type="button">Verificar código</button>
                  <button class="btn" id="clearSyncReader" type="button">Limpar leitura</button>
                </div>
              </div>
            </details>

            <div class="sync-import-preview" id="syncImportPreview" hidden>
              <div class="sync-import-icon">✓</div>
              <div class="sync-import-copy">
                <strong id="syncImportTitle">Código pronto para importar</strong>
                <span id="syncImportDetails"></span>
              </div>
              <button class="btn primary" id="confirmSyncImport" type="button">Importar e mesclar</button>
            </div>
          </div>
        </article>
      </div>

      <article class="card sync-status-card">
        <div class="card-inner">
          <div class="sync-status-grid">
            <div>
              <span>Última sincronização</span>
              <strong id="lastSyncDate">Ainda não realizada</strong>
            </div>
            <div>
              <span>Origem</span>
              <strong id="lastSyncSource">—</strong>
            </div>
            <div>
              <span>Modo</span>
              <strong>QR local, sem nuvem</strong>
            </div>
          </div>
        </div>
      </article>
    </section>

      </main>
    </section>
  </div>

  <div class="modal-backdrop" id="productModal" role="dialog" aria-modal="true" aria-labelledby="productModalTitle">
    <div class="modal">
      <div class="modal-header">
        <h3 id="productModalTitle">Salvar produto</h3>
        <p>Informe um nome para identificar este custo depois.</p>
      </div>
      <div class="modal-body">
        <div class="field">
          <label for="productName">Nome do produto</label>
          <div class="input-wrap">
            <input id="productName" type="text" maxlength="80" placeholder="Ex.: Chaveiro Pato da Vida">
          </div>
        </div>
        <div class="modal-cost">
          <span>Valor unitário calculado</span>
          <strong id="modalUnitCost">R$ 0,00</strong>
        </div>
        <div class="modal-actions">
          <button class="btn" id="cancelSaveProduct" type="button">Cancelar</button>
          <button class="btn primary" id="confirmSaveProduct" type="button">Salvar produto</button>
        </div>
      </div>
    </div>
  </div>

  <div class="toast" id="toast">Copiado</div>

  <script src="https://cdn.jsdelivr.net/gh/davidshimjs/qrcodejs/qrcode.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/lz-string@1.5.0/libs/lz-string.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/html5-qrcode@2.3.8/html5-qrcode.min.js"></script>

  <script>
    const $ = (id) => document.getElementById(id);
    const money = new Intl.NumberFormat('pt-BR',{style:'currency',currency:'BRL'});
    const numberBR = new Intl.NumberFormat('pt-BR',{minimumFractionDigits:2,maximumFractionDigits:2});
    const storageKey = 'calc3dShopee_app_v4';
    const productsStorageKey = 'calc3dShopee_products_v1';
    let adsMode = 'roas';
    let saveTimer;
    let savedProducts = [];
    let deferredInstallPrompt = null;
    const syncDeviceNameKey = 'jb3d_sync_device_name';
    const lastSyncKey = 'jb3d_last_sync';
    const syncPrefix = 'JB3DQR1';
    const syncTextPrefix = 'JB3DTEXT1|';
    const syncChunkSize = 480;
    let syncFrames = [];
    let syncFrameIndex = 0;
    let syncFrameTimer = null;
    let syncScanner = null;
    let syncNativeStream = null;
    let syncNativeDetector = null;
    let syncNativeScanTimer = null;
    let syncLastDecodedText = '';
    let syncLastDecodedAt = 0;
    let syncScannerMode = null;
    let syncCollected = {session:null,total:0,parts:new Map()};
    let pendingSyncPayload = null;

    const productionIds = [
      'filamentKg','filamentGrams','printerValue','printerLife','printHours','printMinutes',
      'batchQty','extraProduction','powerW','energyRate','maintenancePct','lossPct'
    ];
    const shopeeIds = [
      'salePrice','productionCost','packagingCost','otherSaleCosts','shopeeFeePct',
      'campaignFeePct','fixedFee','taxPct','adsValue','desiredProfit'
    ];
    const allIds = [...productionIds,...shopeeIds];

    function num(id){
      const value = parseFloat($(id).value);
      return Number.isFinite(value) ? value : 0;
    }

    function setText(id,value){ $(id).textContent = value; }

    function animateValue(id){
      const el = $(id);
      el.classList.remove('bump');
      requestAnimationFrame(() => {
        el.classList.add('bump');
        setTimeout(() => el.classList.remove('bump'),180);
      });
    }

    function calculateProduction(){
      const kgPrice = num('filamentKg');
      const grams = num('filamentGrams');
      const printer = num('printerValue');
      const life = Math.max(1,num('printerLife'));
      const hours = num('printHours') + num('printMinutes') / 60;
      const qty = Math.max(1,num('batchQty'));
      const extras = num('extraProduction');
      const power = num('powerW');
      const energyRate = num('energyRate');
      const maintenancePct = num('maintenancePct');
      const lossPct = num('lossPct');

      const filament = kgPrice * (grams / 1000);
      const machine = (printer / life) * hours;
      const energyKwh = (power / 1000) * hours;
      const energy = energyKwh * energyRate;
      const maintenance = machine * (maintenancePct / 100);
      const base = filament + machine + energy + maintenance + extras;
      const loss = base * (lossPct / 100);
      const batch = base + loss;
      const unit = batch / qty;

      setText('rFilament',money.format(filament));
      setText('rMachine',money.format(machine));
      setText('rEnergyKwh',`${numberBR.format(energyKwh)} kWh`);
      setText('rEnergy',money.format(energy));
      setText('rMaintenance',money.format(maintenance));
      setText('rExtras',money.format(extras));
      setText('rLoss',money.format(loss));
      setText('rBatch',money.format(batch));
      setText('unitCost',money.format(unit));
      setText('batchCostText',`Custo total do lote: ${money.format(batch)} • ${qty} unidade(s)`);
      animateValue('unitCost');

      return {filament,machine,energyKwh,energy,maintenance,extras,loss,batch,unit,qty,hours};
    }

    function calculateShopee(){
      const sale = num('salePrice');
      const production = num('productionCost');
      const packaging = num('packagingCost');
      const other = num('otherSaleCosts');
      const feePct = num('shopeeFeePct');
      const campaignPct = num('campaignFeePct');
      const taxPct = num('taxPct');
      const fixed = num('fixedFee');
      const roas = num('adsValue');
      const desired = num('desiredProfit');

      const totalPct = feePct + campaignPct + taxPct;
      const pctFees = sale * (totalPct / 100);

      // Mesma lógica exibida pela Shopee:
      // ROAS = faturamento atribuído / investimento em anúncios.
      const ads = roas > 0 ? sale / roas : 0;
      const equivalentAdsPct = roas > 0 ? 100 / roas : 0;

      const costs = production + packaging + other;
      const netRevenue = sale - pctFees - fixed - ads;
      const profit = netRevenue - costs;
      const margin = sale > 0 ? (profit / sale) * 100 : 0;
      const markup = costs > 0 ? sale / costs : 0;

      // Preço necessário para pagar taxas, ADS no ROAS escolhido,
      // custos e ainda atingir o lucro desejado.
      const divisor = 1 - (totalPct / 100) - (roas > 0 ? 1 / roas : 0);
      const suggested = divisor > 0
        ? (costs + fixed + desired) / divisor
        : 0;

      setText('rFeesPct',money.format(pctFees));
      setText('rFixedFee',money.format(fixed));
      setText('rRoas',roas > 0 ? `${numberBR.format(roas)}x` : 'Inválido');
      setText('rAds',money.format(ads));
      setText('rSaleCosts',money.format(costs));
      setText('rNetRevenue',money.format(netRevenue));
      setText('rProfit',money.format(profit));
      setText('rMarkup',`${numberBR.format(markup)}x`);
      setText('rSuggested',money.format(suggested));
      setText('profitValue',money.format(profit));
      setText('marginText',`Margem líquida: ${numberBR.format(margin)}%`);

      setText('roasAdsPreview',money.format(ads));
      setText('roasEquivalentPct',`${numberBR.format(equivalentAdsPct)}%`);
      setText(
        'roasExample',
        roas > 0
          ? `Exemplo: vendendo ${money.format(sale)}, um ROAS ${numberBR.format(roas)} representa aproximadamente ${money.format(ads)} investidos em ADS.`
          : 'O ROAS deve ser maior que zero.'
      );

      $('profitRow').classList.toggle('positive',profit >= 0);
      $('profitRow').classList.toggle('negative',profit < 0);
      $('profitValue').style.color = profit >= 0 ? 'var(--green)' : 'var(--red)';
      $('profitMeter').style.width = `${Math.max(0,Math.min(100,margin * 2))}%`;
      animateValue('profitValue');

      return {
        sale,production,packaging,other,totalPct,pctFees,fixed,
        roas,ads,equivalentAdsPct,costs,netRevenue,profit,margin,
        markup,suggested,desired
      };
    }

    function save(){
      const data = {adsMode:'roas'};
      allIds.forEach(id => data[id] = $(id).value);
      localStorage.setItem(storageKey,JSON.stringify(data));
      $('saveStatus').textContent = 'Salvo agora';
      clearTimeout(saveTimer);
      saveTimer = setTimeout(() => $('saveStatus').textContent = 'Dados salvos automaticamente',1200);
    }

    function load(){
      try{
        const data = JSON.parse(localStorage.getItem(storageKey) || '{}');
        allIds.forEach(id => {
          if(data[id] !== undefined) $(id).value = data[id];
        });
        adsMode = 'roas';
      }catch(e){}
    }

    function loadSavedProducts(){
      try{
        const parsed = JSON.parse(localStorage.getItem(productsStorageKey) || '[]');
        savedProducts = Array.isArray(parsed) ? parsed : [];
      }catch(e){
        savedProducts = [];
      }
      renderSavedProducts();
    }

    function persistSavedProducts(){
      localStorage.setItem(productsStorageKey,JSON.stringify(savedProducts));
      renderSavedProducts();
    }

    function formatSavedDate(value){
      try{
        return new Intl.DateTimeFormat('pt-BR',{
          day:'2-digit',month:'2-digit',year:'numeric',
          hour:'2-digit',minute:'2-digit'
        }).format(new Date(value));
      }catch(e){
        return '';
      }
    }

    function normalizeSearchText(value){
      return String(value || '')
        .normalize('NFD')
        .replace(/[\u0300-\u036f]/g,'')
        .toLocaleLowerCase('pt-BR')
        .trim();
    }

    function renderSavedProducts(){
      const list = $('savedProductsList');
      const searchInput = $('productSearch');
      const query = normalizeSearchText(searchInput ? searchInput.value : '');
      const total = savedProducts.length;

      const filteredProducts = [...savedProducts]
        .filter(product => normalizeSearchText(product.name).includes(query))
        .sort((a,b) => new Date(b.updatedAt || b.createdAt) - new Date(a.updatedAt || a.createdAt));

      list.innerHTML = '';
      $('savedCount').textContent = `${total} ${total === 1 ? 'produto' : 'produtos'}`;
      if($('syncProductCount')) updateSyncSummary();

      if($('productsSummary')){
        $('productsSummary').textContent = query
          ? `${filteredProducts.length} de ${total} encontrado(s)`
          : total
            ? `${total} produto(s) armazenado(s)`
            : 'Nenhum produto armazenado';
      }

      if($('clearProductSearch')){
        $('clearProductSearch').classList.toggle('show',Boolean(query));
      }

      if(!total){
        const empty = document.createElement('div');
        empty.className = 'saved-empty';
        empty.textContent = 'Nenhum produto salvo ainda.';
        list.appendChild(empty);
        return;
      }

      if(!filteredProducts.length){
        const empty = document.createElement('div');
        empty.className = 'saved-empty';
        empty.textContent = 'Nenhum produto encontrado com esse nome.';
        list.appendChild(empty);
        return;
      }

      filteredProducts.forEach(product => {
        const item = document.createElement('div');
        item.className = 'product-item';

        const info = document.createElement('div');

        const name = document.createElement('div');
        name.className = 'product-name';
        name.textContent = product.name;

        const meta = document.createElement('div');
        meta.className = 'product-meta';
        meta.textContent = `Salvo em ${formatSavedDate(product.updatedAt || product.createdAt)}`;

        const value = document.createElement('div');
        value.className = 'product-value';
        value.textContent = `${money.format(product.unitCost)} por unidade`;

        info.append(name,meta,value);

        const actions = document.createElement('div');
        actions.className = 'product-actions';

        const useBtn = document.createElement('button');
        useBtn.className = 'mini-btn';
        useBtn.type = 'button';
        useBtn.textContent = 'Usar na Shopee';
        useBtn.addEventListener('click',() => {
          $('productionCost').value = Number(product.unitCost || 0).toFixed(2);
          calculateShopee();
          save();
          showTab('shopee');
          toast(`${product.name} carregado`);
        });

        const deleteBtn = document.createElement('button');
        deleteBtn.className = 'mini-btn delete';
        deleteBtn.type = 'button';
        deleteBtn.textContent = 'Excluir';
        deleteBtn.addEventListener('click',() => {
          if(!confirm(`Excluir o produto "${product.name}"?`)) return;
          savedProducts = savedProducts.filter(item => item.id !== product.id);
          persistSavedProducts();
          toast('Produto excluído');
        });

        actions.append(useBtn,deleteBtn);
        item.append(info,actions);
        list.appendChild(item);
      });
    }

    function openProductModal(){
      const result = calculateProduction();
      if(result.unit <= 0){
        toast('Preencha os dados da impressão primeiro');
        return;
      }
      $('modalUnitCost').textContent = money.format(result.unit);
      $('productName').value = '';
      $('productModal').classList.add('show');
      setTimeout(() => $('productName').focus(),60);
    }

    function closeProductModal(){
      $('productModal').classList.remove('show');
    }

    function saveCurrentProduct(){
      const name = $('productName').value.trim();
      if(!name){
        $('productName').focus();
        toast('Digite o nome do produto');
        return;
      }

      const result = calculateProduction();
      const now = new Date().toISOString();
      const existing = savedProducts.find(item => item.name.toLocaleLowerCase('pt-BR') === name.toLocaleLowerCase('pt-BR'));

      const productData = {
        id: existing?.id || `${Date.now()}_${Math.random().toString(16).slice(2)}`,
        name,
        unitCost:Number(result.unit.toFixed(4)),
        batchCost:Number(result.batch.toFixed(4)),
        quantity:result.qty,
        filamentGrams:num('filamentGrams'),
        printHours:num('printHours'),
        printMinutes:num('printMinutes'),
        extraProduction:num('extraProduction'),
        createdAt:existing?.createdAt || now,
        updatedAt:now
      };

      if(existing){
        savedProducts = savedProducts.map(item => item.id === existing.id ? productData : item);
      }else{
        savedProducts.push(productData);
      }

      persistSavedProducts();
      closeProductModal();
      toast(existing ? 'Produto atualizado' : 'Produto salvo');
    }

    function isAppInstalled(){
      return window.matchMedia('(display-mode: standalone)').matches ||
             window.navigator.standalone === true;
    }

    function updateInstallButton(){
      const button = $('installAppBtn');
      if(!button) return;
      if(isAppInstalled()){
        button.classList.remove('show');
        button.classList.add('installed');
        return;
      }
      button.classList.toggle('show',Boolean(deferredInstallPrompt));
    }

    async function installApp(){
      if(!deferredInstallPrompt){
        toast('Use o menu do navegador e escolha “Instalar aplicativo”');
        return;
      }
      deferredInstallPrompt.prompt();
      const choice = await deferredInstallPrompt.userChoice;
      deferredInstallPrompt = null;
      updateInstallButton();
      if(choice.outcome === 'accepted') toast('Aplicativo instalado');
    }

    function registerPWA(){
      if('serviceWorker' in navigator){
        window.addEventListener('load',() => {
          navigator.serviceWorker.register('./sw.js').then(registration => {
            registration.update?.();
          }).catch(() => {});
        });
      }

      window.addEventListener('beforeinstallprompt',(event) => {
        event.preventDefault();
        deferredInstallPrompt = event;
        updateInstallButton();
      });

      window.addEventListener('appinstalled',() => {
        deferredInstallPrompt = null;
        updateInstallButton();
        toast('Aplicativo instalado');
      });

      window.matchMedia('(display-mode: standalone)').addEventListener?.('change',updateInstallButton);
    }


    function safeJsonParse(value,fallback){
      try{
        const parsed = JSON.parse(value);
        return parsed ?? fallback;
      }catch(e){
        return fallback;
      }
    }

    function defaultSyncDeviceName(){
      const isMobile = window.matchMedia('(pointer:coarse)').matches;
      return isMobile ? 'Celular JB3D' : 'Computador JB3D';
    }

    function loadSyncDevice(){
      const saved = localStorage.getItem(syncDeviceNameKey);
      $('syncDeviceName').value = saved || defaultSyncDeviceName();
      $('syncDeviceName').addEventListener('input',() => {
        localStorage.setItem(syncDeviceNameKey,$('syncDeviceName').value.trim());
      });
      updateSyncSummary();
      updateLastSyncCard();
    }

    function updateSyncSummary(){
      setText('syncProductCount',String(savedProducts.length));
    }

    function updateLastSyncCard(){
      const last = safeJsonParse(localStorage.getItem(lastSyncKey),'');
      if(!last || !last.date){
        setText('lastSyncDate','Ainda não realizada');
        setText('lastSyncSource','—');
        return;
      }
      setText('lastSyncDate',formatSavedDate(last.date));
      setText('lastSyncSource',last.source || 'Outro aparelho');
    }

    function collectSyncPayload(){
      const includeSettings = $('syncIncludeSettings').checked;
      const includeProducts = $('syncIncludeProducts').checked;
      return {
        schema:1,
        app:'JB3D Cost Studio',
        createdAt:new Date().toISOString(),
        deviceName:$('syncDeviceName').value.trim() || defaultSyncDeviceName(),
        settings:includeSettings
          ? safeJsonParse(localStorage.getItem(storageKey),'')
          : null,
        products:includeProducts
          ? safeJsonParse(localStorage.getItem(productsStorageKey),'')
          : null
      };
    }

    function encodeSyncPayload(payload){
      if(typeof LZString === 'undefined'){
        throw new Error('Módulo de compactação não carregado. Verifique a internet e recarregue.');
      }
      const json = JSON.stringify(payload);
      return LZString.compressToEncodedURIComponent(json);
    }

    function decodeSyncPayload(compressed){
      if(typeof LZString === 'undefined'){
        throw new Error('Módulo de compactação não carregado.');
      }
      const json = LZString.decompressFromEncodedURIComponent(compressed);
      if(!json) throw new Error('Código incompleto ou inválido.');
      const payload = JSON.parse(json);
      if(!payload || payload.schema !== 1 || payload.app !== 'JB3D Cost Studio'){
        throw new Error('Este código não pertence ao JB3D Cost Studio.');
      }
      return payload;
    }

    function makeSyncFrames(compressed){
      const session = `${Date.now().toString(36)}${Math.random().toString(36).slice(2,6)}`;
      const chunks = [];
      for(let i=0;i<compressed.length;i+=syncChunkSize){
        chunks.push(compressed.slice(i,i+syncChunkSize));
      }
      return chunks.map((chunk,index) =>
        `${syncPrefix}|${session}|${index+1}|${chunks.length}|${chunk}`
      );
    }

    function stopSyncFrameRotation(){
      if(syncFrameTimer){
        clearInterval(syncFrameTimer);
        syncFrameTimer = null;
      }
      if($('syncAutoFrames')) setText('syncAutoFrames','Iniciar rotação');
    }

    function startSyncFrameRotation(){
      stopSyncFrameRotation();
      if(syncFrames.length <= 1){
        setText('syncAutoFrames','Código único');
        return;
      }
      setText('syncAutoFrames','Pausar rotação');
      syncFrameTimer = setInterval(() => {
        renderSyncFrame((syncFrameIndex+1)%syncFrames.length);
      },1600);
    }

    function renderSyncFrame(index){
      if(!syncFrames.length) return;
      syncFrameIndex = (index+syncFrames.length)%syncFrames.length;
      const target = $('syncQrCode');
      target.innerHTML = '';

      if(typeof QRCode === 'undefined'){
        $('syncQrActive').hidden = true;
        $('syncQrEmpty').hidden = false;
        $('syncQrEmpty').querySelector('strong').textContent = 'Gerador de QR não carregado';
        $('syncQrEmpty').querySelector('small').textContent = 'Conecte à internet e recarregue a página.';
        return;
      }

      new QRCode(target,{
        text:syncFrames[syncFrameIndex],
        width:280,
        height:280,
        colorDark:'#08111f',
        colorLight:'#ffffff',
        correctLevel:QRCode.CorrectLevel.L
      });

      setText('syncFrameLabel',`Parte ${syncFrameIndex+1} de ${syncFrames.length}`);
      setText(
        'syncFrameHint',
        syncFrames.length > 1
          ? 'As partes mudam automaticamente. Mantenha a câmera apontada.'
          : 'Mantenha a câmera apontada para o código.'
      );
    }

    function generateSyncCode(){
      try{
        if(!$('syncIncludeSettings').checked && !$('syncIncludeProducts').checked){
          toast('Selecione pelo menos um tipo de dado');
          return;
        }

        localStorage.setItem(syncDeviceNameKey,$('syncDeviceName').value.trim());
        const payload = collectSyncPayload();
        const compressed = encodeSyncPayload(payload);

        syncFrames = makeSyncFrames(compressed);
        syncFrameIndex = 0;
        $('syncTextCode').value = syncTextPrefix + compressed;
        $('syncQrEmpty').hidden = true;
        $('syncQrActive').hidden = false;

        renderSyncFrame(0);
        startSyncFrameRotation();
        toast(`${syncFrames.length} parte(s) pronta(s) para leitura`);
      }catch(error){
        toast(error.message || 'Não foi possível gerar o código');
      }
    }

    async function copyFullSyncCode(){
      if(!$('syncTextCode').value) generateSyncCode();
      const value = $('syncTextCode').value;
      if(!value) return;
      await copyText(value);
    }

    function resetCollectedSync(message='Aguardando leitura.'){
      syncCollected = {session:null,total:0,parts:new Map()};
      pendingSyncPayload = null;
      $('syncImportPreview').hidden = true;
      setText('syncScanProgressText','0 de 0 partes');
      $('syncScanProgressBar').style.width = '0%';
      setText('syncScanMessage',message);
    }

    function showSyncImportPreview(payload){
      pendingSyncPayload = payload;
      const products = Array.isArray(payload.products) ? payload.products.length : 0;
      const settingsText = payload.settings ? 'custos e configurações' : 'sem configurações';
      setText('syncImportTitle',`Dados de ${payload.deviceName || 'outro aparelho'}`);
      setText(
        'syncImportDetails',
        `${products} produto(s), ${settingsText}. Gerado em ${formatSavedDate(payload.createdAt)}.`
      );
      $('syncImportPreview').hidden = false;
      setText('syncScanMessage','Leitura concluída. Confirme a importação abaixo.');
    }

    function processFullSyncText(text){
      const clean = String(text || '').trim();
      if(!clean.startsWith(syncTextPrefix)){
        throw new Error('Código textual inválido.');
      }
      const payload = decodeSyncPayload(clean.slice(syncTextPrefix.length));
      showSyncImportPreview(payload);
    }

    function processSyncFrame(decodedText){
      const text = String(decodedText || '').trim();

      if(text.startsWith(syncTextPrefix)){
        processFullSyncText(text);
        stopSyncScanner();
        return;
      }

      if(!text.startsWith(syncPrefix+'|')) return;

      const first = text.indexOf('|');
      const second = text.indexOf('|',first+1);
      const third = text.indexOf('|',second+1);
      const fourth = text.indexOf('|',third+1);
      if([first,second,third,fourth].some(index => index < 0)) return;

      const session = text.slice(first+1,second);
      const index = Number(text.slice(second+1,third));
      const total = Number(text.slice(third+1,fourth));
      const chunk = text.slice(fourth+1);

      if(!session || !Number.isInteger(index) || !Number.isInteger(total) || index<1 || total<1 || index>total){
        return;
      }

      if(syncCollected.session !== session){
        syncCollected = {session,total,parts:new Map()};
      }

      if(!syncCollected.parts.has(index)){
        syncCollected.parts.set(index,chunk);
        navigator.vibrate?.(35);
      }

      const read = syncCollected.parts.size;
      const percentage = Math.round((read/total)*100);
      setText('syncScanProgressText',`${read} de ${total} partes`);
      $('syncScanProgressBar').style.width = `${percentage}%`;
      setText(
        'syncScanMessage',
        read < total
          ? `Parte ${index} recebida. Continue apontando a câmera.`
          : 'Todas as partes recebidas. Validando dados...'
      );

      if(read === total){
        try{
          let compressed = '';
          for(let i=1;i<=total;i++){
            const part = syncCollected.parts.get(i);
            if(!part) throw new Error('Falta uma parte do código.');
            compressed += part;
          }
          const payload = decodeSyncPayload(compressed);
          showSyncImportPreview(payload);
          stopSyncScanner();
        }catch(error){
          resetCollectedSync(error.message || 'Erro ao validar o código.');
        }
      }
    }

    function setCameraDiagnostic(message,type=''){
      const diagnostic = $('syncCameraDiagnostic');
      if(!diagnostic) return;
      diagnostic.textContent = message;
      diagnostic.classList.toggle('error',type === 'error');
      diagnostic.classList.toggle('success',type === 'success');
    }

    function cameraErrorMessage(error){
      const name = error?.name || '';
      const message = String(error?.message || '');

      if(!window.isSecureContext){
        return 'A câmera só funciona no endereço HTTPS do GitHub Pages. Não abra o arquivo HTML diretamente pelo gerenciador de arquivos.';
      }
      if(name === 'NotAllowedError' || name === 'PermissionDeniedError'){
        return 'A permissão da câmera foi bloqueada. No Chrome, toque no cadeado ao lado do endereço, abra Permissões e permita Câmera.';
      }
      if(name === 'NotFoundError' || name === 'DevicesNotFoundError'){
        return 'Nenhuma câmera foi encontrada neste aparelho.';
      }
      if(name === 'NotReadableError' || name === 'TrackStartError'){
        return 'A câmera está sendo usada por outro aplicativo. Feche a câmera, WhatsApp ou outro leitor e tente novamente.';
      }
      if(name === 'OverconstrainedError' || name === 'ConstraintNotSatisfiedError'){
        return 'A câmera traseira não aceitou a configuração solicitada. Tentando uma configuração compatível.';
      }
      if(name === 'SecurityError'){
        return 'O navegador bloqueou a câmera por segurança. Abra o site pelo HTTPS do GitHub Pages.';
      }
      if(message.toLowerCase().includes('permission')){
        return 'O navegador não autorizou a câmera. Revise a permissão do site.';
      }
      return `Não foi possível iniciar a câmera${message ? `: ${message}` : '.'}`;
    }

    async function requestNativeCamera(){
      if(!window.isSecureContext){
        throw new DOMException('Camera requires HTTPS','SecurityError');
      }
      if(!navigator.mediaDevices?.getUserMedia){
        throw new DOMException('getUserMedia unavailable','NotSupportedError');
      }

      const preferredConstraints = {
        audio:false,
        video:{
          facingMode:{ideal:'environment'},
          width:{ideal:1280},
          height:{ideal:720}
        }
      };

      try{
        return await navigator.mediaDevices.getUserMedia(preferredConstraints);
      }catch(error){
        if(
          error?.name === 'OverconstrainedError' ||
          error?.name === 'ConstraintNotSatisfiedError' ||
          error?.name === 'NotFoundError'
        ){
          return await navigator.mediaDevices.getUserMedia({
            audio:false,
            video:true
          });
        }
        throw error;
      }
    }

    async function createNativeQrDetector(){
      if(!('BarcodeDetector' in window)) return null;

      try{
        if(typeof BarcodeDetector.getSupportedFormats === 'function'){
          const formats = await BarcodeDetector.getSupportedFormats();
          if(Array.isArray(formats) && !formats.includes('qr_code')) return null;
        }
        return new BarcodeDetector({formats:['qr_code']});
      }catch(error){
        return null;
      }
    }

    async function nativeQrScanStep(){
      if(
        syncScannerMode !== 'native' ||
        !syncNativeDetector ||
        !syncNativeStream
      ) return;

      const video = $('syncCameraVideo');
      if(video.readyState >= 2 && !video.paused){
        try{
          const codes = await syncNativeDetector.detect(video);
          const decoded = codes?.[0]?.rawValue;
          const now = Date.now();

          if(
            decoded &&
            (decoded !== syncLastDecodedText || now-syncLastDecodedAt > 1800)
          ){
            syncLastDecodedText = decoded;
            syncLastDecodedAt = now;
            processSyncFrame(decoded);
          }
        }catch(error){}
      }

      syncNativeScanTimer = window.setTimeout(nativeQrScanStep,220);
    }

    async function startNativeScanner(){
      const stream = await requestNativeCamera();
      const video = $('syncCameraVideo');

      syncNativeStream = stream;
      syncScannerMode = 'native';
      video.srcObject = stream;
      video.classList.add('active');
      $('syncScannerFallback').classList.remove('active');
      $('syncCameraGuide').hidden = false;

      await video.play();

      syncNativeDetector = await createNativeQrDetector();
      if(!syncNativeDetector){
        throw new DOMException('Native QR detector unavailable','NotSupportedError');
      }

      setCameraDiagnostic('Câmera traseira aberta. Mantenha o QR dentro da moldura.','success');
      setText('syncScanMessage','Câmera pronta. Aponte para o QR do outro aparelho.');
      nativeQrScanStep();
    }

    async function chooseBestHtml5Camera(){
      const cameras = await Html5Qrcode.getCameras();
      if(!Array.isArray(cameras) || !cameras.length){
        throw new DOMException('No cameras found','NotFoundError');
      }

      const backPattern = /(back|rear|environment|traseira|principal|wide|camera 0)/i;
      const frontPattern = /(front|frontal|selfie|user)/i;

      return (
        cameras.find(camera => backPattern.test(camera.label) && !frontPattern.test(camera.label)) ||
        cameras.find(camera => !frontPattern.test(camera.label)) ||
        cameras[cameras.length-1]
      );
    }

    async function startHtml5Fallback(){
      if(typeof Html5Qrcode === 'undefined'){
        throw new DOMException('QR library unavailable','NotSupportedError');
      }

      syncScannerMode = 'html5';
      $('syncCameraVideo').classList.remove('active');
      $('syncScannerFallback').classList.add('active');
      $('syncCameraGuide').hidden = false;

      syncScanner = new Html5Qrcode('syncScannerFallback',{
        experimentalFeatures:{useBarCodeDetectorIfSupported:true},
        verbose:false
      });

      const selectedCamera = await chooseBestHtml5Camera();
      await syncScanner.start(
        selectedCamera.id,
        {
          fps:10,
          qrbox:(width,height) => {
            const size = Math.floor(Math.min(width,height)*0.72);
            return {width:size,height:size};
          }
        },
        processSyncFrame,
        () => {}
      );

      setCameraDiagnostic(
        `Câmera aberta: ${selectedCamera.label || 'câmera traseira'}. Mantenha o QR centralizado.`,
        'success'
      );
      setText('syncScanMessage','Câmera pronta. Aponte para o QR do outro aparelho.');
    }

    async function startSyncScanner(){
      await stopSyncScanner();
      resetCollectedSync('Solicitando acesso à câmera...');

      if(!window.isSecureContext){
        const message = cameraErrorMessage(new DOMException('','SecurityError'));
        setCameraDiagnostic(message,'error');
        setText('syncScanMessage',message);
        toast('Abra pelo HTTPS do GitHub Pages');
        return;
      }

      $('syncScannerPlaceholder').hidden = true;
      $('startSyncScanner').disabled = true;
      $('stopSyncScanner').disabled = false;
      setCameraDiagnostic('Solicitando permissão da câmera...');

      try{
        try{
          await startNativeScanner();
        }catch(nativeError){
          await stopNativeCameraOnly();
          setCameraDiagnostic('Abrindo leitor de compatibilidade...');
          await startHtml5Fallback();
        }
      }catch(error){
        await stopSyncScanner();
        const message = cameraErrorMessage(error);
        setCameraDiagnostic(message,'error');
        setText('syncScanMessage',message);
        toast('Não foi possível abrir a câmera');
      }
    }

    async function stopNativeCameraOnly(){
      if(syncNativeScanTimer){
        clearTimeout(syncNativeScanTimer);
        syncNativeScanTimer = null;
      }

      if(syncNativeStream){
        syncNativeStream.getTracks().forEach(track => track.stop());
        syncNativeStream = null;
      }

      syncNativeDetector = null;
      const video = $('syncCameraVideo');
      if(video){
        video.pause();
        video.srcObject = null;
        video.classList.remove('active');
      }
    }

    async function stopSyncScanner(){
      await stopNativeCameraOnly();

      if(syncScanner){
        try{ await syncScanner.stop(); }catch(e){}
        try{ await syncScanner.clear(); }catch(e){}
        syncScanner = null;
      }

      syncScannerMode = null;
      syncLastDecodedText = '';
      syncLastDecodedAt = 0;

      if($('syncScannerFallback')){
        $('syncScannerFallback').classList.remove('active');
        $('syncScannerFallback').innerHTML = '';
      }
      if($('syncCameraGuide')) $('syncCameraGuide').hidden = true;
      if($('syncScannerPlaceholder')) $('syncScannerPlaceholder').hidden = false;
      if($('startSyncScanner')) $('startSyncScanner').disabled = false;
      if($('stopSyncScanner')) $('stopSyncScanner').disabled = true;
    }

    async function scanSyncImage(file){
      if(!file) return;

      await stopSyncScanner();
      resetCollectedSync('Lendo imagem selecionada...');

      try{
        let decoded = '';

        if('BarcodeDetector' in window){
          const detector = await createNativeQrDetector();
          if(detector){
            const bitmap = await createImageBitmap(file);
            const codes = await detector.detect(bitmap);
            bitmap.close?.();
            decoded = codes?.[0]?.rawValue || '';
          }
        }

        if(!decoded && typeof Html5Qrcode !== 'undefined'){
          const fileScanner = new Html5Qrcode('syncScannerFallback');
          decoded = await fileScanner.scanFile(file,true);
          await fileScanner.clear();
        }

        if(!decoded) throw new Error('QR não encontrado');
        processSyncFrame(decoded);
      }catch(error){
        setText('syncScanMessage','Nenhum QR válido foi encontrado na imagem.');
        setCameraDiagnostic('A imagem não contém um QR legível.','error');
      }finally{
        $('syncQrFile').value = '';
      }
    }

    function mergeSyncedProducts(importedProducts){
      if(!Array.isArray(importedProducts)) return savedProducts;

      const result = [...savedProducts];
      importedProducts.forEach(imported => {
        if(!imported || !imported.name) return;
        const importedName = normalizeSearchText(imported.name);
        const existingIndex = result.findIndex(item =>
          (imported.id && item.id === imported.id) ||
          normalizeSearchText(item.name) === importedName
        );

        if(existingIndex < 0){
          result.push(imported);
          return;
        }

        const existing = result[existingIndex];
        const importedDate = new Date(imported.updatedAt || imported.createdAt || 0).getTime();
        const existingDate = new Date(existing.updatedAt || existing.createdAt || 0).getTime();
        if(importedDate >= existingDate) result[existingIndex] = imported;
      });

      return result;
    }

    function importPendingSync(){
      if(!pendingSyncPayload){
        toast('Nenhum código validado');
        return;
      }

      const payload = pendingSyncPayload;

      if(payload.settings && typeof payload.settings === 'object'){
        localStorage.setItem(storageKey,JSON.stringify(payload.settings));
      }

      if(Array.isArray(payload.products)){
        savedProducts = mergeSyncedProducts(payload.products);
        localStorage.setItem(productsStorageKey,JSON.stringify(savedProducts));
      }

      const lastSync = {
        date:new Date().toISOString(),
        source:payload.deviceName || 'Outro aparelho'
      };
      localStorage.setItem(lastSyncKey,JSON.stringify(lastSync));

      load();
      loadSavedProducts();
      calculateProduction();
      calculateShopee();
      updateSyncSummary();
      updateLastSyncCard();

      pendingSyncPayload = null;
      $('syncImportPreview').hidden = true;
      resetCollectedSync('Dados importados com sucesso.');
      toast('Aparelhos sincronizados');
    }

    function updateAll(){
      calculateProduction();
      calculateShopee();
      save();
    }

    function setAdsMode(mode,shouldSave=true){
      adsMode = 'roas';
      calculateShopee();
      if(shouldSave) save();
    }

    function showTab(tab){
      document.querySelectorAll('.tab-btn').forEach(btn => btn.classList.toggle('active',btn.dataset.tab === tab));
      document.querySelectorAll('.tab-panel').forEach(panel => panel.classList.toggle('active',panel.id === tab));

      const activeButton = document.querySelector(`.tab-btn[data-tab="${tab}"]`);
      if(activeButton){
        setText('pageTitle',activeButton.dataset.title || '');
        setText('pageKicker',activeButton.dataset.kicker || '');
      }

      const content = document.querySelector('.app-content');
      if(content) content.scrollTo({top:0,behavior:'smooth'});
      history.replaceState(null,'',`#${tab}`);
      if(tab !== 'sync') stopSyncScanner();
    }

    function toast(message){
      $('toast').textContent = message;
      $('toast').classList.add('show');
      setTimeout(() => $('toast').classList.remove('show'),1400);
    }

    async function copyText(text){
      try{
        await navigator.clipboard.writeText(text);
        toast('Resumo copiado');
      }catch(e){
        const ta = document.createElement('textarea');
        ta.value = text;
        document.body.appendChild(ta);
        ta.select();
        document.execCommand('copy');
        ta.remove();
        toast('Resumo copiado');
      }
    }

    document.querySelectorAll('.tab-btn').forEach(btn => btn.addEventListener('click',() => showTab(btn.dataset.tab)));
    allIds.forEach(id => $(id).addEventListener('input',updateAll));

    $('installAppBtn').addEventListener('click',installApp);

    $('generateSyncCode').addEventListener('click',generateSyncCode);
    $('copyFullSyncCode').addEventListener('click',copyFullSyncCode);
    $('syncPrevFrame').addEventListener('click',() => {
      renderSyncFrame(syncFrameIndex-1);
      if(syncFrameTimer) startSyncFrameRotation();
    });
    $('syncNextFrame').addEventListener('click',() => {
      renderSyncFrame(syncFrameIndex+1);
      if(syncFrameTimer) startSyncFrameRotation();
    });
    $('syncAutoFrames').addEventListener('click',() => {
      syncFrameTimer ? stopSyncFrameRotation() : startSyncFrameRotation();
    });
    $('startSyncScanner').addEventListener('click',startSyncScanner);
    $('stopSyncScanner').addEventListener('click',stopSyncScanner);
    $('syncQrFile').addEventListener('change',(event) => scanSyncImage(event.target.files?.[0]));
    $('readPastedSyncCode').addEventListener('click',() => {
      try{
        processFullSyncText($('syncPasteCode').value);
      }catch(error){
        toast(error.message || 'Código inválido');
      }
    });
    $('clearSyncReader').addEventListener('click',() => {
      $('syncPasteCode').value = '';
      resetCollectedSync();
    });
    $('confirmSyncImport').addEventListener('click',importPendingSync);

    $('productSearch').addEventListener('input',renderSavedProducts);
    $('clearProductSearch').addEventListener('click',() => {
      $('productSearch').value = '';
      renderSavedProducts();
      $('productSearch').focus();
    });

    $('saveProduct').addEventListener('click',openProductModal);
    $('cancelSaveProduct').addEventListener('click',closeProductModal);
    $('confirmSaveProduct').addEventListener('click',saveCurrentProduct);
    $('productName').addEventListener('keydown',(event) => {
      if(event.key === 'Enter') saveCurrentProduct();
      if(event.key === 'Escape') closeProductModal();
    });
    $('productModal').addEventListener('click',(event) => {
      if(event.target === $('productModal')) closeProductModal();
    });

    $('sendToShopee').addEventListener('click',() => {
      const result = calculateProduction();
      $('productionCost').value = result.unit.toFixed(2);
      calculateShopee();
      save();
      showTab('shopee');
      toast('Custo enviado para a Shopee');
    });

    $('applySuggested').addEventListener('click',() => {
      const result = calculateShopee();
      $('salePrice').value = result.suggested.toFixed(2);
      calculateShopee();
      save();
      toast('Preço recomendado aplicado');
    });

    $('copyProduction').addEventListener('click',() => {
      const r = calculateProduction();
      copyText(
`RESUMO DO CUSTO DE IMPRESSÃO
Filamento: ${money.format(r.filament)}
Depreciação da máquina: ${money.format(r.machine)}
Consumo de energia: ${numberBR.format(r.energyKwh)} kWh
Custo da energia: ${money.format(r.energy)}
Manutenção: ${money.format(r.maintenance)}
Acabamento e consumíveis: ${money.format(r.extras)}
Perdas: ${money.format(r.loss)}
Total do lote: ${money.format(r.batch)}
Quantidade: ${r.qty}
Custo por unidade: ${money.format(r.unit)}`
      );
    });

    $('copyShopee').addEventListener('click',() => {
      const r = calculateShopee();
      copyText(
`RESUMO DA VENDA NA SHOPEE
Preço de venda: ${money.format(r.sale)}
Custo do produto: ${money.format(r.production)}
Embalagem: ${money.format(r.packaging)}
Outros custos: ${money.format(r.other)}
Taxas percentuais: ${money.format(r.pctFees)}
Taxa fixa: ${money.format(r.fixed)}
ROAS configurado: ${numberBR.format(r.roas)}x
ADS estimado: ${money.format(r.ads)}
Lucro líquido: ${money.format(r.profit)}
Margem líquida: ${numberBR.format(r.margin)}%
Preço recomendado: ${money.format(r.suggested)}`
      );
    });

    $('resetProduction').addEventListener('click',() => {
      const calculationDefaults = {
        filamentGrams:0,
        printHours:0,
        printMinutes:0,
        batchQty:1,
        extraProduction:0
      };
      Object.entries(calculationDefaults).forEach(([id,val]) => $(id).value = val);
      updateAll();
      toast('Cálculo limpo; custos fixos preservados');
    });

    $('saveAdvanced').addEventListener('click',() => {
      save();
      toast('Custos fixos salvos neste aparelho');
    });

    $('resetAdvanced').addEventListener('click',() => {
      const k2PlusDefaults = {
        filamentKg:85,
        printerValue:10000,
        printerLife:10000,
        powerW:500,
        energyRate:0.95,
        maintenancePct:10,
        lossPct:5
      };
      Object.entries(k2PlusDefaults).forEach(([id,val]) => $(id).value = val);
      updateAll();
      toast('Perfil padrão da K2 Plus restaurado');
    });

    $('resetShopee').addEventListener('click',() => {
      const defaults = {
        salePrice:39.90,productionCost:0,packagingCost:1,otherSaleCosts:0,
        shopeeFeePct:22.5,campaignFeePct:2.5,fixedFee:4,taxPct:0,adsValue:6,desiredProfit:10
      };
      Object.entries(defaults).forEach(([id,val]) => $(id).value = val);
      setAdsMode('roas',false);
      updateAll();
      toast('Venda restaurada');
    });

    registerPWA();
    updateInstallButton();
    load();
    loadSavedProducts();
    loadSyncDevice();
    resetCollectedSync();
    calculateProduction();
    calculateShopee();

    const initialTab = ['producao','shopee','produtos','sync'].includes(location.hash.slice(1))
      ? location.hash.slice(1)
      : 'producao';
    showTab(initialTab);
  </script>
</body>
</html>
