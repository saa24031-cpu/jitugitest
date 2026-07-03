<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>石鎚黒茶 — ISHIZUCHI KUROCHA</title>
  <!-- Tailwind CSS CDN -->
  <script src="https://cdn.tailwindcss.com"></script>
  <!-- Google Fonts (Noto Serif JP & Noto Sans JP) -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Noto+Sans+JP:wght@300;400;500;700&family=Noto+Serif+JP:wght@400;700;900&display=swap" rel="stylesheet">
  
  <script>
    tailwind.config = {
      theme: {
        extend: {
          fontFamily: {
            serif: ['"Noto Serif JP"', 'serif'],
            sans: ['"Noto Sans JP"', 'sans-serif'],
          },
          colors: {
            tea: {
              50: '#fdfaf2',
              100: '#f7f0df',
              200: '#ebd8b6',
              300: '#deb985',
              400: '#cc9754',
              500: '#be803f',
              600: '#9d5d2b',
              700: '#7e4422',
              800: '#64341c',
              900: '#482212',
            },
            slate: {
              950: '#0f172a',
            }
          }
        }
      }
    }
  </script>
  <style>
    /* 滑らかなスクロールとカスタムスクロールバー */
    html {
      scroll-behavior: smooth;
    }
    ::-webkit-scrollbar {
      width: 8px;
    }
    ::-webkit-scrollbar-track {
      background: #fdfaf2;
    }
    ::-webkit-scrollbar-thumb {
      background: #be803f;
      border-radius: 4px;
    }
  </style>
</head>
<body class="font-sans bg-tea-50 text-stone-800 antialiased leading-relaxed">

  <!-- Header -->
  <header class="sticky top-0 z-50 bg-tea-50/90 backdrop-blur-md border-b border-tea-100">
    <div class="max-w-6xl mx-auto px-4 h-20 flex items-center justify-between">
      <a href="#" class="flex items-center space-x-3">
        <span class="font-serif font-black text-xl tracking-wider text-tea-900">石鎚黒茶</span>
        <span class="text-xs bg-tea-700 text-white px-2.5 py-1 rounded-full font-semibold">幻の後発酵茶</span>
      </a>
      <nav class="hidden md:flex space-x-8 text-sm font-medium text-tea-900">
        <a href="#about" class="hover:text-tea-600 transition-colors">石鎚黒茶とは</a>
        <a href="#fermentation" class="hover:text-tea-600 transition-colors">二段階発酵の秘密</a>
        <a href="#brewing" class="hover:text-tea-600 transition-colors">美味しい淹れ方</a>
        <a href="#pairings" class="hover:text-tea-600 transition-colors">ペアリング</a>
      </nav>
      <a href="#brewing" class="bg-tea-800 hover:bg-tea-900 text-tea-50 text-xs font-bold tracking-widest uppercase px-5 py-3 rounded-lg transition-all shadow-md hover:shadow-lg">
        Brewing Timer
      </a>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="relative py-16 md:py-24 overflow-hidden border-b border-tea-100">
    <div class="max-w-6xl mx-auto px-4 grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
      <!-- Text Content -->
      <div class="lg:col-span-5 space-y-6 z-10">
        <div class="inline-flex items-center space-x-2 bg-tea-100 text-tea-800 px-3 py-1.5 rounded-full text-xs font-semibold tracking-wider">
          <span>愛媛県西条市ブランド認定</span>
        </div>
        <h2 class="font-serif text-4xl md:text-5xl lg:text-6xl text-tea-900 font-bold leading-tight">
          四国霊峰の麓、<br>
          <span class="text-tea-700">二度の発酵</span>が紡ぐ<br>
          琥珀色の奇跡。
        </h2>
        <p class="text-stone-600 text-base md:text-lg">
          日本にわずか4つしか存在しない「後発酵茶」。石鎚山の澄んだ空気と、職人の卓越した技によって、果実のような爽やかな酸味と奥深いコクが共存する、至高の一杯が生まれました。
        </p>
        <div class="pt-4 flex flex-col sm:flex-row gap-4">
          <a href="#about" class="inline-flex justify-center items-center px-6 py-3.5 bg-tea-800 hover:bg-tea-900 text-white font-medium rounded-lg shadow-lg hover:shadow-xl transition-all">
            その歴史を紐解く
            <svg class="w-4 h-4 ml-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M14 5l7 7m0 0l-7 7m7-7H3"></path></svg>
          </a>
          <a href="#brewing" class="inline-flex justify-center items-center px-6 py-3.5 bg-white hover:bg-tea-100 border border-tea-200 text-tea-800 font-medium rounded-lg transition-all">
            淹れ方を学ぶ
          </a>
        </div>
      </div>

      <!-- Main Visual Container -->
      <div class="lg:col-span-7 relative">
        <div class="absolute -top-12 -left-12 w-64 h-64 bg-tea-200/40 rounded-full filter blur-3xl -z-10"></div>
        <div class="absolute -bottom-12 -right-12 w-64 h-64 bg-tea-300/30 rounded-full filter blur-3xl -z-10"></div>
        
        <div class="bg-white p-4 rounded-2xl shadow-xl border border-tea-100 transform hover:scale-[1.01] transition-transform">
          <!-- 
            IMAGE PLACEHOLDER:
            [image_0.png] の位置に画像を表示。
            環境に応じてsrcを実際のURLやパスに書き換えてください。
          -->
          <div class="relative overflow-hidden rounded-xl aspect-[4/3] bg-stone-100 flex items-center justify-center group">
            <img 
              src="[image_0.png]" 
              alt="石鎚黒茶の佇まい - 木目の温もり、ガラス急須に映える琥珀色の抽出液、そして静かに佇む茶葉とパッケージ" 
              class="object-cover w-full h-full"
              onerror="this.onerror=null; this.parentElement.innerHTML='<div class=\'text-center p-8\'><svg class=\'w-16 h-16 text-tea-400 mx-auto mb-4\' fill=\'none\' stroke=\'currentColor\' viewBox=\'0 0 24 24\'><path stroke-linecap=\'round\' stroke-linejoin=\'round\' stroke-width=\'1\' d=\'M4 16l4.586-4.586a2 2 0 012.828 0L16 16m-2-2l1.586-1.586a2 2 0 012.828 0L20 14m-6-6h.01M6 20h12a2 2 0 002-2V6a2 2 0 00-2-2H6a2 2 0 00-2 2v12a2 2 0 002 2z\'></path></svg><p class=\'text-tea-800 font-serif font-bold text-lg mb-2\'>[ Main Visual Placeholder ]</p><p class=\'text-stone-500 text-xs max-w-sm mx-auto\'>ここに石鎚黒茶の美しい写真 [image_0.png] が配置されます。木目テーブル、ガラスの急須、琥珀色のお茶、そして石鎚山が描かれたパッケージの世界観をお楽しみください。</p></div>';"
            >
          </div>
          <div class="mt-4 px-2 py-1 text-center">
            <p class="font-serif italic text-stone-500 text-sm">
              木目の温もり、ガラス急須に満ちる琥珀の光、歴史が育んだ芳醇なる一杯。
            </p>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Overview Section -->
  <section id="about" class="py-20 bg-white">
    <div class="max-w-6xl mx-auto px-4">
      <div class="text-center max-w-2xl mx-auto mb-16">
        <span class="text-xs font-bold tracking-widest text-tea-600 uppercase">Project Overview</span>
        <h3 class="font-serif text-3xl md:text-4xl text-tea-900 font-bold mt-2">幻の銘茶「石鎚黒茶」とは</h3>
        <div class="w-12 h-1 bg-tea-500 mx-auto mt-4 rounded"></div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center">
        <div class="space-y-6">
          <p class="text-stone-600 text-lg leading-relaxed">
            愛媛県西条市に今も伝わる<strong>「石鎚黒茶（いしづちくろちゃ）」</strong>は、日本に数えるほどしか存在しない希少な「後発酵茶」のひとつです。
          </p>
          <p class="text-stone-600">
            名峰・石鎚山の豊かな自然と、西条市の澄み切った名水「うちぬき」に育まれ、古くからお遍路さんたちを癒やすお茶として愛されてきました。一時は生産者が途絶えかけ、まさに「幻」となりましたが、地元の手仕事と情熱的な技術継承により、その伝統製法が奇跡的に守り抜かれました。
          </p>
          <p class="text-stone-600">
            最大の特徴は、パッケージにも描かれている石鎚山の美しき山並みのように、清らかでありながらも力強い風味。独特の発酵プロセスによって醸される、フルーティーで澄んだ味が現代のテーブルを彩ります。
          </p>
        </div>

        <!-- Spec Table Card -->
        <div class="bg-tea-50 p-8 rounded-2xl border border-tea-100 shadow-sm">
          <h4 class="font-serif font-bold text-xl text-tea-900 mb-6 flex items-center">
            <svg class="w-5 h-5 mr-2 text-tea-600" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path></svg>
            石鎚黒茶の品質仕様
          </h4>
          <div class="space-y-4 text-sm">
            <div class="flex justify-between py-2.5 border-b border-tea-200/50">
              <span class="font-medium text-stone-500">生産地</span>
              <span class="font-semibold text-tea-900">愛媛県西条市</span>
            </div>
            <div class="flex justify-between py-2.5 border-b border-tea-200/50">
              <span class="font-medium text-stone-500">お茶の分類</span>
              <span class="font-semibold text-tea-900">後発酵茶（ダブル発酵）</span>
            </div>
            <div class="flex justify-between py-2.5 border-b border-tea-200/50">
              <span class="font-medium text-stone-500">主な原材料</span>
              <span class="font-semibold text-tea-900">石鎚山麓の厳選茶葉</span>
            </div>
            <div class="flex justify-between py-2.5 border-b border-tea-200/50">
              <span class="font-medium text-stone-500">主要含有成分</span>
              <span class="font-semibold text-tea-900">乳酸菌、クエン酸、テアニン</span>
            </div>
            <div class="flex justify-between py-2.5">
              <span class="font-medium text-stone-500">風味プロフィール</span>
              <span class="font-semibold text-tea-900 text-right">爽やかな酸味、後引くまろやかさ</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Fermentation Steps -->
  <section id="fermentation" class="py-20 bg-tea-100/30 border-y border-tea-100">
    <div class="max-w-6xl mx-auto px-4">
      <div class="text-center max-w-2xl mx-auto mb-16">
        <span class="text-xs font-bold tracking-widest text-tea-600 uppercase">Brewing Bio-Technology</span>
        <h3 class="font-serif text-3xl md:text-4xl text-tea-900 font-bold mt-2">二段階の発酵が仕掛ける、味わいの秘密</h3>
        <p class="text-stone-500 mt-3">職人の感覚と自然が共生する、伝統的なダブル・ファーメンテーション</p>
        <div class="w-12 h-1 bg-tea-500 mx-auto mt-4 rounded"></div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-2 gap-8 lg:gap-12 relative">
        <!-- Connecting Line for timeline (Desktop) -->
        <div class="hidden md:block absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 w-12 h-0.5 bg-tea-300"></div>

        <!-- Step 1 -->
        <div class="bg-white p-8 rounded-2xl shadow-sm border border-tea-100 relative overflow-hidden group hover:shadow-md transition-shadow">
          <div class="absolute top-0 right-0 w-24 h-24 bg-tea-50 rounded-bl-full flex items-start justify-end p-4">
            <span class="font-serif font-bold text-3xl text-tea-300">01</span>
          </div>
          <div class="flex items-center space-x-4 mb-6">
            <div class="p-3 bg-tea-100 rounded-xl text-tea-700">
              <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19.428 15.428a2 2 0 00-1.022-.547l-2.387-.477a6 6 0 00-3.86.517l-.318.158a6 6 0 01-3.86.517L6.05 15.21a2 2 0 00-1.806.547M8 4h8l-1 1v5.172a2 2 0 00.586 1.414l5 5c1.26 1.26.367 3.414-1.415 3.414H4.828c-1.782 0-2.674-2.154-1.414-3.414l5-5A2 2 0 009 10.172V5L8 4z"></path></svg>
            </div>
            <div>
              <span class="text-xs font-semibold text-tea-500 uppercase tracking-widest">第一段階 (好気発酵)</span>
              <h4 class="font-serif font-bold text-xl text-tea-900 mt-0.5">こうじ菌（糸状菌）発酵</h4>
            </div>
          </div>
          <p class="text-stone-600">
            手摘みした厳選茶葉を「蒸して、揉む」工程の後、伝統の蔵に生息する「こうじ菌（糸状菌）」を植え付け、空気に触れさせながら発酵させます。この段階で、茶葉が持つ旨味成分が十分に引き出され、芳醇で深いコクの土台が設計されます。
          </p>
        </div>

        <!-- Step 2 -->
        <div class="bg-white p-8 rounded-2xl shadow-sm border border-tea-100 relative overflow-hidden group hover:shadow-md transition-shadow">
          <div class="absolute top-0 right-0 w-24 h-24 bg-tea-50 rounded-bl-full flex items-start justify-end p-4">
            <span class="font-serif font-bold text-3xl text-tea-300">02</span>
          </div>
          <div class="flex items-center space-x-4 mb-6">
            <div class="p-3 bg-tea-100 rounded-xl text-tea-700">
              <svg class="w-8 h-8" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 3v1m0 16v1m9-9h-1M4 12H3m15.364-6.364l-.707.707M6.343 17.657l-.707.707m0-11.314l.707.707m11.314 11.314l.707-.707M12 8a4 4 0 110 8 4 4 0 010-8z"></path></svg>
            </div>
            <div>
              <span class="text-xs font-semibold text-tea-500 uppercase tracking-widest">第二段階 (嫌気発酵)</span>
              <h4 class="font-serif font-bold text-xl text-tea-900 mt-0.5">乳酸菌発酵＆天日干し</h4>
            </div>
          </div>
          <p class="text-stone-600">
            一度目の発酵を終えた茶葉を、今度は木樽に隙間なく敷き詰めて重石を載せ、空気を遮断した密閉状態で「乳酸菌」によってじっくりと発酵させます。その後、天日（てんぴ）でしっかりと乾燥させることで、すっきりとした爽快な酸味と、雑味のない澄んだ余韻が生み出されます。
          </p>
        </div>
      </div>
    </div>
  </section>

  <!-- Interactive Brewing Section & Timer -->
  <section id="brewing" class="py-20 bg-white">
    <div class="max-w-6xl mx-auto px-4">
      <div class="text-center max-w-2xl mx-auto mb-16">
        <span class="text-xs font-bold tracking-widest text-tea-600 uppercase">Brewing Protocol</span>
        <h3 class="font-serif text-3xl md:text-4xl text-tea-900 font-bold mt-2">美味しいお茶の淹れ方</h3>
        <p class="text-stone-500 mt-3">最高の一杯を引き出す、インタラクティブタイマー</p>
        <div class="w-12 h-1 bg-tea-500 mx-auto mt-4 rounded"></div>
      </div>

      <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-center">
        <!-- Guide -->
        <div class="lg:col-span-5 space-y-6">
          <h4 class="font-serif font-bold text-2xl text-tea-900">伝統的な淹れ方で琥珀色を愛でる</h4>
          <p class="text-stone-600">
            石鎚黒茶は沸き立ての熱湯（95℃〜100℃）で淹れるのがおすすめです。熱いお湯を注いだ瞬間、ふわりと立ち上がる発酵由来のほの酸っぱい香り、そしてガラスの器を美しく満たす黄金から琥珀色へのグラデーションをゆっくりとお楽しみください。
          </p>
          
          <ul class="space-y-4">
            <li class="flex items-start">
              <span class="bg-tea-200 text-tea-800 text-xs font-bold w-6 h-6 flex items-center justify-center rounded-full mr-3 mt-1 shrink-0">1</span>
              <span class="text-stone-600 text-sm">茶葉は約3g（大さじ1杯程度）を急須に入れます。</span>
            </li>
            <li class="flex items-start">
              <span class="bg-tea-200 text-tea-800 text-xs font-bold w-6 h-6 flex items-center justify-center rounded-full mr-3 mt-1 shrink-0">2</span>
              <span class="text-stone-600 text-sm">沸騰した熱湯約300mlを、気泡を立てるように静かに注ぎます。</span>
            </li>
            <li class="flex items-start">
              <span class="bg-tea-200 text-tea-800 text-xs font-bold w-6 h-6 flex items-center justify-center rounded-full mr-3 mt-1 shrink-0">3</span>
              <span class="text-stone-600 text-sm">蓋をして、約3分（180秒）じっくりと蒸らします。</span>
            </li>
          </ul>
        </div>

        <!-- Interactive Timer UI -->
        <div class="lg:col-span-7 bg-tea-50 border border-tea-200/60 p-8 rounded-2xl shadow-sm text-center">
          <div class="max-w-xs mx-auto space-y-6">
            <div class="text-xs uppercase tracking-widest font-bold text-tea-600">Steep Timer</div>
            
            <!-- Dial -->
            <div class="relative w-48 h-48 mx-auto flex items-center justify-center bg-white rounded-full border-4 border-tea-300 shadow-inner">
              <div class="text-center">
                <span id="timer-display" class="font-serif text-5xl font-bold text-tea-900">03:00</span>
                <p id="timer-status" class="text-xs text-stone-400 mt-1">Ready</p>
              </div>
            </div>

            <!-- Controls -->
            <div class="flex justify-center space-x-3">
              <button id="btn-start" onclick="toggleTimer()" class="px-6 py-2.5 bg-tea-800 hover:bg-tea-900 text-white font-semibold rounded-lg shadow-sm transition-all focus:outline-none">
                スタート
              </button>
              <button id="btn-reset" onclick="resetTimer()" class="px-6 py-2.5 bg-white hover:bg-tea-100 text-tea-800 border border-tea-200 font-semibold rounded-lg transition-all focus:outline-none">
                リセット
              </button>
            </div>

            <!-- Audio or Alert message -->
            <div id="timer-alert" class="hidden text-xs text-tea-700 bg-tea-100 p-2.5 rounded-lg font-medium transition-all animate-pulse">
              🍵 お茶が飲み頃になりました！静かに注ぎ切ってください。
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Pairings Section -->
  <section id="pairings" class="py-20 bg-tea-100/30 border-y border-tea-100">
    <div class="max-w-6xl mx-auto px-4">
      <div class="text-center max-w-2xl mx-auto mb-16">
        <span class="text-xs font-bold tracking-widest text-tea-600 uppercase">Sensory Harmony</span>
        <h3 class="font-serif text-3xl md:text-4xl text-tea-900 font-bold mt-2">おすすめの楽しみ方・ペアリング</h3>
        <p class="text-stone-500 mt-3">石鎚黒茶ならではの「クエン酸のさっぱり感」が、様々な食の時間を贅沢にします</p>
        <div class="w-12 h-1 bg-tea-500 mx-auto mt-4 rounded"></div>
      </div>

      <!-- Tab Buttons -->
      <div class="flex justify-center space-x-2 mb-10 max-w-md mx-auto bg-tea-100 p-1.5 rounded-xl border border-tea-200/50">
        <button onclick="switchTab('wagashi')" id="tab-wagashi" class="tab-btn flex-1 py-2 text-sm font-medium rounded-lg bg-tea-800 text-white shadow-sm transition-all">
          和菓子
        </button>
        <button onclick="switchTab('yogashi')" id="tab-yogashi" class="tab-btn flex-1 py-2 text-sm font-medium rounded-lg text-tea-900 hover:bg-tea-200/50 transition-all">
          洋菓子
        </button>
        <button onclick="switchTab('meal')" id="tab-meal" class="tab-btn flex-1 py-2 text-sm font-medium rounded-lg text-tea-900 hover:bg-tea-200/50 transition-all">
          食事
        </button>
      </div>

      <!-- Tab Contents -->
      <div class="max-w-3xl mx-auto">
        <!-- Wagashi -->
        <div id="content-wagashi" class="tab-content block space-y-6 bg-white p-8 rounded-2xl border border-tea-100 shadow-sm animate-fadeIn">
          <div class="flex flex-col sm:flex-row gap-6 items-center">
            <div class="w-20 h-20 shrink-0 bg-tea-100 text-tea-800 rounded-full flex items-center justify-center text-3xl">🍡</div>
            <div>
              <h4 class="font-serif font-bold text-xl text-tea-900 mb-2">和菓子：あんこの上品な甘みを引き立てる</h4>
              <p class="text-stone-600">
                羊羹や大福、どら焼きといった重厚な甘みを持つ和菓子との相性は究極です。お茶が持つ爽快な酸味と奥深さが、餡（あん）の甘みを包み込み、口の中をすっきりとリフレッシュさせてくれます。ひとくち毎にお互いの良さが際立つ、贅沢なループが始まります。
              </p>
            </div>
          </div>
        </div>

        <!-- Yogashi (Hidden by default) -->
        <div id="content-yogashi" class="tab-content hidden space-y-6 bg-white p-8 rounded-2xl border border-tea-100 shadow-sm animate-fadeIn">
          <div class="flex flex-col sm:flex-row gap-6 items-center">
            <div class="w-20 h-20 shrink-0 bg-tea-100 text-tea-800 rounded-full flex items-center justify-center text-3xl">🍰</div>
            <div>
              <h4 class="font-serif font-bold text-xl text-tea-900 mb-2">洋菓子：濃厚なバター、チョコレートとの融合</h4>
              <p class="text-stone-600">
                バターをふんだんに使用したフィナンシェやマドレーヌ、またはカカオ香るチョコレートと石鎚黒茶を合わせてみてください。発酵由来のクエン酸が焼き菓子のオイル分をさっぱりとさせ、まるで上品なレモンティーやフルーツティーを合わせているかのような立体的な余韻を楽しめます。
              </p>
            </div>
          </div>
        </div>

        <!-- Meal (Hidden by default) -->
        <div id="content-meal" class="tab-content hidden space-y-6 bg-white p-8 rounded-2xl border border-tea-100 shadow-sm animate-fadeIn">
          <div class="flex flex-col sm:flex-row gap-6 items-center">
            <div class="w-20 h-20 shrink-0 bg-tea-100 text-tea-800 rounded-full flex items-center justify-center text-3xl">🍱</div>
            <div>
              <h4 class="font-serif font-bold text-xl text-tea-900 mb-2">食事：油を流し、料理の風味を引き立てる</h4>
              <p class="text-stone-600">
                中華料理や揚げ物、少し脂ののったお魚料理など、食事のお供としても非常に優秀です。後発酵茶特有のクリーンな喉越しと適度な酸味が、口の中の油っぽさをきれいに洗い流します。毎日の食卓に添えることで、食後も軽やかに過ごすことができます。
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Footer / Call to Action -->
  <footer class="bg-tea-950 text-tea-100/80 py-16">
    <div class="max-w-6xl mx-auto px-4 grid grid-cols-1 md:grid-cols-3 gap-12 border-b border-tea-900 pb-12">
      <div class="space-y-4">
        <h5 class="font-serif font-bold text-xl text-white">石鎚黒茶 — Saijo</h5>
        <p class="text-sm">
          愛媛県西条市の澄んだ水、豊かな自然、そして受け継がれる「二段階発酵」という伝統技術をデジタルで世界へ。
        </p>
      </div>
      <div class="space-y-4">
        <h5 class="font-bold text-sm text-white tracking-widest uppercase">Quick Links</h5>
        <ul class="space-y-2 text-sm">
          <li><a href="#about" class="hover:text-white transition-colors">石鎚黒茶とは</a></li>
          <li><a href="#fermentation" class="hover:text-white transition-colors">二段階発酵の秘密</a></li>
          <li><a href="#brewing" class="hover:text-white transition-colors">美味しい淹れ方</a></li>
          <li><a href="#pairings" class="hover:text-white transition-colors">おすすめペアリング</a></li>
        </ul>
      </div>
      <div class="space-y-4">
        <h5 class="font-bold text-sm text-white tracking-widest uppercase">About Us</h5>
        <p class="text-sm">
          この紹介プロジェクトは、地域の素晴らしい伝統工芸や食文化の存続を支援するため、デジタルUXと美学を融合させて情報発信を行っています。
        </p>
      </div>
    </div>
    
    <div class="max-w-6xl mx-auto px-4 pt-8 text-center text-xs text-tea-200/50 flex flex-col sm:flex-row justify-between items-center gap-4">
      <p>© 2026 Saijo Content & Frontend Project. Developed with 🤎 by Developer.</p>
      <div class="flex space-x-4">
        <span class="hover:text-white transition-colors cursor-pointer">Privacy Policy</span>
        <span>•</span>
        <span class="hover:text-white transition-colors cursor-pointer">Terms of Service</span>
      </div>
    </div>
  </footer>

  <!-- Interactivity Script (Timer & Tabs) -->
  <script>
    // --- TIMER SYSTEM ---
    let timerInstance = null;
    let timeRemaining = 180; // 3 minutes in seconds
    let isRunning = false;

    const timerDisplay = document.getElementById('timer-display');
    const timerStatus = document.getElementById('timer-status');
    const btnStart = document.getElementById('btn-start');
    const timerAlert = document.getElementById('timer-alert');

    function updateDisplay() {
      const mins = Math.floor(timeRemaining / 60);
      const secs = timeRemaining % 60;
      timerDisplay.innerText = `${String(mins).padStart(2, '0')}:${String(secs).padStart(2, '0')}`;
    }

    function toggleTimer() {
      if (isRunning) {
        // Pause
        clearInterval(timerInstance);
        isRunning = false;
        btnStart.innerText = '再開';
        btnStart.className = 'px-6 py-2.5 bg-tea-600 hover:bg-tea-700 text-white font-semibold rounded-lg shadow-sm transition-all focus:outline-none';
        timerStatus.innerText = 'Paused';
      } else {
        // Start
        timerAlert.classList.add('hidden');
        isRunning = true;
        btnStart.innerText = '一時停止';
        btnStart.className = 'px-6 py-2.5 bg-amber-600 hover:bg-amber-700 text-white font-semibold rounded-lg shadow-sm transition-all focus:outline-none';
        timerStatus.innerText = 'Steeping...';
        
        timerInstance = setInterval(() => {
          if (timeRemaining > 0) {
            timeRemaining--;
            updateDisplay();
          } else {
            // Timer Finished
            clearInterval(timerInstance);
            isRunning = false;
            btnStart.innerText = 'スタート';
            btnStart.className = 'px-6 py-2.5 bg-tea-800 hover:bg-tea-900 text-white font-semibold rounded-lg shadow-sm transition-all focus:outline-none';
            timerStatus.innerText = 'Finished';
            timerAlert.classList.remove('hidden');
          }
        }, 1000);
      }
    }

    function resetTimer() {
      clearInterval(timerInstance);
      isRunning = false;
      timeRemaining = 180;
      updateDisplay();
      btnStart.innerText = 'スタート';
      btnStart.className = 'px-6 py-2.5 bg-tea-800 hover:bg-tea-900 text-white font-semibold rounded-lg shadow-sm transition-all focus:outline-none';
      timerStatus.innerText = 'Ready';
      timerAlert.classList.add('hidden');
    }

    // --- TAB SYSTEM ---
    function switchTab(tabId) {
      // Hide all contents
      const contents = document.querySelectorAll('.tab-content');
      contents.forEach(content => {
        content.classList.add('hidden');
        content.classList.remove('block');
      });

      // Reset all tab button styles
      const tabs = document.querySelectorAll('.tab-btn');
      tabs.forEach(tab => {
        tab.className = 'tab-btn flex-1 py-2 text-sm font-medium rounded-lg text-tea-900 hover:bg-tea-200/50 transition-all';
      });

      // Show targeted content
      const activeContent = document.getElementById(`content-${tabId}`);
      activeContent.classList.remove('hidden');
      activeContent.classList.add('block');

      // Highlight targeted tab button
      const activeTab = document.getElementById(`tab-${tabId}`);
      activeTab.className = 'tab-btn flex-1 py-2 text-sm font-medium rounded-lg bg-tea-800 text-white shadow-sm transition-all';
    }
  </script>
</body>
</html>
