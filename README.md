<!doctype html>

<html lang="fa" dir="rtl">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>صفحه پشتیبانی — سایت نمونه</title>
  <style>
    :root{--accent:#0b84ff;--bg:#f7fbff;--card:#ffffff}
    html,body{height:100%;margin:0;font-family: Vazirmatn, "Helvetica Neue", Tahoma, Arial; background:var(--bg);color:#222}
    .container{max-width:980px;margin:48px auto;padding:24px}
    header{display:flex;align-items:center;gap:16px}
    header h1{margin:0;font-size:22px}
    .card{background:var(--card);border-radius:12px;padding:20px;box-shadow:0 6px 20px rgba(20,30,60,0.06)}/* support button */
.support-btn{
  position:fixed;right:18px;bottom:18px;z-index:9999;display:flex;align-items:center;gap:10px;background:var(--accent);color:white;padding:12px 14px;border-radius:999px;box-shadow:0 10px 30px rgba(11,132,255,0.18);cursor:pointer;border:none;outline:none;font-weight:600}
.support-btn:active{transform:translateY(1px)}
.support-btn .dot{width:36px;height:36px;border-radius:50%;display:inline-flex;align-items:center;justify-content:center;background:rgba(255,255,255,0.12)}
.support-btn svg{width:18px;height:18px}
.support-hint{position:fixed;right:18px;bottom:78px;background:#111;color:white;padding:8px 12px;border-radius:8px;box-shadow:0 10px 30px rgba(0,0,0,0.12);font-size:13px;display:none}

/* demo content */
.howto{margin-top:18px}
pre{background:#0f1724;color:#e6f0ff;padding:12px;border-radius:8px;overflow:auto}

footer{margin-top:30px;font-size:13px;color:#555}

@media (max-width:520px){.container{margin:20px 12px;padding:16px}.support-btn{right:12px;left:auto}}

  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="card" style="padding:10px 14px;display:inline-block">نمونه سایت</div>
      <h1>پشتیبانی آنلاین — نمونه</h1>
    </header><section class="card howto" aria-labelledby="howto-title">
  <h2 id="howto-title">چه کار کردیم</h2>
  <p>این صفحه نمونه شاملِ ویجت گفتینو با شناسهٔ <strong>UN9vJh</strong> است. دکمهٔ پشتیبانی گوشهٔ پایین صفحه هم بازشوندهٔ چت است.</p>
  <ol>
    <li>فایل HTML رو دانلود یا روی هاست‌ت بذار.</li>
    <li>این صفحه خودش اسکریپت ویجت رو بار می‌کنه و ویجت باید بعد از لود صفحه نشان داده شود.</li>
    <li>روی دکمهٔ پشتیبانی کلیک کن تا تلاش کنیم ویجت را باز کنیم؛ اگر ویجت سازندهٔ خودش دکمه‌ای ساخت، اسکریپت سعی می‌کند آن را کلیک کند.</li>
  </ol>

  <p>اگر می‌خواهی این صفحه را در وردپرس فعال کنی، فقط محتوای داخل <code>&lt;body&gt;</code> را در فایل قالب (مثلاً <code>footer.php</code>) یا با استفاده از پلاگین "Insert Headers and Footers" قرار بده؛ یا از افزونهٔ Goftino استفاده کن و شناسه را در تنظیمات وارد کن.</p>

  <pre>&lt;!-- فایل HTML: goftino-support-page.html --&gt;

// این فایل شامل اسکریپت ویجت و دکمهٔ پشتیبانی است.

</pre><footer>موفق باشی! اگر می‌خوای این صفحه رو برات روی یک زیردامنه (مثلاً support.yourdomain.com) راه‌اندازی کنم، بگو تا راهنمایی deploy بدم.</footer>
</section>

  </div>  <!-- Support button -->  <button class="support-btn" id="supportBtn" aria-label="پشتیبانی آنلاین">
    <span class="dot" aria-hidden>
      <!-- chat icon -->
      <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden>
        <path d="M21 15a2 2 0 0 1-2 2H8l-5 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2v10z" stroke="currentColor" stroke-width="1.4" stroke-linecap="round" stroke-linejoin="round"></path>
      </svg>
    </span>
    پشتیبانی
  </button>
  <div class="support-hint" id="supportHint">در حال تلاش برای باز کردن پنجرهٔ گفتگو…</div>  <!-- Goftino widget snippet (با شناسهٔ شما) -->  <script type="text/javascript">
    !function(){var i="UN9vJh",a=window,d=document;function g(){var g=d.createElement("script"),s="https://www.goftino.com/widget/"+i,l=localStorage.getItem("goftino_"+i);g.async=!0,g.src=l?s+"?o="+l:s;d.getElementsByTagName("head")[0].appendChild(g);}"complete"===d.readyState?g():a.attachEvent?a.attachEvent("onload",g):a.addEventListener("load",g,!1);}();
  </script>  <script>
    // تلاش می‌کنیم با کلیک روی دکمهٔ ما، ویجت را باز کنیم
    (function(){
      const btn = document.getElementById('supportBtn');
      const hint = document.getElementById('supportHint');

      function tryOpenWidget(){
        hint.style.display = 'block';
        // چند انتخابگر که ممکنه برای لانچر ویجت استفاده شده باشه
        const selectors = [
          'button[data-goftino-launch]',
          '[data-goftino-launch]',
          '.goftino-launcher',
          '.goftino-button',
          'iframe[src*="goftino"]',
          'iframe[id*=goftino]'
        ];

        let clicked = false;
        for(const sel of selectors){
          const el = document.querySelector(sel);
          if(el){
            // اگر iframe است، سعی می‌کنیم با ارسال پیام postMessage بازش کنیم
            if(el.tagName === 'IFRAME'){
              try{ el.contentWindow.postMessage({type:'goftino-open'},'*'); clicked = true; break; }catch(e){}
            }
            try{ el.click(); clicked = true; break; }catch(e){}
          }
        }

        // اگر پیدا نشد، تلاش می‌کنیم فراخوانی عمومی احتمالی را اجرا کنیم
        if(!clicked){
          try{
            if(window.Goftino && typeof window.Goftino.open === 'function'){ window.Goftino.open(); clicked = true; }
          }catch(e){}
        }

        setTimeout(()=>{ hint.style.display = 'none'; if(!clicked) alert('ویجت هنوز بارگذاری نشده یا لانچر قابل کلیک پیدا نشد. لطفاً صفحه را رفرش کن یا از پنل my.goftino.com استفاده کن.'); },1500);
      }

      btn.addEventListener('click', tryOpenWidget, {passive:true});

      // نمایش کوتاه راهنمای شناور پس از بارگذاری
      window.addEventListener('load', ()=>{
        const h = document.getElementById('supportHint');
        h.style.display='block';
        setTimeout(()=>h.style.display='none',1600);
      });
    })();
  </script></body>
</html>
