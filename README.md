# websity_netlify

# How to Publish an HTML Website on Netlify & Github

## How to Publish a Website on Netlify

---

### Step 1: Log in to Github
* click on the “New” button on the top left side to create a new repository like _yourgithubusername.github.io_.
* than _add file_ __index.html__ and __/dist/style.css__ to repository _yourgithubusername.github.io_
* __index.html__ like:

```html
 <!DOCTYPE html>
 <html lang="en">
  <head>
   <meta charset="utf-8">
   <title>Пример веб-страницы</title>

   <link rel="stylesheet" href="/dist/style.css">

  </head>
  <body>
   <h1>Заголовок</h1>
   <!-- Комментарий -->
   <p>Первый абзац.</p>
   <p>Второй абзац.</p>
  </body>
 </html>
```

* dist/__style.css__ like:
```css
:root{--border-radius-1: 2px;--border-radius-2: 4px;--border-radius-3: 8px;--border-radius-4: 16px;--border-radius-scale: 2px;--border-radius-pill: 360px;--neutral-light-100: #f6f6f7;--neutral-light-200: #e9ebed;--neutral-light-300: #d1d5da;--neutral-light-400: #9da7b2;--neutral-light-500: #778089;--neutral-light-600: #545a61;--neutral-light-700: #353a3e;--neutral-light-800: #181a1c;--neutral-light-000: #ffffff;--neutral-dark-100: #e6ecf2;--neutral-dark-200: #abb5bf;--neutral-dark-300: #7e8792;--neutral-dark-400: #4d565f;--neutral-dark-500: #3b434c;--neutral-dark-600: #272f38;--neutral-dark-700: #1e242c;--neutral-dark-800: #12181f;--neutral-dark-900: #060b10;--neutral-dark-000: #ffffff;--teal-100: #8efbf7;--teal-200: #32e6e2;--teal-300: #14d8d4;--teal-400: #05bdba;--teal-500: #04a29f;--teal-600: #02807d;--teal-700: #016968;--teal-800: #014847;--teal-900: #0c2a2a;--teal-000: #defffe;--blue-100: #cde2ff;--blue-200: #b5d2fb;--blue-300: #9cbef6;--blue-400: #80abfa;--blue-500: #5d8df5;--blue-600: #316bf4;--blue-700: #2e51ed;--blue-800: #2036a1;--blue-900: #1b205b;--blue-000: #edf4ff;--gold-100: #f6e0a5;--gold-200: #facd6f;--gold-300: #fbb13d;--gold-400: #f98e21;--gold-500: #d5771a;--gold-600: #a85d13;--gold-700: #8c4c0d;--gold-800: #603408;--gold-900: #332213;--gold-000: #fdf5d8;--red-100: #fbd3d0;--red-200: #ffbdba;--red-300: #ffada9;--red-400: #fe8382;--red-500: #fe4e5c;--red-600: #d62740;--red-700: #af2536;--red-800: #800a20;--red-900: #3d1c1b;--red-000: #fbeeed;--green-100: #bef9c6;--green-200: #93f5a5;--green-300: #64d87f;--green-400: #3ac364;--green-500: #31a855;--green-600: #228240;--green-700: #1a6b34;--green-800: #0f4a21;--green-900: #152a19;--green-000: #e7fce9;--pink-100: #f6d2f2;--pink-200: #f7bcf3;--pink-300: #f3a8ee;--pink-400: #ef7feb;--pink-500: #df5adc;--pink-600: #b938b8;--pink-700: #9a2d99;--pink-800: #6c1d6b;--pink-900: #381b37;--pink-000: #fcf0fb;--purple-100: #e2d9f7;--purple-200: #d8c7ff;--purple-300: #cab9f4;--purple-400: #b49df1;--purple-500: #9b80ed;--purple-600: #775ce7;--purple-700: #614aca;--purple-800: #382aa4;--purple-900: #292142;--purple-000: #f5f2fc}*,*::before,*::after{box-sizing:border-box}html,body,h1,h2,h3,h4,h5,p,figure,blockquote,dl,dd,ul,ol,pre,code{margin:0}:where(p,h1,h2,h3,h4,h5,h6){overflow-wrap:break-word}:where(ul,ol){padding-inline-start:1em}:where(ul[role=list],ol[role=list],ul[class],ol[class]){list-style:none;padding-inline-start:0}@media(prefers-reduced-motion: no-preference){html:focus-within{scroll-behavior:smooth}}html{-moz-text-size-adjust:none;-webkit-text-size-adjust:none;text-size-adjust:none}body{line-height:1.5;min-height:100vh}a{color:currentcolor}a:not([class]){text-decoration-skip-ink:auto}picture,img,video,iframe,object{display:block;max-inline-size:100%;block-size:auto}input,button,textarea,select{font:inherit}:root{--font-system: system-ui, -apple-system, BlinkMacSystemFont, “Segoe UI”, Roboto, Oxygen-Sans, Ubuntu, Cantarell, “Helvetica Neue”, Arial, sans-serif;--font-primary: Mulish, var(--font-system);--font-secondary: Pacaembu, var(--font-system);--font-heading: var(--font-secondary);--font-monospace: ui-monospace, "Cascadia Code", "Source Code Pro", Menlo, Consolas, "DejaVu Sans Mono", monospace;--step--1: clamp(0.625rem, 0.5811rem + 0.2193vi, 0.9375rem);--step-0: clamp(0.75rem, 0.6974rem + 0.2632vi, 1.125rem);--step-1: clamp(0.9rem, 0.8368rem + 0.3158vi, 1.35rem);--step-2: clamp(1.08rem, 1.0042rem + 0.3789vi, 1.62rem);--step-3: clamp(1.296rem, 1.2051rem + 0.4547vi, 1.944rem);--step-4: clamp(1.5552rem, 1.4461rem + 0.5457vi, 2.3328rem);--step-5: clamp(1.8662rem, 1.7353rem + 0.6548vi, 2.7994rem);--step-6: clamp(2.2395rem, 2.0823rem + 0.7858vi, 3.3592rem);--radius-1: 4px;--radius-2: 6px;--radius-3: 10px;--grid-line-size: 10px;--icon-chevron: url(data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCA1MTIgNTEyIj4KICA8cGF0aCBmaWxsPSIjMTgxYTFjIiBkPSJNMjMzLjQgNDA2LjZjMTIuNSAxMi41IDMyLjggMTIuNSA0NS4zIDBsMTkyLTE5MmMxMi41LTEyLjUgMTIuNS0zMi44IDAtNDUuM3MtMzIuOC0xMi41LTQ1LjMgMEwyNTYgMzM4LjcgODYuNiAxNjkuNGMtMTIuNS0xMi41LTMyLjgtMTIuNS00NS4zIDBzLTEyLjUgMzIuOCAwIDQ1LjNsMTkyIDE5MnoiLz4KPC9zdmc+);--text-color-primary: #ffffffdd;--text-color-vibrant: #ffffff;--shade-down-1: #00000008;--shade-down-2: #00000015;--shade-down-3: #00000022;--gradient-main: var(--blue-900) 10vh, var(--blue-800) 80vh}.light-mode{--gradient-main: var(--blue-100) 5vh, white 20vh;--text-color-primary: #000000aa;--text-color-vibrant: #000;--shade-down-1: #00000008;--shade-down-2: #00000015;--shade-down-3: #00000022}@font-face{font-family:Pacaembu;src:url(https://example-styles.netlify.app/fonts/PacaembuVar-latin.woff2) format("woff2");unicode-range:U+5,U+20,U+21,U+24,U+25,U+26,U+27,U+2B-2E,U+30-3A,U+3F,U+41-5A,U+61-7A,U+D7,U+2019,U+201C,U+201D;font-weight:100 1000;font-display:swap}@font-face{font-family:Mulish;src:url(https://example-styles.netlify.app/fonts/MulishVar-latin.woff2) format("woff2");unicode-range:U+5,U+20,U+21,U+24,U+25,U+26,U+27,U+2B-2E,U+30-3A,U+3F,U+41-5A,U+61-7A,U+D7,U+2019,U+201C,U+201D;font-weight:200 900;font-display:swap}body{text-align:center;min-height:100vh;display:flex;flex-direction:column;gap:0}header nav,footer nav{display:flex;flex-direction:row;justify-content:space-between;align-items:center;gap:1em;padding:2em 0em;margin:0;border-bottom:solid .5px rgba(255,255,255,.1333333333)}header nav ul,footer nav ul{list-style:none;display:flex;flex-direction:row;justify-content:space-between;align-items:center;gap:1em}main{padding-bottom:6em}section{text-align:left;max-width:70ch;margin:2em auto 4em}header section{margin-top:3em;margin-bottom:5em}footer{background-color:#fff;padding:4em;margin:0 -2rem}footer>div{text-align:left;margin:2em auto}footer section{margin:0;padding:0}footer .links-container{display:flex;flex-wrap:wrap;gap:3rem;justify-content:start;margin-top:3rem}footer small{font-size:1em;display:flex;justify-content:space-between;align-items:baseline;flex-wrap:wrap;margin-top:4em;border-top:solid 1px var(--neutral-dark-100);color:var(--neutral-dark-300)}footer small ul{list-style:none;display:flex;flex-wrap:wrap;justify-content:flex-start;gap:1em}.flex-btwn{display:flex;justify-content:space-between;align-content:center}.panel{background-color:var(--shade-down-2);border-radius:var(--radius-3);padding:2em;margin:2em 0}body{color:var(--text-color-primary);line-height:1.6;font-size:var(--step-1);font-family:var(--font-primary)}nav{font-size:var(--step-0)}h1,h2,h3,h4{font-family:var(--font-heading);padding:1em 0 .75em;line-height:1.3;text-wrap:pretty;color:var(--text-color-vibrant)}h1{font-size:var(--step-6)}h2{font-size:var(--step-5)}h3{font-size:var(--step-4)}h4{font-size:var(--step-3)}h4{font-family:var(--font-primary);font-weight:600}p+p{margin-top:1.5em}blockquote{border-left:solid 2px var(--blue-100);background:var(--shade-down-2);padding:2em;margin:2em 0;font-size:var(--step-0)}blockquote h1,blockquote h2,blockquote h3,blockquote h4{font-size:1.4em;padding-top:0}ul,ol{margin:1em 0}li::marker{color:var(--blue-200)}dl{margin:1em 0;display:grid;grid-template-columns:max-content 1fr;gap:.4em 1em}dt{font-weight:700}dt::after{content:":"}footer{font-size:.85em}footer h3{color:#000;font-size:1.1em;font-family:var(--font-primary);font-weight:700;padding-block:var(--space-s)}footer li{margin-block-start:12px}footer a:link,footer a:visited{color:var(--neutral-dark-300);text-decoration:none}footer a:hover,footer a:focus{color:var(--neutral-dark-900);text-decoration:underline}a.btn-primary:link,a.btn-primary:visited,a.btn-secondary:link,a.btn-secondary:visited,input[type=submit],button{background-color:var(--teal-200);color:var(--blue-800);border:1px solid var(--teal-200);padding:.3em 1em;margin:1em auto;border-radius:var(--radius-2);font-weight:600;font-size:.9em;font-family:var(--font-heading);text-decoration:none;display:inline-block;transition:all 300ms;cursor:pointer}a.btn-secondary:link,a.btn-secondary:visited{color:var(--blue-000);background-color:rgba(0,0,0,0);border-color:#fff}a.btn-primary:hover,a.btn-primary:focus,a.btn-secondary:hover,a.btn-secondary:focus,button:not(:disabled):hover,button:not(:disabled):focus{background-color:#fff;color:var(--blue-800);border:1px solid #fff;cursor:pointer;transition:all 100ms}button:disabled{opacity:.4;cursor:not-allowed}form{background-color:var(--shade-down-2);border-radius:var(--radius-3);padding:2em}label{font-size:.9em;color:var(--text-color-primary)}input:not([type=submit]),select{width:100%;font-size:1.1em;border:solid 1px #000;border-radius:var(--radius-2);padding:.3em .8em;margin-bottom:.8em}input[type=text]::placeholder,input[type=password]::placeholder{color:var(--neutral-light-500)}input[type=submit]{padding:.4em 1em}input[type=submit]:not(:disabled):hover,input[type=submit]:not(:disabled):focus{background-color:#fff;border-color:#fff}select{appearance:none;-webkit-appearance:none;background-image:var(--icon-chevron);background-position:calc(100% - 8px);background-repeat:no-repeat;background-size:.75em}label>*{display:block;margin-top:.3em}pre,code{background-color:var(--blue-900);color:var(--blue-300)}code{padding:.2em;border-radius:var(--radius-1);font-size:var(--step-0)}pre{padding:1em;margin:1em 0;border-radius:var(--radius-3);overflow-y:scroll}pre code{padding:0}.hljs-cdata,.hljs-comment,.hljs-doctype,.hljs-prolog{color:#568ccf}.hljs-punctuation{color:#c5c8c6}.namespace{opacity:.7}.hljs-keyword,.hljs-property,.hljs-tag{color:#95d6f8}.hljs-title.class_{color:#fff}.hljs-boolean,.hljs-constant{color:#9c9}.hljs-symbol{color:#f92672}.hljs-number{color:#ff73fd}.hljs-attr-name,.hljs-builtin,.hljs-char,.hljs-inserted,.hljs-selector,.hljs-string{color:#00faee}.hljs-variable{color:#c6c5fe}.hljs-operator{color:#ededed}.hljs-entity{color:#ffffb6;cursor:help}.hljs-url{color:#96cbfe}.language-css .hljs-string,.style .hljs-string{color:#87c38a}.hljs-atrule,.hljs-attr-value{color:#f9ee98}.hljs-title.function_{color:#dad085}.hljs-regex{color:#e9c062}.hljs-important{color:#fd971f}.hljs-bold,.hljs-important{font-weight:bold}.hljs-italic{font-style:italic}.hljs-prefix.deleted,.hljs-prefix.inserted,.hljs-prefix.unchanged{-webkit-user-select:none;-moz-user-select:none;-ms-user-select:none;user-select:none}.hljs-table{background:0 0;box-shadow:none;display:inline}::selection{background-color:var(--teal-200);color:#000}html{background:linear-gradient(180deg, var(--gradient-main))}body{padding:0 2rem;font-family:var(--font-primary);background:linear-gradient(rgba(0, 0, 0, 0.062745098) 0.5px, transparent 0.5px),linear-gradient(90deg, rgba(0, 0, 0, 0.062745098) 0.5px, transparent 0.5px);background-size:var(--grid-line-size) var(--grid-line-size)}footer .nf-logo,header .nf-logo{height:var(--step-5);color:#fff}hr{border-style:none;border-top:solid .5px rgba(255,255,255,.1333333333);margin:0}a:link,a:visited{color:var(--text-color-vibrant);text-decoration:underline;text-decoration-color:rgba(255,255,255,.4666666667);text-decoration-thickness:1px;text-underline-offset:.2em;transition:all 300ms}a:hover,a:focus{text-decoration-color:var(--teal-200);text-underline-offset:.3em;transition:all 100ms}.social-icons{display:flex;gap:1em;justify-content:space-between;margin-bottom:2em}.social-icons a:link,.social-icons a:visited{display:inline-block;opacity:.3}.social-icons a:focus,.social-icons a:hover{opacity:1}.social-icons img{width:24px;height:24px}
```

### Step 2: Go to netlify.com
<ol>
  <li>Import an existing project</li>
  <li>Choose Github Let’s deploy your project with username.github.io</li>
  <li>Review configuration for username.github.io</li>
  <ol>
  <li>Team: username's team</li>
  <li>Site name: (empty)</li>
  <li>Branch to deploy: main</li>
  <li>Base directory: (empty)</li>
  <li>Build command: (empty)</li>
  <li>Publish directory: (empty)</li>
  </ol>
  <li>Deploy username.github.io</li>

### Step 3: Enable visual editing for resilient-*

### Step 4: Contact forms
```html
<form name="contact" netlify>
  <p>
    <label>Name <input type="text" name="name" /></label>
  </p>
  <p>
    <label>Email <input type="email" name="email" /></label>
  </p>
    <label>Message: <textarea name="message"></textarea></label>  <p>
    <button type="submit">Send</button>
  </p>
</form>
```


### Step 5:

### Step 6:

### Step 7:

### Step 8:

### Step 9:

### Step 10:


---

### Step 1: Add your new site
Click the New site from git button to add your new website to Netlify.

### Step 2: Link to your GitHub
When you click the New site from git button, it will take you to the "Create a new site" page. Make sure that you push your repository on GitHub so that Netlify can link to your GitHub account.

### Step 3: Authorize Netlify
Next, click the Authorize Netlify by Netlify button. This permission is needed so that both Netlify and GitHub can connect.

### Step 4: Select your repository
Once you grant permission to Netlify, you can see a list of all your repositories. Select your website to publish. You can find it by either scrolling down the list or using the search bar to narrow down the list.

### Step 5: Configure your settings
After selecting your website, you will be prompted to configure the settings for deploying the website. Since your website is simply a static one, there's not much to do here. Just click Deploy site to continue.

### Step 6: Publish your website
Your website is now ready to publish! Netlify will do the rest of the work for you, and it will only take a minute or so to complete the process.

Now you are done! Your new website is published, and you can view it by clicking the green link.
Right now, your URL looks random, but you can edit it by clicking the Site settings button and then the Change site name button.

Congratulation on publishing your first new website! Now we'll learn how to publish a website with GitHub.

## How to Publish a Website on GitHub

The second method we'll look at uses GitHub to publish your site. GitHub is a platform for storing, tracking, and managing project source code. It is also where you can publish your HTML website – and like Netlify, it is free to host here.
Here's the step-by-step process of publishing your website on GitHub:
Note: You can only publish your website on GitHub if you set the repository's visibility to public. If you want to deploy a website while it is private, upgrade your account to Pro or use Netlify to host there instead.

### Step 1: Go to your website's repository
After you've logged in, go to the repository on the left sidebar and select the one you want to publish.

### Step 2: Select the settings
In your repository, click the Settings link, and it will take you to the repository's settings page.

### Step 3: Go to GitHub Pages
When you're in a repository's settings, scroll down a bit until you see the Pages link on the left sidebar. Click it, and it will lead you to GitHub Pages.

### Step 4: Select the branch
In the source section, click the dropdown and select the master branch and save it. Depending on how you name it, it can be master or main.

### Step 5: All done
And you are done! Your website will be published, and it will take only a minute or so to complete the process. Refresh the page, and you will see a link to your newly published website.

Conclusion
I hope you've found this tutorial helpful. You have learned how to publish your HTML website with Netlify and GitHub. Now you can go ahead and show the world of your incredible work.

### Source:

> [Netlify](https://www.netlify.com/)

> [Get started with Netlify](https://docs.netlify.com/get-started/)

> [Publish your website netlify github](https://www.freecodecamp.org/news/publish-your-website-netlify-github/)

> [Github pages vs netlify](https://www.aleksandrhovhannisyan.com/blog/github-pages-vs-netlify/)

> [Beginners guide github netlify](https://sjinnovation.com/beginners-guide-deploy-super-fast-website-nelify-or-github-within-minutes)
