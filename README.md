<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 900 220" width="100%" height="220">
  <defs>
    <!-- Background Gradient -->
    <linearGradient id="bg-grad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#070709" />
      <stop offset="50%" stop-color="#0f0709" />
      <stop offset="100%" stop-color="#050507" />
    </linearGradient>

    <!-- Red Neon Gradient for Text -->
    <linearGradient id="red-glow-grad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#ff4458" />
      <stop offset="40%" stop-color="#ff1a35" />
      <stop offset="70%" stop-color="#ffffff" />
      <stop offset="100%" stop-color="#ff2a45" />
      <animate attributeName="x1" from="-100%" to="100%" dur="7s" repeatCount="indefinite" />
      <animate attributeName="x2" from="0%" to="200%" dur="7s" repeatCount="indefinite" />
    </linearGradient>

    <!-- Border Glow Gradient -->
    <linearGradient id="border-grad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#7f1d1d" />
      <stop offset="30%" stop-color="#ef4444" />
      <stop offset="50%" stop-color="#ff4d6d" />
      <stop offset="70%" stop-color="#ef4444" />
      <stop offset="100%" stop-color="#7f1d1d" />
    </linearGradient>

    <!-- Filters for Neon Glow -->
    <filter id="glow-red" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="8" result="blur" />
      <feMerge>
        <feMergeNode in="blur" />
        <feMergeNode in="blur" />
        <feMergeNode in="SourceGraphic" />
      </feMerge>
    </filter>

    <filter id="ambient-blur">
      <feGaussianBlur stdDeviation="40" />
    </filter>

    <!-- Grid Pattern -->
    <pattern id="tech-grid" width="30" height="30" patternUnits="userSpaceOnUse">
      <path d="M 30 0 L 0 0 0 30" fill="none" stroke="#ef4444" stroke-width="0.75" stroke-opacity="0.08" />
    </pattern>
  </defs>

  <style>
    .title-text {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
      font-weight: 900;
      font-size: 44px;
      letter-spacing: 4px;
      text-transform: uppercase;
    }
    .subtitle-text {
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
      font-weight: 600;
      font-size: 15px;
      letter-spacing: 3px;
      text-transform: uppercase;
      fill: #e2e8f0;
    }
    .badge-text {
      font-family: "SF Pro Text", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, sans-serif;
      font-weight: 700;
      font-size: 12px;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      fill: #ff4d6d;
    }
    .pulse-dot {
      animation: pulse 2s infinite ease-in-out;
    }
    @keyframes pulse {
      0% { opacity: 0.4; r: 4px; }
      50% { opacity: 1; r: 6px; }
      100% { opacity: 0.4; r: 4px; }
    }
  </style>

  <!-- Background Rect -->
  <rect width="900" height="220" rx="14" fill="url(#bg-grad)" />

  <!-- Ambient Red Glows -->
  <circle cx="150" cy="70" r="90" fill="#dc2626" opacity="0.18" filter="url(#ambient-blur)" />
  <circle cx="750" cy="120" r="110" fill="#ff1a35" opacity="0.14" filter="url(#ambient-blur)" />

  <!-- Subtle Tech Grid -->
  <rect width="900" height="220" rx="14" fill="url(#tech-grid)" />

  <!-- Border Outline -->
  <rect x="1.5" y="1.5" width="897" height="217" rx="13" fill="none" stroke="url(#border-grad)" stroke-width="1.5" stroke-opacity="0.65" />

  <!-- Cybernetic Corner Accents -->
  <!-- Top-Left -->
  <path d="M 12 30 L 12 14 L 30 14" stroke="#ff2a45" stroke-width="3" fill="none" stroke-linecap="round" />
  <!-- Top-Right -->
  <path d="M 888 30 L 888 14 L 870 14" stroke="#ff2a45" stroke-width="3" fill="none" stroke-linecap="round" />
  <!-- Bottom-Left -->
  <path d="M 12 190 L 12 206 L 30 206" stroke="#ff2a45" stroke-width="3" fill="none" stroke-linecap="round" />
  <!-- Bottom-Right -->
  <path d="M 888 190 L 888 206 L 870 206" stroke="#ff2a45" stroke-width="3" fill="none" stroke-linecap="round" />

  <!-- Status Pill Badge at Top Center -->
  <g transform="translate(325, 24)">
    <rect width="250" height="26" rx="13" fill="#17090b" stroke="#ff2a45" stroke-width="1" stroke-opacity="0.7" />
    <circle cx="18" cy="13" r="5" fill="#ef4444" class="pulse-dot" />
    <text x="135" y="17.5" text-anchor="middle" class="badge-text">BUILDING REAL-WORLD TECH</text>
  </g>

  <!-- Main Name Header -->
  <text x="450" y="105" text-anchor="middle" class="title-text" fill="url(#red-glow-grad)" filter="url(#glow-red)">
    DEEPAK AMAL WINSTAR J
  </text>
  <text x="450" y="105" text-anchor="middle" class="title-text" fill="#ffffff" fill-opacity="0.95">
    DEEPAK AMAL WINSTAR J
  </text>

  <!-- Subtitle Tagline -->
  <text x="450" y="142" text-anchor="middle" class="subtitle-text">
    <tspan fill="#ff4d6d">COMPUTER SCIENCE ENGINEER</tspan>
    <tspan fill="#64748b"> &#8226; </tspan>
    <tspan fill="#f1f5f9">FULL STACK</tspan>
    <tspan fill="#64748b"> &#8226; </tspan>
    <tspan fill="#ff4d6d">AI &amp; IoT DEVELOPER</tspan>
  </text>

  <!-- Decorative Sleek Red Line with Diamond -->
  <g transform="translate(0, 160)">
    <line x1="200" y1="0" x2="420" y2="0" stroke="url(#border-grad)" stroke-width="1.5" stroke-opacity="0.8" />
    <polygon points="450,-5 455,0 450,5 445,0" fill="#ef4444" filter="url(#glow-red)" />
    <line x1="480" y1="0" x2="700" y2="0" stroke="url(#border-grad)" stroke-width="1.5" stroke-opacity="0.8" />
  </g>

  <!-- Secondary Meta Tags at Bottom -->
  <g transform="translate(450, 192)">
    <text text-anchor="middle" font-family="-apple-system, BlinkMacSystemFont, sans-serif" font-size="12" font-weight="600" fill="#94a3b8" letter-spacing="1.5">
      <tspan fill="#ef4444">&lt;/&gt;</tspan> TURNING RANDOM IDEAS INTO PRODUCTION CODE
    </text>
  </g>
</svg>
👋 Hi, I'm Amay Nigam
# 💫 About Me:
🔭 I’m currently working on<br>👯 I’m looking to collaborate on<br>🤝 I’m looking🚀 I’m currently working on<br>Building web development projects, AI-powered experiments, and creative digital solutions while improving my programming and development skills.<br>🤝 I’m looking to collaborate on<br>Open-source projects, AI/GenAI projects, web development, creative tech projects, hackathons, and innovative ideas that solve real-world problems.<br>💡 I’m looking for help with<br>Advanced Python, Web Development, Generative AI, APIs, Git & GitHub, cloud technologies, and turning ideas into scalable real-world projects.<br>🌱 I’m currently learning<br>Python, Generative AI, AI & Machine Learning, Web Development, Git & GitHub, Cloud Technologies, and modern development tools.<br>💬 Ask me about<br>GenAI, AI tools, prompt engineering, web development, programming, GitHub, creative editing, content creation, and my journey as a BCA student.<br>⚡ Fun fact<br>I don’t just learn technology — I love experimenting with it, turning random ideas into projects, and learning something new by building it. 🚀 for help with<br>🌱 I’m currently learning<br>💬 Ask me about<br>⚡ Fun fact


## 🌐 Socials:
[![Instagram](https://img.shields.io/badge/Instagram-%23E4405F.svg?logo=Instagram&logoColor=white)](https://instagram.com/_nigam_amay_) [![LinkedIn](https://img.shields.io/badge/LinkedIn-%230077B5.svg?logo=linkedin&logoColor=white)](https://linkedin.com/in/amaynigam) [![Mastodon](https://img.shields.io/badge/-MASTODON-%232B90D9?logo=mastodon&logoColor=white)](https://mastodon.social/@Amay Nigam) [![email](https://img.shields.io/badge/Email-D14836?logo=gmail&logoColor=white)](mailto:nigamamay@gmail.com) 

# 💻 Tech Stack:
![C](https://img.shields.io/badge/c-%2300599C.svg?style=for-the-badge&logo=c&logoColor=white) ![AssemblyScript](https://img.shields.io/badge/assembly%20script-%23000000.svg?style=for-the-badge&logo=assemblyscript&logoColor=white) ![C++](https://img.shields.io/badge/c++-%2300599C.svg?style=for-the-badge&logo=c%2B%2B&logoColor=white) ![C#](https://img.shields.io/badge/c%23-%23239120.svg?style=for-the-badge&logo=csharp&logoColor=white) ![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E) ![Java](https://img.shields.io/badge/java-%23ED8B00.svg?style=for-the-badge&logo=openjdk&logoColor=white) ![HTML5](https://img.shields.io/badge/html5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white) ![AWS](https://img.shields.io/badge/AWS-%23FF9900.svg?style=for-the-badge&logo=amazon-aws&logoColor=white) ![Codeberg](https://img.shields.io/badge/Codeberg-2185D0?style=for-the-badge&logo=Codeberg&logoColor=white) ![Datadog](https://img.shields.io/badge/datadog-%23632CA6.svg?style=for-the-badge&logo=datadog&logoColor=white) ![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=Cloudflare&logoColor=white) ![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white) ![.Net](https://img.shields.io/badge/.NET-5C2D91?style=for-the-badge&logo=.net&logoColor=white) ![Ant-Design](https://img.shields.io/badge/-AntDesign-%230170FE?style=for-the-badge&logo=ant-design&logoColor=white) ![Apache Spark](https://img.shields.io/badge/Apache%20Spark-FDEE21?style=for-the-badge&logo=apachespark&logoColor=black) ![Alpine.js](https://img.shields.io/badge/alpinejs-white.svg?style=for-the-badge&logo=alpinedotjs&logoColor=%238BC0D0) ![Anaconda](https://img.shields.io/badge/Anaconda-%2344A833.svg?style=for-the-badge&logo=anaconda&logoColor=white) ![Angular](https://img.shields.io/badge/angular-%23DD0031.svg?style=for-the-badge&logo=angular&logoColor=white) ![NestJS](https://img.shields.io/badge/nestjs-%23E0234E.svg?style=for-the-badge&logo=nestjs&logoColor=white) ![Jenkins](https://img.shields.io/badge/jenkins-%232C5263.svg?style=for-the-badge&logo=jenkins&logoColor=white) ![Apache Flink](https://img.shields.io/badge/Apache%20Flink-E6526F?style=for-the-badge&logo=Apache%20Flink&logoColor=white) ![Arango DB](https://img.shields.io/badge/ArangoDB-DDE072?style=for-the-badge&logo=arangodb&logoColor=white) ![Appwrite](https://img.shields.io/badge/Appwrite-%23FD366E.svg?style=for-the-badge&logo=appwrite&logoColor=white) ![AmazonDynamoDB](https://img.shields.io/badge/Amazon%20DynamoDB-4053D6?style=for-the-badge&logo=Amazon%20DynamoDB&logoColor=white) ![Adobe After Effects](https://img.shields.io/badge/Adobe%20After%20Effects-9999FF.svg?style=for-the-badge&logo=Adobe%20After%20Effects&logoColor=white) ![Adobe Acrobat Reader](https://img.shields.io/badge/Adobe%20Acrobat%20Reader-EC1C24.svg?style=for-the-badge&logo=Adobe%20Acrobat%20Reader&logoColor=white) ![Adobe Creative Cloud](https://img.shields.io/badge/Adobe%20Creative%20Cloud-DA1F26.svg?style=for-the-badge&logo=Adobe%20Creative%20Cloud&logoColor=white) ![Adobe InDesign](https://img.shields.io/badge/Adobe%20InDesign-49021F?style=for-the-badge&logo=adobeindesign&logoColor=FF3366) ![Adobe Dreamweaver](https://img.shields.io/badge/Adobe%20Dreamweaver-FF61F6.svg?style=for-the-badge&logo=Adobe%20Dreamweaver&logoColor=white) ![Adobe](https://img.shields.io/badge/adobe-%23FF0000.svg?style=for-the-badge&logo=adobe&logoColor=white) ![Adobe Illustrator](https://img.shields.io/badge/adobe%20illustrator-%23FF9A00.svg?style=for-the-badge&logo=adobe%20illustrator&logoColor=white) ![Adobe Lightroom Classic](https://img.shields.io/badge/Adobe%20Lightroom%20Classic-31A8FF.svg?style=for-the-badge&logo=Adobe%20Lightroom%20Classic&logoColor=white) ![Aseprite](https://img.shields.io/badge/Aseprite-FFFFFF?style=for-the-badge&logo=Aseprite&logoColor=#7D929E) ![Adobe Photoshop](https://img.shields.io/badge/adobe%20photoshop-%2331A8FF.svg?style=for-the-badge&logo=adobe%20photoshop&logoColor=white) ![Adobe Premiere Pro](https://img.shields.io/badge/Adobe%20Premiere%20Pro-9999FF.svg?style=for-the-badge&logo=Adobe%20Premiere%20Pro&logoColor=white) ![Adobe XD](https://img.shields.io/badge/Adobe%20XD-470137?style=for-the-badge&logo=Adobe%20XD&logoColor=#FF61F6) ![Adobe Fonts](https://img.shields.io/badge/Adobe%20Fonts-000B1D.svg?style=for-the-badge&logo=Adobe%20Fonts&logoColor=white) ![Figma](https://img.shields.io/badge/figma-%23F24E1E.svg?style=for-the-badge&logo=figma&logoColor=white) ![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black) ![PyTorch](https://img.shields.io/badge/PyTorch-%23EE4C2C.svg?style=for-the-badge&logo=PyTorch&logoColor=white) ![CircleCI](https://img.shields.io/badge/circleci-%23161616.svg?style=for-the-badge&logo=circleci&logoColor=white) ![ChipperCI](https://img.shields.io/badge/chipperci-1e394e.svg?style=for-the-badge&logo=chipperci&logoColor=white) ![Mocha](https://img.shields.io/badge/-mocha-%238D6748?style=for-the-badge&logo=mocha&logoColor=white) ![Cypress](https://img.shields.io/badge/-cypress-%23E5E5E5?style=for-the-badge&logo=cypress&logoColor=058a5e) ![Alfred](https://img.shields.io/badge/alfred-%235C1F87.svg?style=for-the-badge&logo=alfred) ![CMake](https://img.shields.io/badge/CMake-%23008FBA.svg?style=for-the-badge&logo=cmake&logoColor=white)
# 📊 GitHub Stats:
![](https://github-readme-stats.shion.dev/api?username=nigamamay&theme=dark&hide_border=false&include_all_commits=true&count_private=false)<br/>
![](https://streak-stats.demolab.com/?user=nigamamay&theme=dark&hide_border=false)<br/>
![](https://github-readme-stats.shion.dev/api/top-langs/?username=nigamamay&theme=dark&hide_border=false&include_all_commits=true&count_private=false&layout=compact)

## 🏆 GitHub Trophies
![](https://github-profile-trophy.vercel.app/?username=nigamamay&theme=radical&no-frame=false&no-bg=true&margin-w=4)

---
[![](https://komarev.com/ghpvc/?username=nigamamay&icon=0&color=0)](https://visitcount.itsvg.in)

<!-- Proudly created with GPRM ( https://gprm.itsvg.in ) -->
