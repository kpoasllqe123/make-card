<!DOCTYPE html>
<html lang="ko">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>커스텀 능력 카드 제작소</title>
  <style>
    /* Global Styles */
    :root {
      --bg-color-1: #eef2f5;
      --bg-color-2: #e0e7ed;
      --panel-bg: #ffffff;
      --text-color: #2c3e50;
      --accent-color: #4a90e2;
      --border-color: #dcdfe6;
    }

    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
      font-family: 'Pretendard', 'Apple SD Gothic Neo', 'Noto Sans KR', sans-serif;
    }

    body {
      background-color: var(--bg-color-1);
      background-image: repeating-conic-gradient(
        var(--bg-color-2) 0% 25%, 
        var(--bg-color-1) 0% 50%
      );
      background-size: 32px 32px;
      color: var(--text-color);
      display: flex;
      flex-direction: column;
      align-items: center;
      min-height: 100vh;
      padding: 25px;
    }

    header {
      margin-bottom: 20px;
      text-align: center;
      background: rgba(255, 255, 255, 0.88);
      padding: 15px 30px;
      border-radius: 30px;
      box-shadow: 0 4px 15px rgba(0,0,0,0.05);
      backdrop-filter: blur(5px);
    }

    header h1 {
      font-size: 1.8rem;
      color: #1a252f;
      margin-bottom: 4px;
    }

    header p {
      font-size: 0.95rem;
      color: #7f8c8d;
    }

    .view-tabs {
      display: flex;
      gap: 10px;
      margin-bottom: 20px;
      background: rgba(255,255,255,0.9);
      padding: 6px;
      border-radius: 12px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.05);
    }

    .tab-btn {
      padding: 10px 24px;
      border: none;
      background: none;
      font-size: 1rem;
      font-weight: bold;
      color: #7f8c8d;
      cursor: pointer;
      border-radius: 8px;
      transition: all 0.2s ease;
    }

    .tab-btn.active {
      background-color: var(--accent-color);
      color: #ffffff;
      box-shadow: 0 2px 8px rgba(74, 144, 226, 0.3);
    }

    .container {
      display: flex;
      flex-wrap: wrap;
      gap: 30px;
      max-width: 1000px;
      width: 100%;
      justify-content: center;
      align-items: flex-start;
    }

    /* 패널 및 슬라이드 컨테이너 */
    .panel {
      background: var(--panel-bg);
      padding: 25px;
      border-radius: 16px;
      box-shadow: 0 8px 24px rgba(0, 0, 0, 0.08);
      flex: 1;
      min-width: 320px;
      max-width: 450px;
      border: 1px solid var(--border-color);
      overflow: hidden;
      transition: height 0.4s cubic-bezier(0.4, 0, 0.2, 1);
    }

    .form-slider-wrapper {
      position: relative;
      width: 100%;
    }

    .form-section {
      width: 100%;
      position: absolute;
      top: 0;
      left: 0;
      opacity: 0;
      pointer-events: none;
      transform: translateY(30px);
      transition: transform 0.4s cubic-bezier(0.4, 0, 0.2, 1), opacity 0.4s ease;
    }

    .form-section.active {
      position: relative;
      opacity: 1;
      pointer-events: auto;
      transform: translateY(0);
    }

    .form-group {
      margin-bottom: 18px;
    }

    .form-group label {
      display: block;
      font-size: 0.9rem;
      font-weight: 600;
      margin-bottom: 6px;
      color: #34495e;
      min-height: 20px;
    }

    .form-group input, 
    .form-group select, 
    .form-group textarea {
      width: 100%;
      padding: 10px 12px;
      border: 1px solid var(--border-color);
      border-radius: 8px;
      font-size: 0.95rem;
      background-color: #fcfcfc;
      transition: border-color 0.2s ease, box-shadow 0.2s ease;
    }

    .form-group input[type="file"] {
      padding: 8px;
      background: #fff;
    }

    .form-group input:focus, 
    .form-group select:focus, 
    .form-group textarea:focus {
      outline: none;
      border-color: var(--accent-color);
      box-shadow: 0 0 0 3px rgba(74, 144, 226, 0.15);
      background-color: #fff;
    }

    .row-flex {
      display: flex;
      gap: 10px;
    }

    .row-flex input[type="text"] {
      flex: 2;
    }

    .row-flex input[type="color"] {
      flex: 1;
      height: 42px;
      padding: 2px;
      cursor: pointer;
    }

    .color-pickers {
      display: flex;
      gap: 12px;
    }

    .color-picker-item {
      flex: 1;
    }

    .color-picker-item input[type="color"] {
      height: 40px;
      padding: 2px;
      cursor: pointer;
    }

    .btn-remove-img {
      margin-top: 6px;
      padding: 6px 12px;
      font-size: 0.8rem;
      background-color: #e74c3c;
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      display: none;
    }

    .btn-remove-img:hover {
      background-color: #c0392b;
    }

    .btn-save {
      width: 100%;
      padding: 14px;
      background-color: var(--accent-color);
      color: white;
      border: none;
      border-radius: 8px;
      font-size: 1rem;
      font-weight: bold;
      cursor: pointer;
      transition: background-color 0.2s ease, transform 0.1s ease;
      margin-top: 15px;
      box-shadow: 0 4px 12px rgba(74, 144, 226, 0.3);
    }

    .btn-save:hover {
      background-color: #357abd;
    }

    .btn-save:active {
      transform: scale(0.98);
    }

    .preview-area {
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
    }

    .preview-title {
      font-size: 0.95rem;
      font-weight: bold;
      color: #4a5568;
      margin-bottom: 12px;
      background: rgba(255,255,255,0.85);
      padding: 4px 14px;
      border-radius: 12px;
    }

    /* 3D Flip Card Container */
    .card-perspective-container {
      width: 320px;
      height: 480px;
      perspective: 1000px;
    }

    .card-flipper {
      width: 100%;
      height: 100%;
      position: relative;
      transform-style: preserve-3d;
      transition: transform 0.7s cubic-bezier(0.4, 0.2, 0.2, 1);
    }

    .card-flipper.flipped {
      transform: rotateY(180deg);
    }

    .card-face {
      width: 100%;
      height: 100%;
      position: absolute;
      top: 0;
      left: 0;
      border-radius: 18px;
      box-shadow: 0 12px 32px rgba(0,0,0,0.15);
      border: 8px solid #ffffff;
      box-sizing: border-box;
      backface-visibility: hidden;
      overflow: hidden;
      background-size: cover;
      background-position: center;
      background-repeat: no-repeat;
    }

    /* 앞면 컨텐츠 */
    #cardFrontPreview {
      background-color: #ffffff;
      padding: 20px;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
      z-index: 2;
    }

    /* 뒷면 컨텐츠 */
    #cardBackPreview {
      padding: 16px;
      display: flex;
      align-items: center;
      justify-content: center;
      transform: rotateY(180deg);
    }

    .card-border-layer {
      position: absolute;
      top: 0; left: 0; right: 0; bottom: 0;
      border: 3px solid #333;
      border-radius: 12px;
      pointer-events: none;
      margin: 6px;
    }

    .card-corner {
      position: absolute;
      display: flex;
      flex-direction: column;
      align-items: center;
      line-height: 1;
      font-weight: bold;
      z-index: 2;
    }

    .card-corner.top-left { top: 15px; left: 15px; }
    .card-corner.bottom-right { bottom: 15px; right: 15px; transform: rotate(180deg); }

    .corner-rank { font-size: 1.2rem; }
    .corner-suit { font-size: 1rem; margin-top: 2px; }
    .corner-suit-img { width: 18px; height: 18px; object-fit: contain; margin-top: 2px; }

    .card-header {
      text-align: center;
      margin-top: 15px;
      padding: 0 25px;
      z-index: 2;
    }

    .card-grade-badge {
      display: inline-block;
      font-size: 0.75rem;
      font-weight: bold;
      padding: 3px 12px;
      border-radius: 12px;
      color: #fff;
      background-color: #333;
      margin-bottom: 6px;
      letter-spacing: 1px;
      box-shadow: 0 2px 4px rgba(0,0,0,0.1);
    }

    .card-title {
      font-size: 1.3rem;
      font-weight: 800;
      word-break: keep-all;
      line-height: 1.2;
      min-height: 1.5em;
    }

    .card-art-area {
      flex: 1;
      margin: 12px 0;
      display: flex;
      align-items: center;
      justify-content: center;
      position: relative;
      border-radius: 8px;
      background-color: rgba(0,0,0,0.03);
      z-index: 2;
    }

    .card-center-suit {
      font-size: 4.5rem;
      user-select: none;
    }

    .card-center-suit-img {
      max-width: 90px;
      max-height: 90px;
      object-fit: contain;
    }

    .card-body {
      background: rgba(255, 255, 255, 0.88);
      border-radius: 8px;
      padding: 12px;
      border: 1px solid rgba(0,0,0,0.1);
      z-index: 2;
      backdrop-filter: blur(2px);
    }

    .card-effect-title {
      font-size: 0.75rem;
      font-weight: bold;
      color: #666;
      margin-bottom: 4px;
      text-transform: uppercase;
    }

    .card-description {
      font-size: 0.85rem;
      line-height: 1.4;
      color: #2c3e50;
      white-space: pre-wrap;
      word-break: break-word;
      min-height: 48px;
    }

    .card-back-inner {
      width: 100%;
      height: 100%;
      border-radius: 10px;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: space-between;
      padding: 20px 10px;
      position: relative;
      box-sizing: border-box;
    }

    .back-text {
      font-size: 0.9rem;
      font-weight: 800;
      letter-spacing: 2px;
      z-index: 2;
      text-transform: uppercase;
    }

    .back-text.bottom {
      transform: rotate(180deg);
    }

    .back-emblem-box {
      width: 90px;
      height: 90px;
      border-radius: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
      background: rgba(255, 255, 255, 0.9);
      box-shadow: 0 4px 10px rgba(0,0,0,0.15);
      z-index: 2;
    }

    .back-emblem {
      font-size: 3rem;
      line-height: 1;
    }

    #export-canvas {
      display: none;
    }
  </style>
</head>
<body>

  <header>
    <h1>나만의 커스텀 카드 제작소</h1>
    <p>카드 등급과 커스텀 문양 이미지까지 자유롭게 커스터마이징하세요.</p>
  </header>

  <div class="view-tabs">
    <button class="tab-btn active" data-tab="front">🎴 카드 앞면 편집</button>
    <button class="tab-btn" data-tab="back">🛡️ 카드 뒷면 편집</button>
  </div>

  <div class="container">
    <div class="panel" id="editorPanel">
      
      <div class="form-slider-wrapper">
        <!-- 앞면 폼 -->
        <div class="form-section active" id="frontForm">
          
          <div class="form-group">
            <label for="gradeTypeSelect">카드 등급 지정 방식</label>
            <select id="gradeTypeSelect">
              <option value="preset">기본 프리셋 등급 사용</option>
              <option value="custom">커스텀 등급 직접 만들기</option>
            </select>
          </div>

          <!-- 프리셋 등급 선택 -->
          <div class="form-group" id="presetGradeGroup">
            <label for="cardRank">카드 프리셋 등급</label>
            <select id="cardRank">
              <optgroup label="일반 등급 (숫자 카드)">
                <option value="2">2 (최하위)</option>
                <option value="5">5</option>
                <option value="7" selected>7</option>
                <option value="10">10 (숫자 최고)</option>
              </optgroup>
              <optgroup label="에픽 등급 (문양 카드)">
                <option value="J">J (Jack)</option>
                <option value="Q">Q (Queen)</option>
                <option value="K">K (King)</option>
              </optgroup>
              <optgroup label="전설 등급 (에이스)">
                <option value="A">A (Ace)</option>
              </optgroup>
              <optgroup label="레전더리 등급">
                <option value="JOKER">★ JOKER ★</option>
              </optgroup>
            </select>
          </div>

          <!-- 커스텀 등급 직접 입력 -->
          <div class="form-group" id="customGradeGroup" style="display: none;">
            <label>커스텀 등급 이름 & 배지 색상</label>
            <div class="row-flex">
              <input type="text" id="customGradeName" placeholder="예: MYTHIC / 신화">
              <input type="color" id="customGradeColor" value="#ff007f">
            </div>
          </div>

          <div class="form-group">
            <label for="suitTypeSelect">문양 방식 선택</label>
            <select id="suitTypeSelect">
              <option value="text">기본 텍스트 문양 (♠, ◆, ♥, ♣)</option>
              <option value="image">커스텀 문양 이미지 업로드</option>
            </select>
          </div>

          <div class="form-group" id="textSuitGroup">
            <label for="cardSuit">카드 문양</label>
            <select id="cardSuit">
              <option value="♠">♠ 스페이드 (Spade)</option>
              <option value="◆">◆ 다이아몬드 (Diamond)</option>
              <option value="♥">♥ 하트 (Heart)</option>
              <option value="♣">♣ 클로버 (Clover)</option>
            </select>
          </div>

          <div class="form-group" id="imageSuitGroup" style="display: none;">
            <label for="suitImageInput">커스텀 문양 이미지 선택</label>
            <input type="file" id="suitImageInput" accept="image/*">
            <button type="button" class="btn-remove-img" id="removeSuitImgBtn">문양 이미지 제거</button>
          </div>

          <div class="form-group">
            <label for="cardTitle">능력/카드 이름</label>
            <input type="text" id="cardTitle" value="" placeholder="카드 이름을 입력하세요">
          </div>

          <div class="form-group">
            <label for="cardDesc">능력 설명</label>
            <textarea id="cardDesc" rows="3" placeholder="카드의 능력을 입력하세요"></textarea>
          </div>

          <div class="form-group">
            <label for="bgImageInput">커스텀 배경 이미지 업로드</label>
            <input type="file" id="bgImageInput" accept="image/*">
            <button type="button" class="btn-remove-img" id="removeImgBtn">배경 이미지 제거 (단색으로 변경)</button>
          </div>

          <div class="color-pickers form-group">
            <div class="color-picker-item">
              <label for="bgColor">카드 배경색</label>
              <input type="color" id="bgColor" value="#ffffff">
            </div>
            <div class="color-picker-item">
              <label for="textColor">글자 & 테두리색</label>
              <input type="color" id="textColor" value="#222222">
            </div>
          </div>
        </div>

        <!-- 뒷면 폼 -->
        <div class="form-section" id="backForm">
          <div class="form-group">
            <label for="backPattern">뒷면 패턴 스타일</label>
            <select id="backPattern">
              <option value="grid">격자 (Grid)</option>
              <option value="diamond">다이아몬드 (Diamond)</option>
              <option value="lines">사선 스트라이프 (Lines)</option>
              <option value="checker">미니 체스판 (Checker)</option>
              <option value="solid">단색 패턴 없음 (Solid)</option>
            </select>
          </div>

          <div class="form-group">
            <label for="backEmblem">중앙 엠블럼 기호</label>
            <select id="backEmblem">
              <option value="★">★ (별)</option>
              <option value="♠">♠ (스페이드)</option>
              <option value="♥">♥ (하트)</option>
              <option value="◆">◆ (다이아몬드)</option>
              <option value="♣">♣ (클로버)</option>
              <option value="🛡️">🛡️ (방패)</option>
              <option value="👑">👑 (왕관)</option>
              <option value="🔮">🔮 (수정구)</option>
              <option value="⚔️">⚔️ (교차된 검)</option>
              <option value="☯">☯ (음양)</option>
            </select>
          </div>

          <div class="form-group">
            <label for="backTopText">상단/하단 라벨 텍스트</label>
            <input type="text" id="backTopText" value="CUSTOM CARD" placeholder="예: CUSTOM CARD">
          </div>

          <div class="color-pickers form-group">
            <div class="color-picker-item">
              <label for="backBgColor">뒷면 배경색</label>
              <input type="color" id="backBgColor" value="#1a252f">
            </div>
            <div class="color-picker-item">
              <label for="backPatternColor">패턴 색상</label>
              <input type="color" id="backPatternColor" value="#2c3e50">
            </div>
            <div class="color-picker-item">
              <label for="backAccentColor">테두리/엠블럼색</label>
              <input type="color" id="backAccentColor" value="#f1c40f">
            </div>
          </div>
        </div>
      </div>

      <button class="btn-save" id="saveBtn">PNG 이미지로 저장하기</button>
    </div>

    <div class="preview-area">
      <div class="preview-title" id="previewTitleLabel">실시간 카드 미리보기 (앞면)</div>
      
      <!-- 3D Card Flipper -->
      <div class="card-perspective-container">
        <div class="card-flipper" id="cardFlipper">
          
          <!-- 카드 앞면 -->
          <div class="card-face" id="cardFrontPreview">
            <div class="card-border-layer" id="borderLayer"></div>
            
            <div class="card-corner top-left">
              <span class="corner-rank" id="tlRank">7</span>
              <span class="corner-suit" id="tlSuit">♠</span>
            </div>

            <div class="card-header">
              <div class="card-grade-badge" id="gradeBadge">일반</div>
              <div class="card-title" id="previewTitle"></div>
            </div>

            <div class="card-art-area" id="artArea">
              <div class="card-center-suit" id="centerSuit">♠</div>
            </div>

            <div class="card-body">
              <div class="card-effect-title">CARD EFFECT</div>
              <div class="card-description" id="previewDesc"></div>
            </div>

            <div class="card-corner bottom-right">
              <span class="corner-rank" id="brRank">7</span>
              <span class="corner-suit" id="brSuit">♠</span>
            </div>
          </div>

          <!-- 카드 뒷면 -->
          <div class="card-face" id="cardBackPreview">
            <div class="card-back-inner" id="backInner">
              <div class="back-text" id="backTopTextDisplay">CUSTOM CARD</div>
              
              <div class="back-emblem-box" id="backEmblemBox">
                <div class="back-emblem" id="backEmblemDisplay">★</div>
              </div>
              
              <div class="back-text bottom" id="backBottomTextDisplay">CUSTOM CARD</div>
            </div>
          </div>

        </div>
      </div>

    </div>
  </div>

  <canvas id="export-canvas" width="640" height="960"></canvas>

  <script>
    const tabBtns = document.querySelectorAll('.tab-btn');
    const frontForm = document.getElementById('frontForm');
    const backForm = document.getElementById('backForm');
    const editorPanel = document.getElementById('editorPanel');
    const cardFlipper = document.getElementById('cardFlipper');
    const previewTitleLabel = document.getElementById('previewTitleLabel');
    const saveBtn = document.getElementById('saveBtn');

    let currentTab = 'front';
    let typingTimer = null;

    let customBgImageObj = null;
    let customSuitImageObj = null;

    function adjustPanelHeight(targetForm) {
      const saveBtnHeight = saveBtn.offsetHeight + 25; 
      const targetHeight = targetForm.offsetHeight + saveBtnHeight + 50; 
      editorPanel.style.height = `${targetHeight}px`;
    }

    window.addEventListener('load', () => {
      adjustPanelHeight(frontForm);
    });

    function runTypewriterEffect(targetForm) {
      if (typingTimer) clearTimeout(typingTimer);

      const labels = targetForm.querySelectorAll('label');
      const inputs = targetForm.querySelectorAll('input[type="text"], textarea');

      const elementsToAnimate = [];

      labels.forEach(label => {
        if (!label.dataset.original) label.dataset.original = label.textContent;
        elementsToAnimate.push({ el: label, text: label.dataset.original, isInput: false });
        label.textContent = '';
      });

      inputs.forEach(input => {
        if (!input.dataset.original) input.dataset.original = input.value;
        elementsToAnimate.push({ el: input, text: input.value, isInput: true });
        input.value = '';
      });

      let elemIdx = 0;
      let charIdx = 0;

      function typeNextChar() {
        if (elemIdx >= elementsToAnimate.length) return;

        const current = elementsToAnimate[elemIdx];
        
        if (charIdx < current.text.length) {
          const char = current.text.charAt(charIdx);
          if (current.isInput) {
            current.el.value += char;
          } else {
            current.el.textContent += char;
          }
          charIdx++;
          typingTimer = setTimeout(typeNextChar, 18);
        } else {
          elemIdx++;
          charIdx = 0;
          typingTimer = setTimeout(typeNextChar, 30);
        }
      }

      typeNextChar();
    }

    tabBtns.forEach(btn => {
      btn.addEventListener('click', () => {
        if (btn.classList.contains('active')) return;

        tabBtns.forEach(b => b.classList.remove('active'));
        btn.classList.add('active');
        
        currentTab = btn.dataset.tab;

        if (currentTab === 'front') {
          backForm.classList.remove('active');
          frontForm.classList.add('active');

          cardFlipper.classList.remove('flipped');
          previewTitleLabel.textContent = '실시간 카드 미리보기 (앞면)';
          
          adjustPanelHeight(frontForm);
          runTypewriterEffect(frontForm);
        } else {
          frontForm.classList.remove('active');
          backForm.classList.add('active');

          cardFlipper.classList.add('flipped');
          previewTitleLabel.textContent = '실시간 카드 미리보기 (뒷면)';
          
          adjustPanelHeight(backForm);
          runTypewriterEffect(backForm);
        }
      });
    });

    // 앞면 폼 요소들
    const gradeTypeSelect = document.getElementById('gradeTypeSelect');
    const presetGradeGroup = document.getElementById('presetGradeGroup');
    const customGradeGroup = document.getElementById('customGradeGroup');
    const customGradeName = document.getElementById('customGradeName');
    const customGradeColor = document.getElementById('customGradeColor');

    const suitTypeSelect = document.getElementById('suitTypeSelect');
    const textSuitGroup = document.getElementById('textSuitGroup');
    const imageSuitGroup = document.getElementById('imageSuitGroup');
    const suitImageInput = document.getElementById('suitImageInput');
    const removeSuitImgBtn = document.getElementById('removeSuitImgBtn');

    const rankSelect = document.getElementById('cardRank');
    const suitSelect = document.getElementById('cardSuit');
    const titleInput = document.getElementById('cardTitle');
    const descInput = document.getElementById('cardDesc');
    const bgColorInput = document.getElementById('bgColor');
    const textColorInput = document.getElementById('textColor');
    const bgImageInput = document.getElementById('bgImageInput');
    const removeImgBtn = document.getElementById('removeImgBtn');

    const borderLayer = document.getElementById('borderLayer');
    const gradeBadge = document.getElementById('gradeBadge');
    const previewTitle = document.getElementById('previewTitle');
    const previewDesc = document.getElementById('previewDesc');
    const centerSuit = document.getElementById('centerSuit');
    const artArea = document.getElementById('artArea');

    const tlRank = document.getElementById('tlRank');
    const tlSuit = document.getElementById('tlSuit');
    const brRank = document.getElementById('brRank');
    const brSuit = document.getElementById('brSuit');

    // 뒷면 폼 요소들
    const backPatternSelect = document.getElementById('backPattern');
    const backEmblemSelect = document.getElementById('backEmblem');
    const backTopTextInput = document.getElementById('backTopText');
    const backBgColorInput = document.getElementById('backBgColor');
    const backPatternColorInput = document.getElementById('backPatternColor');
    const backAccentColorInput = document.getElementById('backAccentColor');

    const backInner = document.getElementById('backInner');
    const backTopTextDisplay = document.getElementById('backTopTextDisplay');
    const backBottomTextDisplay = document.getElementById('backBottomTextDisplay');
    const backEmblemBox = document.getElementById('backEmblemBox');
    const backEmblemDisplay = document.getElementById('backEmblemDisplay');

    const cardFrontPreview = document.getElementById('cardFrontPreview');
    const cardBackPreview = document.getElementById('cardBackPreview');

    // 등급 유형 변경 이벤트
    gradeTypeSelect.addEventListener('change', () => {
      if (gradeTypeSelect.value === 'preset') {
        presetGradeGroup.style.display = 'block';
        customGradeGroup.style.display = 'none';
      } else {
        presetGradeGroup.style.display = 'none';
        customGradeGroup.style.display = 'block';
      }
      adjustPanelHeight(frontForm);
      updateFrontCard();
    });

    // 문양 유형 변경 이벤트
    suitTypeSelect.addEventListener('change', () => {
      if (suitTypeSelect.value === 'text') {
        textSuitGroup.style.display = 'block';
        imageSuitGroup.style.display = 'none';
      } else {
        textSuitGroup.style.display = 'none';
        imageSuitGroup.style.display = 'block';
      }
      adjustPanelHeight(frontForm);
      updateFrontCard();
    });

    // 커스텀 문양 이미지 업로드 처리
    suitImageInput.addEventListener('change', (e) => {
      const file = e.target.files[0];
      if (file) {
        const reader = new FileReader();
        reader.onload = function(evt) {
          const img = new Image();
          img.onload = function() {
            customSuitImageObj = img;
            removeSuitImgBtn.style.display = 'inline-block';
            adjustPanelHeight(frontForm);
            updateFrontCard();
          };
          img.src = evt.target.result;
        };
        reader.readAsDataURL(file);
      }
    });

    removeSuitImgBtn.addEventListener('click', () => {
      customSuitImageObj = null;
      suitImageInput.value = '';
      removeSuitImgBtn.style.display = 'none';
      adjustPanelHeight(frontForm);
      updateFrontCard();
    });

    // 배경 이미지 업로드 처리
    bgImageInput.addEventListener('change', (e) => {
      const file = e.target.files[0];
      if (file) {
        const reader = new FileReader();
        reader.onload = function(evt) {
          const img = new Image();
          img.onload = function() {
            customBgImageObj = img;
            cardFrontPreview.style.backgroundImage = `url(${evt.target.result})`;
            removeImgBtn.style.display = 'inline-block';
            adjustPanelHeight(frontForm);
          };
          img.src = evt.target.result;
        };
        reader.readAsDataURL(file);
      }
    });

    removeImgBtn.addEventListener('click', () => {
      customBgImageObj = null;
      bgImageInput.value = '';
      cardFrontPreview.style.backgroundImage = 'none';
      removeImgBtn.style.display = 'none';
      adjustPanelHeight(frontForm);
    });

    function getGradeInfo(rank) {
      if (gradeTypeSelect.value === 'custom') {
        return {
          name: customGradeName.value.trim() || 'CUSTOM',
          color: customGradeColor.value
        };
      }

      if (['2', '5', '7', '10'].includes(rank)) {
        return { name: '일반', color: '#7f8c8d' };
      } else if (['J', 'Q', 'K'].includes(rank)) {
        return { name: '에픽', color: '#2980b9' };
      } else if (rank === 'A') {
        return { name: '전설', color: '#8e44ad' };
      } else if (rank === 'JOKER') {
        return { name: '★ 레전더리 ★', color: '#e74c3c' };
      }
      return { name: '일반', color: '#333' };
    }

    function renderCornerSuit(containerEl, isImgSuit, textSuit) {
      if (isImgSuit && customSuitImageObj) {
        containerEl.innerHTML = `<img src="${customSuitImageObj.src}" class="corner-suit-img" alt="suit">`;
      } else {
        containerEl.innerHTML = textSuit;
      }
    }

    function renderCenterSuit(containerEl, isImgSuit, textSuit) {
      if (isImgSuit && customSuitImageObj) {
        containerEl.innerHTML = `<img src="${customSuitImageObj.src}" class="card-center-suit-img" alt="suit">`;
      } else {
        containerEl.innerHTML = `<div class="card-center-suit">${textSuit}</div>`;
      }
    }

    function updateFrontCard() {
      const rank = rankSelect.value;
      const textSuit = suitSelect.value;
      const isJoker = (gradeTypeSelect.value === 'preset' && rank === 'JOKER');
      const isImgSuit = (suitTypeSelect.value === 'image' && customSuitImageObj !== null);

      suitSelect.disabled = isJoker;

      const displayRank = isJoker ? 'JK' : rank;
      const displaySuitText = isJoker ? '★' : textSuit;

      tlRank.textContent = displayRank;
      brRank.textContent = displayRank;

      renderCornerSuit(tlSuit, isImgSuit, displaySuitText);
      renderCornerSuit(brSuit, isImgSuit, displaySuitText);
      renderCenterSuit(artArea, isImgSuit, displaySuitText);

      previewTitle.textContent = titleInput.value;
      previewDesc.textContent = descInput.value;

      const grade = getGradeInfo(rank);
      gradeBadge.textContent = grade.name;
      gradeBadge.style.backgroundColor = grade.color;

      const bgColor = bgColorInput.value;
      const textColor = textColorInput.value;

      cardFrontPreview.style.backgroundColor = bgColor;
      cardFrontPreview.style.color = textColor;
      borderLayer.style.borderColor = textColor;

      if (!isImgSuit) {
        const centerSuitEl = artArea.querySelector('.card-center-suit');
        if (centerSuitEl) {
          if (isJoker && (suitSelect.value === '♥' || suitSelect.value === '◆')) {
            centerSuitEl.style.color = textColor;
          } else if (textSuit === '♥' || textSuit === '◆') {
            tlSuit.style.color = '#e74c3c';
            brSuit.style.color = '#e74c3c';
            centerSuitEl.style.color = '#e74c3c';
          } else {
            tlSuit.style.color = textColor;
            brSuit.style.color = textColor;
            centerSuitEl.style.color = textColor;
          }
        }
      }
    }

    function generatePatternCSS(type, color1, color2) {
      if (type === 'grid') {
        return `linear-gradient(${color2} 2px, transparent 2px), linear-gradient(90deg, ${color2} 2px, ${color1} 2px)`;
      } else if (type === 'diamond') {
        return `repeating-linear-gradient(45deg, ${color2}, ${color2} 10px, ${color1} 10px, ${color1} 20px)`;
      } else if (type === 'lines') {
        return `repeating-linear-gradient(-45deg, ${color1}, ${color1} 8px, ${color2} 8px, ${color2} 16px)`;
      } else if (type === 'checker') {
        return `repeating-conic-gradient(${color2} 0% 25%, ${color1} 0% 50%)`;
      } else {
        return 'none';
      }
    }

    function updateBackCard() {
      const pattern = backPatternSelect.value;
      const emblem = backEmblemSelect.value;
      const textVal = backTopTextInput.value || 'CUSTOM CARD';
      const bgColor = backBgColorInput.value;
      const patternColor = backPatternColorInput.value;
      const accentColor = backAccentColorInput.value;

      cardBackPreview.style.backgroundColor = bgColor;
      cardBackPreview.style.backgroundImage = generatePatternCSS(pattern, bgColor, patternColor);
      if (pattern === 'checker' || pattern === 'grid') {
        cardBackPreview.style.backgroundSize = '20px 20px';
      } else {
        cardBackPreview.style.backgroundSize = 'auto';
      }

      backInner.style.border = `3px solid ${accentColor}`;
      backTopTextDisplay.textContent = textVal;
      backBottomTextDisplay.textContent = textVal;
      backTopTextDisplay.style.color = accentColor;
      backBottomTextDisplay.style.color = accentColor;

      backEmblemBox.style.border = `3px solid ${accentColor}`;
      backEmblemDisplay.textContent = emblem;
      backEmblemDisplay.style.color = accentColor;
    }

    [rankSelect, suitSelect, titleInput, descInput, bgColorInput, textColorInput, customGradeName, customGradeColor].forEach(elem => {
      elem.addEventListener('input', updateFrontCard);
    });

    [backPatternSelect, backEmblemSelect, backTopTextInput, backBgColorInput, backPatternColorInput, backAccentColorInput].forEach(elem => {
      elem.addEventListener('input', updateBackCard);
    });

    updateFrontCard();
    updateBackCard();

    function drawWrappedText(ctx, text, x, startY, maxWidth, lineHeight) {
      if (!text) return;
      const paragraphs = text.split('\n');
      let currentY = startY;

      paragraphs.forEach(paragraph => {
        let currentLine = '';
        const chars = Array.from(paragraph);

        for (let i = 0; i < chars.length; i++) {
          const testLine = currentLine + chars[i];
          const metrics = ctx.measureText(testLine);
          
          if (metrics.width > maxWidth && i > 0) {
            ctx.fillText(currentLine, x, currentY);
            currentLine = chars[i];
            currentY += lineHeight;
          } else {
            currentLine = testLine;
          }
        }
        if (currentLine.length > 0) {
          ctx.fillText(currentLine, x, currentY);
          currentY += lineHeight;
        }
      });
    }

    saveBtn.addEventListener('click', () => {
      const canvas = document.getElementById('export-canvas');
      const ctx = canvas.getContext('2d');
      const w = canvas.width;  
      const h = canvas.height; 

      if (currentTab === 'front') {
        const bgColor = bgColorInput.value;
        const textColor = textColorInput.value;
        const rank = rankSelect.value;
        const textSuit = suitSelect.value;
        const isJoker = (gradeTypeSelect.value === 'preset' && rank === 'JOKER');
        const isImgSuit = (suitTypeSelect.value === 'image' && customSuitImageObj !== null);

        const displayRank = isJoker ? 'JK' : rank;
        const displaySuit = isJoker ? '★' : textSuit;
        const title = titleInput.value || '';
        const desc = descInput.value || '';
        const grade = getGradeInfo(rank);

        ctx.clearRect(0, 0, w, h);

        // 배경 처리
        if (customBgImageObj) {
          ctx.save();
          ctx.beginPath();
          ctx.roundRect(0, 0, w, h, 36);
          ctx.clip();
          
          const imgRatio = customBgImageObj.width / customBgImageObj.height;
          const canvasRatio = w / h;
          let renderW, renderH, renderX, renderY;

          if (imgRatio > canvasRatio) {
            renderH = h;
            renderW = h * imgRatio;
            renderX = (w - renderW) / 2;
            renderY = 0;
          } else {
            renderW = w;
            renderH = w / imgRatio;
            renderX = 0;
            renderY = (h - renderH) / 2;
          }

          ctx.drawImage(customBgImageObj, renderX, renderY, renderW, renderH);
          ctx.restore();
        } else {
          ctx.fillStyle = bgColor;
          ctx.beginPath();
          ctx.roundRect(0, 0, w, h, 36);
          ctx.fill();
        }

        // 테두리
        ctx.strokeStyle = textColor;
        ctx.lineWidth = 6;
        ctx.beginPath();
        ctx.roundRect(16, 16, w - 32, h - 32, 24);
        ctx.stroke();

        // 좌상단 코너
        ctx.fillStyle = textColor;
        ctx.font = 'bold 36px sans-serif';
        ctx.textAlign = 'center';
        ctx.fillText(displayRank, 50, 65);
        
        if (isImgSuit) {
          ctx.drawImage(customSuitImageObj, 32, 75, 36, 36);
        } else {
          if (!isJoker && (textSuit === '♥' || textSuit === '◆')) ctx.fillStyle = '#e74c3c';
          ctx.font = '30px sans-serif';
          ctx.fillText(displaySuit, 50, 100);
        }

        // 우하단 코너
        ctx.save();
        ctx.translate(w - 50, h - 65);
        ctx.rotate(Math.PI);
        ctx.fillStyle = textColor;
        ctx.font = 'bold 36px sans-serif';
        ctx.fillText(displayRank, 0, 0);
        
        if (isImgSuit) {
          ctx.drawImage(customSuitImageObj, -18, 10, 36, 36);
        } else {
          if (!isJoker && (textSuit === '♥' || textSuit === '◆')) ctx.fillStyle = '#e74c3c';
          ctx.font = '30px sans-serif';
          ctx.fillText(displaySuit, 0, -35);
        }
        ctx.restore();

        // 등급 배지
        ctx.fillStyle = grade.color;
        ctx.beginPath();
        ctx.roundRect(w / 2 - 100, 50, 200, 36, 18);
        ctx.fill();

        ctx.fillStyle = '#ffffff';
        ctx.font = 'bold 18px sans-serif';
        ctx.textAlign = 'center';
        ctx.fillText(grade.name, w / 2, 74);

        // 카드 타이틀
        ctx.fillStyle = textColor;
        ctx.font = 'bold 42px sans-serif';
        ctx.fillText(title, w / 2, 140);

        // 중앙 영역
        ctx.fillStyle = 'rgba(0,0,0,0.03)';
        ctx.beginPath();
        ctx.roundRect(50, 180, w - 100, 400, 20);
        ctx.fill();

        if (isImgSuit) {
          const suitSize = 180;
          ctx.drawImage(
            customSuitImageObj, 
            w / 2 - suitSize / 2, 
            380 - suitSize / 2, 
            suitSize, 
            suitSize
          );
        } else {
          ctx.font = '150px sans-serif';
          if (!isJoker && (textSuit === '♥' || textSuit === '◆')) ctx.fillStyle = '#e74c3c';
          else ctx.fillStyle = textColor;
          ctx.fillText(displaySuit, w / 2, 430);
        }

        // 하단 설명 상자
        ctx.fillStyle = 'rgba(255,255,255,0.92)';
        ctx.strokeStyle = 'rgba(0,0,0,0.15)';
        ctx.lineWidth = 2;
        ctx.beginPath();
        ctx.roundRect(40, 610, w - 80, 270, 16);
        ctx.fill();
        ctx.stroke();

        ctx.fillStyle = '#666666';
        ctx.font = 'bold 20px sans-serif';
        ctx.textAlign = 'left';
        ctx.fillText('CARD EFFECT', 65, 650);

        ctx.fillStyle = '#2c3e50';
        ctx.font = '24px sans-serif';
        drawWrappedText(ctx, desc, 65, 695, w - 130, 36);

        const fileName = title.trim() ? title.replace(/\s+/g, '_') : '카드';
        const link = document.createElement('a');
        link.download = `${fileName}_앞면.png`;
        link.href = canvas.toDataURL('image/png');
        link.click();

      } else {
        const pattern = backPatternSelect.value;
        const emblem = backEmblemSelect.value;
        const textVal = backTopTextInput.value || 'CUSTOM CARD';
        const bgColor = backBgColorInput.value;
        const patternColor = backPatternColorInput.value;
        const accentColor = backAccentColorInput.value;

        ctx.clearRect(0, 0, w, h);

        ctx.fillStyle = bgColor;
        ctx.beginPath();
        ctx.roundRect(0, 0, w, h, 36);
        ctx.fill();

        ctx.save();
        ctx.beginPath();
        ctx.roundRect(0, 0, w, h, 36);
        ctx.clip();

        ctx.fillStyle = patternColor;
        if (pattern === 'grid') {
          for (let x = 0; x < w; x += 40) {
            ctx.fillRect(x, 0, 4, h);
          }
          for (let y = 0; y < h; y += 40) {
            ctx.fillRect(0, y, w, 4);
          }
        } else if (pattern === 'checker') {
          const size = 40;
          for (let x = 0; x < w; x += size) {
            for (let y = 0; y < h; y += size) {
              if ((Math.floor(x / size) + Math.floor(y / size)) % 2 === 0) {
                ctx.fillRect(x, y, size, size);
              }
            }
          }
        } else if (pattern === 'lines') {
          ctx.lineWidth = 10;
          ctx.strokeStyle = patternColor;
          for (let i = -h; i < w + h; i += 30) {
            ctx.beginPath();
            ctx.moveTo(i, 0);
            ctx.lineTo(i + h, h);
            ctx.stroke();
          }
        } else if (pattern === 'diamond') {
          ctx.lineWidth = 6;
          ctx.strokeStyle = patternColor;
          for (let i = -h; i < w + h; i += 40) {
            ctx.beginPath();
            ctx.moveTo(i, 0);
            ctx.lineTo(i + h, h);
            ctx.stroke();

            ctx.beginPath();
            ctx.moveTo(i, 0);
            ctx.lineTo(i - h, h);
            ctx.stroke();
          }
        }
        ctx.restore();

        ctx.strokeStyle = accentColor;
        ctx.lineWidth = 6;
        ctx.beginPath();
        ctx.roundRect(32, 32, w - 64, h - 64, 20);
        ctx.stroke();

        ctx.fillStyle = accentColor;
        ctx.font = 'bold 28px sans-serif';
        ctx.textAlign = 'center';
        ctx.fillText(textVal, w / 2, 85);

        ctx.save();
        ctx.translate(w / 2, h - 85);
        ctx.rotate(Math.PI);
        ctx.fillText(textVal, 0, 0);
        ctx.restore();

        ctx.fillStyle = '#ffffff';
        ctx.strokeStyle = accentColor;
        ctx.lineWidth = 6;
        ctx.beginPath();
        ctx.arc(w / 2, h / 2, 90, 0, Math.PI * 2);
        ctx.fill();
        ctx.stroke();

        ctx.fillStyle = accentColor;
        ctx.font = '90px sans-serif';
        ctx.textAlign = 'center';
        ctx.textBaseline = 'middle';
        ctx.fillText(emblem, w / 2, h / 2 + 5);

        const link = document.createElement('a');
        link.download = `${textVal.replace(/\s+/g, '_')}_뒷면.png`;
        link.href = canvas.toDataURL('image/png');
        link.click();
      }
    });
  </script>
</body>
</html>
