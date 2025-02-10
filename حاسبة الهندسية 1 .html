<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>الآلة الحاسبة الهندسية المتكاملة - حساب أبعاد العتبات والقوى</title>
  <!-- استدعاء الخطوط وأيقونات Font Awesome -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css">
  <!-- خط "Cairo" لتحسين العرض -->
  <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700&display=swap">
  <!-- مكتبة Chart.js للرسم البياني -->
  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <!-- مكتبة AOS لتأثيرات الحركة -->
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.css">
  <!-- مكتبة jsPDF لتصدير النتائج إلى PDF -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/jspdf/2.5.1/jspdf.umd.min.js"></script>
  <!-- مكتبة SheetJS لتصدير النتائج إلى Excel -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/xlsx/0.18.5/xlsx.full.min.js"></script>
  <style>
    /* إعدادات الخطوط والألوان الأساسية */
    :root {
      --primary-color: #8B4513;
      --secondary-color: #1abc9c;
      --accent-color: #FFD700;
      --text-color: #333;
      --bg-gradient: linear-gradient(45deg, #654321, #8B4513, #A0522D);
    }
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }
    body {
      font-family: 'Cairo', sans-serif;
      background: var(--bg-gradient);
      background-size: 400% 400%;
      min-height: 100vh;
      position: relative;
      direction: rtl;
      color: var(--text-color);
      transition: background 0.5s, color 0.5s;
    }
    body.light-mode {
      --primary-color: #4a4a4a;
      --secondary-color: #3498db;
      --accent-color: #e67e22;
      --text-color: #333;
      --bg-gradient: linear-gradient(45deg, #f0f0f0, #fff);
      background: var(--bg-gradient);
    }
    @keyframes gradientBG {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }
    /* شاشة التحميل */
    .loader {
      position: fixed;
      top: 0; left: 0; right: 0; bottom: 0;
      background: var(--bg-gradient);
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 3000;
    }
    .loader::after {
      content: "";
      width: 50px;
      height: 50px;
      border: 5px solid var(--secondary-color);
      border-top-color: var(--accent-color);
      border-radius: 50%;
      animation: spin 1s linear infinite;
    }
    @keyframes spin { to { transform: rotate(360deg); } }
    
    /* زر تغيير النظام */
    #modeToggle {
      position: fixed;
      top: 20px;
      left: 20px;
      background: var(--secondary-color);
      color: #fff;
      border: none;
      padding: 10px 20px;
      border-radius: 5px;
      z-index: 2100;
      cursor: pointer;
      transition: background 0.3s, transform 0.3s;
    }
    #modeToggle:hover { background: #16a085; transform: scale(1.05); }
    
    /* تنسيق الحاوية الرئيسية */
    .container {
      max-width: 1200px;
      margin: 30px auto;
      padding: 30px;
      background-color: #fff;
      border-radius: 8px;
      box-shadow: 0 0 15px rgba(0,0,0,0.1);
      direction: rtl;
    }
    h1 {
      text-align: center;
      color: var(--primary-color);
      margin-bottom: 20px;
      font-size: 2.5em;
    }
    h2 {
      color: var(--primary-color);
      margin-bottom: 10px;
      border-bottom: 2px solid var(--primary-color);
      padding-bottom: 10px;
      font-size: 1.8em;
    }
    h3 {
      color: var(--secondary-color);
      margin-bottom: 10px;
      font-size: 1.6em;
    }
    label {
      display: block;
      margin-bottom: 8px;
      font-weight: bold;
    }
    input, select, button {
      width: 100%;
      padding: 10px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 4px;
      font-size: 16px;
    }
    button {
      background-color: var(--primary-color);
      color: #fff;
      cursor: pointer;
      border: none;
      transition: background 0.3s, transform 0.3s;
    }
    button:hover { background-color: var(--accent-color); transform: scale(1.02); }
    .section {
      margin-bottom: 40px;
      padding-bottom: 20px;
      border-bottom: 1px solid #eee;
    }
    .result {
      margin-top: 20px;
      padding: 20px;
      background-color: #ecf0f1;
      border-radius: 4px;
      text-align: center;
      font-size: 1.2em;
    }
    .chart-container { margin-top: 30px; }
    .export-buttons { margin-top: 20px; text-align: center; }
    .export-buttons button { margin: 5px; }
    .reset-button { background-color: #d9534f; margin-bottom: 20px; }
    .reset-button:hover { background-color: #c9302c; }
    
    /* قسم الآلة الحاسبة الهندسية */
    .calc-section {
      margin-top: 20px;
      padding: 15px;
      background-color: #f7f7f7;
      border: 1px solid #ddd;
      border-radius: 5px;
    }
    
    /* قسم تحليل السيناريوهات */
    #scenarioResults {
      margin-top: 20px;
      padding: 15px;
      background-color: #f7f7f7;
      border: 1px solid #ddd;
      border-radius: 5px;
    }
    #scenarioComparison {
      margin-top: 20px;
    }
    
    /* الأقسام التعليمية والتوضيحية */
    .info-section {
      margin-top: 40px;
      padding: 20px;
      background-color: #f9f9f9;
      border-radius: 8px;
      border: 1px solid #ddd;
      font-size: 1.1em;
    }
    .info-section h2 { color: var(--primary-color); margin-bottom: 10px; }
    .info-section p { margin-bottom: 10px; color: #555; line-height: 1.6; }
    .info-section ul { list-style-type: disc; margin-right: 20px; color: #555; }
    .info-section ul li { margin-bottom: 5px; }
    
    /* زر العودة للأعلى */
    #backToTop {
      position: fixed;
      bottom: 40px;
      right: 20px;
      background: var(--secondary-color);
      color: #fff;
      border: none;
      padding: 10px;
      border-radius: 50%;
      font-size: 1.5em;
      cursor: pointer;
      display: none;
      z-index: 2000;
      transition: background 0.3s;
    }
    #backToTop:hover { background: #16a085; }
    
    /* تأثير حركي للأزرار العامة */
    .btn-animate {
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .btn-animate:hover {
      transform: scale(1.05);
      box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    }
    
    /* تنسيق جدول السيناريوهات */
    #scenarioComparison table {
      width: 100%;
      border-collapse: collapse;
      margin-top: 15px;
    }
    #scenarioComparison th, #scenarioComparison td {
      border: 1px solid #ccc;
      padding: 10px;
      text-align: center;
    }
    #scenarioComparison th { background-color: var(--primary-color); color: #fff; }
  </style>
</head>
<body>
  <!-- شاشة التحميل -->
  <div id="loader" class="loader"></div>
  
  <div class="container">
    <h1>الآلة الحاسبة الهندسية المتكاملة</h1>
    <p style="text-align: center; color: #555;">أداة متقدمة لحساب أبعاد العتبات والقوى وتصاميم المنشآت بدقة عالية وفق المعايير الدولية.</p>
    
    <!-- نموذج إدخال البيانات -->
    <div class="section calc-section" id="dataSection" data-aos="fade-up">
      <h2>مدخلات الحساب</h2>
      <p style="color: #555; font-size: 1.1em;">
        أدخل المعطيات التالية لحساب عزم الانحناء والأبعاد المقترحة لعتبة بسيطة.
        <br>
        <small>يُحسب عزم الانحناء (M) باستخدام المعادلة: M = w × L² ⁄ n، حيث n = 8 للعتبة البسيطة و n = 10 للعتبة المستمرة.</small>
      </p>
      
      <label for="span" title="أدخل طول العتبة (المسافة بين الدعامات) بالأمتار">طول العتبة (L) بالأمتار:</label>
      <input type="number" id="span" placeholder="مثال: 6" step="0.1">
      
      <label for="uniformLoad" title="أدخل الحمل الموزع على العتبة بالكيلو نيوتن لكل متر (kN/m)">الحمل الموزع (w) بالكيلو نيوتن/م:</label>
      <input type="number" id="uniformLoad" placeholder="مثال: 10" step="0.1">
      
      <label for="allowableStress" title="أدخل مقاومة العزم المسموح بها للمادة (مثلاً 100 MPa)">مقاومة العزم المسموح بها (f) (MPa):</label>
      <input type="number" id="allowableStress" placeholder="مثال: 100" step="1" value="100">
      
      <!-- اختيار نوع العتبة -->
      <label for="beamType" title="اختر نوع العتبة: بسيطة أو مستمرة">نوع العتبة:</label>
      <select id="beamType">
        <option value="simple" selected>بسيطة</option>
        <option value="continuous">مستمرة</option>
      </select>
      
      <!-- قسم حساب التسليح المتقدم -->
      <div class="inflation-section" data-aos="fade-up">
        <label for="calcReinforcement" title="اختر إذا كنت ترغب في احتساب كمية التسليح">احتساب كمية التسليح:</label>
        <input type="checkbox" id="calcReinforcement">
        <div id="reinforcementInputs" style="display: none; margin-top:10px;">
          <label for="fy" title="أدخل قوة حديد التسليح (f_y) (مثلاً 500 MPa)">قوة حديد التسليح (f_y) (MPa):</label>
          <input type="number" id="fy" placeholder="مثال: 500" step="1" value="500">
          <label for="cover" title="أدخل سماكة غطاء الخرسانة (cover) بالمليمتر">غطاء الخرسانة (cover) (mm):</label>
          <input type="number" id="cover" placeholder="مثال: 40" step="1" value="40">
        </div>
      </div>
      
      <!-- تم حذف قسم التضخم لأنه غير مرتبط مباشرةً بالحسابات الهندسية -->
      
      <button onclick="calculateEngineering()" class="btn-animate"><i class="fas fa-calculator"></i> احسب الأبعاد والقوى</button>
      <button class="reset-button btn-animate" onclick="resetEngineeringCalculator()"><i class="fas fa-undo"></i> إعادة تعيين</button>
    </div>
    
    <!-- عرض النتائج الهندسية -->
    <div class="result" id="engResultSection" data-aos="fade-up">
      <h2>النتائج الهندسية</h2>
      <p id="momentResult"></p>
      <p id="sectionModulusResult"></p>
      <p id="recommendedDepth"></p>
      <p id="recommendedWidth"></p>
      <p id="stressResult"></p>
      <div id="reinforcementResult"></div>
      <div class="export-buttons">
        <button onclick="printResult()" class="btn-animate"><i class="fas fa-print"></i> طباعة</button>
        <button onclick="exportPDF()" class="btn-animate"><i class="fas fa-file-pdf"></i> مشاركة النتيجة</button>
        <button onclick="exportExcel()" class="btn-animate"><i class="fas fa-file-excel"></i> تصدير إلى Excel</button>
      </div>
    </div>
    
    <!-- رسم بياني لمخطط العزم على طول العتبة -->
    <div class="chart-container" data-aos="fade-up">
      <canvas id="momentChart"></canvas>
    </div>
    
    <!-- قسم تحليل السيناريوهات الهندسية -->
    <div class="section" data-aos="fade-up">
      <h2>تحليل السيناريوهات الهندسية</h2>
      <p style="color: #555;">يمكنك تجربة نسب تحميل مختلفة لتعديل الحمل الموزع، ثم حفظ السيناريو الحالي ومقارنة النتائج:</p>
      <div style="display:flex; gap:10px; margin-bottom:20px;">
        <button onclick="calculateScenario(0.8)" class="btn-animate"><i class="fas fa-percentage"></i> 80%</button>
        <button onclick="calculateScenario(1)" class="btn-animate"><i class="fas fa-percentage"></i> 100%</button>
        <button onclick="calculateScenario(1.2)" class="btn-animate"><i class="fas fa-percentage"></i> 120%</button>
      </div>
      <div id="scenarioResults"></div>
      <button onclick="saveScenario()" class="btn-animate" style="margin-top:10px;"><i class="fas fa-save"></i> حفظ السيناريو الحالي</button>
      <div id="scenarioComparison"></div>
    </div>
    
    <!-- الأقسام التعليمية والتوضيحية -->
    <div class="info-section" data-aos="fade-up">
      <h2>دليل المستخدم - شرح مفصل</h2>
      <p>تعتمد هذه الآلة الحاسبة الهندسية على معادلات هندسية مبسطة لتقدير عزم الانحناء والأبعاد المطلوبة لعتبة بسيطة تحت حمل موزع موحد. فيما يلي شرح تفصيلي لكل خطوة:</p>
      <ul>
        <li><strong>حساب عزم الانحناء (M):</strong> تُحسب المعادلة M = w × L² ⁄ n حيث n = 8 للعتبة البسيطة و n = 10 للعتبة المستمرة. يُحول الناتج إلى N·mm بضربه في 1,000,000.</li>
        <li><strong>حساب المطلب المقطعي المطلوب (S_req):</strong> يُحسب S_req = M_Nmm / f، حيث f هي مقاومة العزم بوحدة MPa (1 MPa = 1 N/mm²).</li>
        <li><strong>تصميم المقطع:</strong> مع افتراض مقطع مستطيلي حيث b = 0.4 × d، يكون المطلب المقطعي للمقطع: S = 0.06667 × d³. لذا يكون d = cubeRoot(S_req / 0.06667) و b = 0.4 × d.</li>
        <li><strong>حساب الإجهاد الناتج (σ):</strong> يُحسب σ = M_Nmm / ((b × d²)/6).</li>
        <li><strong>حساب كمية التسليح (اختياري):</strong> إذا تم تفعيل خيار التسليح، تُحسب مساحة التسليح المطلوبة باستخدام: Aₛ = M_Nmm / (0.87 × f_y × (d - cover))، حيث f_y هو قوة حديد التسليح (MPa) و cover هو سماكة غطاء الخرسانة (mm).</li>
        <li><strong>رسم مخطط العزم:</strong> يُحسب توزيع العزم على طول العتبة باستخدام معادلة مبسطة: M(x) = w × x × (L - x) / 2، ويتم رسم المخطط باستخدام Chart.js.</li>
        <li><strong>تحليل السيناريوهات:</strong> يمكنك تجربة نسب تحميل مختلفة (80%، 100%، 120%) عن طريق تعديل الحمل الموزع مؤقتاً، ثم حفظ السيناريو الحالي وعرض جدول مقارنة للسيناريوهات المحفوظة.</li>
        <li><strong>التصدير والطباعة:</strong> توجد أزرار لتصدير النتائج إلى PDF أو Excel أو طباعتها مباشرةً.</li>
      </ul>
      <p>هذه الآلة الحاسبة تعتبر أداة أولية لتقديرات التصميم، وينبغي استخدامها مع التحليلات التفصيلية في مراحل التصميم النهائية.</p>
    </div>
    
    <div class="info-section" data-aos="fade-up">
      <h2>المعايير الدولية وأهمية التصميم الهندسي</h2>
      <p>تستند تصاميم المنشآت على معايير دولية دقيقة لضمان السلامة الهيكلية وكفاءة استخدام المواد، مما يقلل من المخاطر ويحقق الأداء الأمثل.</p>
    </div>
    
  </div>
  
  <!-- زر العودة للأعلى -->
  <button id="backToTop" title="العودة للأعلى" aria-label="العودة للأعلى">↑</button>
  
  <!-- الفوتر (يظهر مرة واحدة فقط) -->
  <footer style="background: #333; color: #ccc; padding: 20px; text-align: center; direction: rtl; margin-top: 40px;">
    <p style="margin-bottom: 10px;">© 2024 منصة الاتحاد العام للمقاولين اليمنيين - جميع الحقوق محفوظة</p>
    <p>
      <a href="https://guyc-yemen.com/" style="color: var(--accent-color); text-decoration: none;">الموقع الرسمي</a> |
      <a href="mailto:info@guyc-ye.com" style="color: var(--accent-color); text-decoration: none;">البريد الإلكتروني</a> |
      <a href="tel:01450553" style="color: var(--accent-color); text-decoration: none;">01-450553</a>
    </p>
    <p style="margin-top: 10px;">
      <a href="#" style="color: var(--accent-color); margin: 0 5px; text-decoration: none;"><i class="fab fa-facebook"></i></a>
      <a href="#" style="color: var(--accent-color); margin: 0 5px; text-decoration: none;"><i class="fab fa-twitter"></i></a>
      <a href="#" style="color: var(--accent-color); margin: 0 5px; text-decoration: none;"><i class="fab fa-youtube"></i></a>
      <a href="#" style="color: var(--accent-color); margin: 0 5px; text-decoration: none;"><i class="fab fa-whatsapp"></i></a>
    </p>
  </footer>
  
  <!-- استدعاء مكتبة AOS -->
  <script src="https://cdn.jsdelivr.net/npm/aos@2.3.4/dist/aos.js"></script>
  <script>
    window.addEventListener('load', () => {
      AOS.init();
      document.getElementById('loader').style.display = 'none';
      loadInputs();
    });
  </script>
  
  <!-- دوال الآلة الحاسبة الهندسية -->
  <script>
    // حفظ البيانات في localStorage
    function saveInputs() {
      const inputs = {
        projectName: document.getElementById('projectName').value,
        totalCost: document.getElementById('totalCost').value,
        exchangeRate: document.getElementById('exchangeRate').value,
        buildingType: document.getElementById('buildingType').value,
        buildingUsage: document.getElementById('buildingUsage').value,
        financingType: document.getElementById('financingType').value,
        financingPercent: document.getElementById('financingPercent').value,
        annualRevenue: document.getElementById('annualRevenue').value,
        annualExpenses: document.getElementById('annualExpenses').value,
        interestRate: document.getElementById('interestRate').value,
        projectDuration: document.getElementById('projectDuration').value
      };
      localStorage.setItem('engCalcInputs', JSON.stringify(inputs));
    }
    
    // استعادة البيانات من localStorage
    function loadInputs() {
      const saved = localStorage.getItem('engCalcInputs');
      if (saved) {
        const inputs = JSON.parse(saved);
        document.getElementById('projectName').value = inputs.projectName || "";
        document.getElementById('totalCost').value = inputs.totalCost || "";
        document.getElementById('exchangeRate').value = inputs.exchangeRate || "250";
        document.getElementById('buildingType').value = inputs.buildingType || "residential";
        document.getElementById('buildingUsage').value = inputs.buildingUsage || "residential";
        document.getElementById('financingType').value = inputs.financingType || "bankLoan";
        document.getElementById('financingPercent').value = inputs.financingPercent || "30";
        document.getElementById('annualRevenue').value = inputs.annualRevenue || "";
        document.getElementById('annualExpenses').value = inputs.annualExpenses || "";
        document.getElementById('interestRate').value = inputs.interestRate || "8";
        document.getElementById('projectDuration').value = inputs.projectDuration || "10";
      }
    }
    
    // زر تحديث سعر الصرف من API
    function updateExchangeRate() {
      fetch("https://api.exchangerate-api.com/v4/latest/USD")
        .then(response => response.json())
        .then(data => {
          if(data && data.rates && data.rates["YER"]) {
            const rate = data.rates["YER"];
            document.getElementById("exchangeRate").value = rate;
            alert("تم تحديث سعر الصرف: " + rate);
            saveInputs();
          } else {
            alert("تعذر الحصول على سعر الصرف.");
          }
        })
        .catch(err => alert("فشل تحديث سعر الصرف: " + err));
    }
    
    // استخدام debounce لتحديث النتائج تلقائياً
    const inputFields = document.querySelectorAll('#dataSection input, #dataSection select');
    let debounceTimer;
    inputFields.forEach(field => {
      field.addEventListener('input', () => {
        clearTimeout(debounceTimer);
        debounceTimer = setTimeout(() => {
          calculateEngineering();
          saveInputs();
        }, 500);
      });
    });
    
    // دالة حساب الآلة الحاسبة الهندسية
    function calculateEngineering() {
      const L = parseFloat(document.getElementById('span').value); // طول العتبة (م)
      const w = parseFloat(document.getElementById('uniformLoad').value); // الحمل الموزع (kN/m)
      const f = parseFloat(document.getElementById('allowableStress').value); // f (MPa)
      
      // اختيار نوع العتبة
      const beamType = document.getElementById('beamType').value;
      let momentFactor = (beamType === "simple") ? 8 : 10;
      
      if (!L || L <= 0 || !w || w <= 0 || !f || f <= 0) {
        return;
      }
      
      // حساب عزم الانحناء الأقصى: M = w × L² / momentFactor (kN·m)
      let M = (w * Math.pow(L, 2)) / momentFactor;
      let M_Nmm = M * 1e6; // تحويل إلى N·mm
      
      // حساب المطلب المقطعي المطلوب: S_req = M_Nmm / f
      let S_req = M_Nmm / f;
      
      // حساب الأبعاد المطلوبة للمقطع المستطيل:
      // مع افتراض b = 0.4 × d، يكون S = 0.06667 × d³، إذن: d = cubeRoot(S_req / 0.06667)
      let d = Math.cbrt(S_req / 0.06667);
      let b = 0.4 * d;
      
      // حساب الإجهاد الناتج: σ = M_Nmm / ((b * d²)/6)
      let sigma = M_Nmm / ((b * Math.pow(d, 2)) / 6);
      
      // تحديث النتائج في القسم المخصص
      document.getElementById('momentResult').innerText = "عزم الانحناء الأقصى (M): " + M.toFixed(2) + " kN·m";
      document.getElementById('sectionModulusResult').innerText = "المطلب المقطعي المطلوب (S_req): " + S_req.toFixed(0) + " mm³";
      document.getElementById('recommendedDepth').innerText = "العمق المقترح (d): " + d.toFixed(0) + " mm";
      document.getElementById('recommendedWidth').innerText = "العرض المقترح (b): " + b.toFixed(0) + " mm";
      document.getElementById('stressResult').innerText = "الإجهاد الناتج (σ): " + sigma.toFixed(2) + " N/mm²";
      
      // حساب كمية التسليح إذا تم تفعيل الخيار
      if(document.getElementById('calcReinforcement') && document.getElementById('calcReinforcement').checked) {
        const fy = parseFloat(document.getElementById('fy').value);
        const cover = parseFloat(document.getElementById('cover').value);
        let d_eff = d - cover;
        // حساب مساحة التسليح المطلوبة: Aₛ = M_Nmm / (0.87 * fy * d_eff)
        let A_s = M_Nmm / (0.87 * fy * d_eff);
        document.getElementById('reinforcementResult').innerText = "مساحة التسليح المطلوبة (Aₛ): " + A_s.toFixed(0) + " mm²";
      } else {
        document.getElementById('reinforcementResult').innerText = "";
      }
      
      // تحديث الرسم البياني لمخطط العزم على طول العتبة
      updateMomentChart(L, w, momentFactor);
      
      // تحديث قسم السيناريو الأساسي
      updateScenarioResult(
        "عزم الانحناء: " + M.toFixed(2) + " kN·m",
        "S_req: " + S_req.toFixed(0) + " mm³",
        "d: " + d.toFixed(0) + " mm",
        "b: " + b.toFixed(0) + " mm",
        "السيناريو الأساسي"
      );
    }
    
    // تحديث الرسم البياني لمخطط العزم باستخدام Chart.js
    let momentChartInstance;
    function updateMomentChart(L, w, momentFactor) {
      const ctx = document.getElementById('momentChart').getContext('2d');
      let labels = [];
      let dataPoints = [];
      const numPoints = 50;
      for (let i = 0; i <= numPoints; i++) {
        let x = (L / numPoints) * i;
        labels.push(x.toFixed(2) + " م");
        // معادلة توزيع العزم: M(x) = w × x × (L - x) / 2 (kN·m)
        let Mx = (w * x * (L - x)) / 2;
        dataPoints.push(Mx);
      }
      if(momentChartInstance) {
        momentChartInstance.data.labels = labels;
        momentChartInstance.data.datasets[0].data = dataPoints;
        momentChartInstance.update();
      } else {
        momentChartInstance = new Chart(ctx, {
          type: 'line',
          data: {
            labels: labels,
            datasets: [{
              label: "مخطط العزم (kN·m)",
              data: dataPoints,
              backgroundColor: 'rgba(26,188,156,0.3)',
              borderColor: 'rgba(26,188,156,1)',
              borderWidth: 2,
              fill: true,
              tension: 0.3
            }]
          },
          options: {
            responsive: true,
            animation: { duration: 1500, easing: 'easeOutQuart' },
            scales: { y: { beginAtZero: true } }
          }
        });
      }
    }
    
    // متغير لتخزين معامل الحمل الحالي في السيناريو (افتراضي 1)
    var currentLoadFactor = 1;
    
    // دالة تحليل السيناريوهات: تُعدل قيمة الحمل الموزع مؤقتًا وتعيد الحساب
    function calculateScenario(loadFactor) {
      currentLoadFactor = loadFactor;
      let baseUniformLoad = parseFloat(document.getElementById('uniformLoad').value);
      let modifiedLoad = baseUniformLoad * loadFactor;
      // حفظ القيمة الأصلية ثم تعديلها مؤقتاً
      document.getElementById('uniformLoad').value = modifiedLoad;
      calculateEngineering();
      // إعداد عرض نتائج السيناريو
      let scenarioText = `<h3>سيناريو تحميل بنسبة ${loadFactor * 100}%</h3>
        <p><strong>${document.getElementById('momentResult').innerText}</strong></p>
        <p><strong>${document.getElementById('sectionModulusResult').innerText}</strong></p>
        <p><strong>${document.getElementById('recommendedDepth').innerText}</strong></p>
        <p><strong>${document.getElementById('recommendedWidth').innerText}</strong></p>
        <p><strong>${document.getElementById('stressResult').innerText}</strong></p>`;
      document.getElementById('scenarioResults').innerHTML = scenarioText;
      // استعادة قيمة الحمل الأصلية
      document.getElementById('uniformLoad').value = baseUniformLoad;
    }
    
    // تحديث عرض نتائج السيناريو الأساسي
    function updateScenarioResult(momentVal, S_reqVal, dVal, bVal, scenarioName) {
      const scenarioDiv = document.getElementById('scenarioResults');
      scenarioDiv.innerHTML = `
        <h3>${scenarioName}</h3>
        <p><strong>${momentVal}</strong></p>
        <p><strong>${S_reqVal}</strong></p>
        <p><strong>${dVal}</strong></p>
        <p><strong>${bVal}</strong></p>
      `;
    }
    
    // حفظ السيناريو الحالي للمقارنة
    let savedScenarios = [];
    function saveScenario() {
      const scenario = {
        projectName: document.getElementById('projectName').value || "المشروع غير محدد",
        loadFactor: currentLoadFactor,
        moment: document.getElementById('momentResult').innerText,
        sectionModulus: document.getElementById('sectionModulusResult').innerText,
        depth: document.getElementById('recommendedDepth').innerText,
        width: document.getElementById('recommendedWidth').innerText,
        stress: document.getElementById('stressResult').innerText,
        timestamp: new Date().toLocaleString()
      };
      savedScenarios.push(scenario);
      updateScenarioComparison();
    }
    
    // عرض مقارنة السيناريوهات المحفوظة
    function updateScenarioComparison() {
      const compDiv = document.getElementById('scenarioComparison');
      if (savedScenarios.length === 0) {
        compDiv.innerHTML = "<p>لا توجد سيناريوهات محفوظة.</p>";
        return;
      }
      let tableHTML = `<table>
                          <thead>
                            <tr style="background-color: var(--primary-color); color: #fff;">
                              <th style="padding: 10px;">التاريخ</th>
                              <th style="padding: 10px;">نسبة التحميل</th>
                              <th style="padding: 10px;">عزم الانحناء</th>
                              <th style="padding: 10px;">S_req</th>
                              <th style="padding: 10px;">d</th>
                              <th style="padding: 10px;">b</th>
                              <th style="padding: 10px;">الإجهاد</th>
                            </tr>
                          </thead>
                          <tbody>`;
      savedScenarios.forEach(scn => {
        tableHTML += `<tr>
                        <td style="padding: 10px;">${scn.timestamp}</td>
                        <td style="padding: 10px;">${scn.loadFactor * 100}%</td>
                        <td style="padding: 10px;">${scn.moment}</td>
                        <td style="padding: 10px;">${scn.sectionModulus}</td>
                        <td style="padding: 10px;">${scn.depth}</td>
                        <td style="padding: 10px;">${scn.width}</td>
                        <td style="padding: 10px;">${scn.stress}</td>
                      </tr>`;
      });
      tableHTML += `</tbody></table>`;
      compDiv.innerHTML = `<h3>مقارنة السيناريوهات المحفوظة</h3>` + tableHTML;
    }
    
    // تصدير النتائج إلى PDF باستخدام jsPDF
    function exportPDF() {
      const { jsPDF } = window.jspdf;
      const doc = new jsPDF("p", "mm", "a4");
      doc.setFont("Arial", "normal");
      doc.text("تقرير الآلة الحاسبة الهندسية المتكاملة", 20, 20);
      const results = document.getElementById("engResultSection").innerText;
      doc.text(results, 20, 40);
      doc.text("يرجى مراجعة باقي الأقسام للحصول على التفاصيل الكاملة.", 20, 60);
      doc.save("تقرير_الآلة_الحاسبة_الهندسية.pdf");
    }
    
    // تصدير النتائج إلى Excel باستخدام SheetJS
    function exportExcel() {
      let data = [
        ["عزم الانحناء", document.getElementById('momentResult').innerText],
        ["المطلب المقطعي (S_req)", document.getElementById('sectionModulusResult').innerText],
        ["العمق المقترح (d)", document.getElementById('recommendedDepth').innerText],
        ["العرض المقترح (b)", document.getElementById('recommendedWidth').innerText],
        ["الإجهاد", document.getElementById('stressResult').innerText]
      ];
      let ws = XLSX.utils.aoa_to_sheet(data);
      let wb = XLSX.utils.book_new();
      XLSX.utils.book_append_sheet(wb, ws, "النتائج");
      XLSX.writeFile(wb, "تقرير_الآلة_الحاسبة_الهندسية.xlsx");
    }
    
    // دالة الطباعة
    function printResult() {
      window.print();
    }
    
    // دالة إعادة تعيين الحقول للآلة الحاسبة الهندسية
    function resetEngineeringCalculator() {
      document.getElementById('projectName').value = "";
      document.getElementById('totalCost').value = "";
      document.getElementById('exchangeRate').value = "250";
      document.getElementById('buildingType').selectedIndex = 0;
      document.getElementById('buildingUsage').selectedIndex = 0;
      document.getElementById('financingType').selectedIndex = 0;
      document.getElementById('financingPercent').value = "30";
      document.getElementById('annualRevenue').value = "";
      document.getElementById('annualExpenses').value = "";
      document.getElementById('interestRate').value = "8";
      document.getElementById('projectDuration').value = "10";
      if(document.getElementById('useInflation')) {
        document.getElementById('useInflation').checked = false;
      }
      if(document.getElementById('inflationRate')) {
        document.getElementById('inflationRate').value = "3";
      }
      // إعادة تعيين مدخلات الحساب الهندسي
      document.getElementById('span').value = "";
      document.getElementById('uniformLoad').value = "";
      document.getElementById('allowableStress').value = "100";
      if(document.getElementById('beamType')) {
        document.getElementById('beamType').selectedIndex = 0;
      }
      // إعادة تعيين قسم التسليح (إذا موجود)
      if(document.getElementById('calcReinforcement')) {
        document.getElementById('calcReinforcement').checked = false;
      }
      if(document.getElementById('reinforcementInputs')) {
        document.getElementById('reinforcementInputs').style.display = "none";
      }
      if(document.getElementById('fy')) {
        document.getElementById('fy').value = "500";
      }
      if(document.getElementById('cover')) {
        document.getElementById('cover').value = "40";
      }
      document.getElementById('engResultSection').innerHTML = "<h2>النتائج الهندسية</h2>";
      if(momentChartInstance) {
        momentChartInstance.destroy();
      }
      document.getElementById('sensitivityTable').querySelector("tbody").innerHTML = "";
      document.getElementById('scenarioResults').innerHTML = "";
      document.getElementById('scenarioComparison').innerHTML = "";
      savedScenarios = [];
      saveInputs();
    }
    
    // إظهار/إخفاء مدخلات التسليح عند تفعيل الخيار
    if(document.getElementById('calcReinforcement')) {
      document.getElementById('calcReinforcement').addEventListener('change', function() {
        document.getElementById('reinforcementInputs').style.display = this.checked ? "block" : "none";
      });
    }
  </script>
</body>
</html>
