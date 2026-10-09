<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>スマート冷蔵庫シェフ</title>
  <style>
    body { font-family: sans-serif; background: #f5f6f8; margin: 0; padding: 16px; color: #333; }
    .box { background: #fff; border-radius: 12px; padding: 16px; margin-bottom: 14px; box-shadow: 0 2px 8px rgba(0,0,0,0.05); }
    h1 { font-size: 1.2rem; color: #e65100; margin: 0 0 8px; text-align: center; }
    .btn-mode { display: flex; gap: 8px; margin-bottom: 12px; }
    .btn-mode button { flex: 1; padding: 10px; border: 1px solid #ddd; background: #eee; border-radius: 8px; font-weight: bold; }
    .btn-mode button.active { background: #ff6f00; color: #fff; border-color: #ff6f00; }
    input[type="text"] { width: 70%; padding: 10px; border: 1px solid #ccc; border-radius: 8px; box-sizing: border-box; }
    .btn-add { width: 26%; padding: 10px; background: #ff6f00; color: #fff; border: none; border-radius: 8px; font-weight: bold; }
    .tags { display: flex; flex-wrap: wrap; gap: 6px; margin-top: 10px; }
    .tag { background: #ffe0b2; color: #e65100; padding: 4px 10px; border-radius: 16px; font-size: 0.85rem; font-weight: bold; }
    .grid { display: grid; grid-template-columns: 1fr 1fr; gap: 8px; margin-top: 8px; }
    .check-item { background: #fafafa; border: 1px solid #ddd; padding: 8px; border-radius: 6px; font-size: 0.85rem; }
    .btn-submit { width: 100%; padding: 14px; background: #e65100; color: #fff; border: none; border-radius: 12px; font-size: 1rem; font-weight: bold; margin-top: 8px; }
    .recipe-card { background: #fff; border-radius: 12px; padding: 16px; margin-top: 12px; border: 1px solid #eee; }
    .recipe-title { font-size: 1rem; font-weight: bold; color: #212121; margin-bottom: 6px; }
    .recipe-badge { display: inline-block; background: #e8f5e9; color: #2e7d32; font-size: 0.75rem; padding: 2px 6px; border-radius: 4px; margin-bottom: 6px; }
    .recipe-steps { padding-left: 20px; font-size: 0.85rem; line-height: 1.6; }
  </style>
</head>
<body>
  <h1>🍳 スマート冷蔵庫シェフ</h1>

  <div class="box">
    <div class="btn-mode">
      <button id="btnQuick" class="active" onclick="setMode('quick')">⚡ 時短 (10分)</button>
      <button id="btnGourmet" onclick="setMode('gourmet')">🥘 じっくり (25分)</button>
    </div>
    <div><strong>1. ある食材を入力</strong></div>
    <div style="display:flex; justify-content:space-between; margin-top:6px;">
      <input type="text" id="foodInput" placeholder="例: 豚肉、卵、キャベツ">
      <button class="btn-add" onclick="addFood()">追加</button>
    </div>
    <div class="tags" id="foodTags"></div>
  </div>

  <div class="box">
    <div><strong>2. 調味料（チェック式）</strong></div>
    <div class="grid">
      <label class="check-item"><input type="checkbox" id="s_soya" checked> 醤油</label>
      <label class="check-item"><input type="checkbox" id="s_mirin" checked> みりん</label>
      <label class="check-item"><input type="checkbox" id="s_sake" checked> 料理酒</label>
      <label class="check-item"><input type="checkbox" id="s_miso" checked> 味噌</label>
      <label class="check-item"><input type="checkbox" id="s_salt" checked> 塩コショウ</label>
      <label class="check-item"><input type="checkbox" id="s_oil" checked> 油・ごま油</label>
    </div>
  </div>

  <button class="btn-submit" onclick="makeRecipes()">3通りのレシピを提案！</button>
  <div id="results"></div>

  <script>
    let mode = 'quick';
    let foods = [];

    function setMode(m) {
      mode = m;
      document.getElementById('btnQuick').className = (m === 'quick' ? 'active' : '');
      document.getElementById('btnGourmet').className = (m === 'gourmet' ? 'active' : '');
    }

    function addFood() {
      const input = document.getElementById('foodInput');
      const val = input.value.trim();
      if (!val) return;
      foods.push(val);
      input.value = '';
      renderTags();
    }

    function renderTags() {
      const box = document.getElementById('foodTags');
      box.innerHTML = '';
      foods.forEach((f, i) => {
        box.innerHTML += `<span class="tag">${f} <span onclick="removeFood(${i})" style="cursor:pointer">×</span></span>`;
      });
    }

    function removeFood(i) {
      foods.splice(i, 1);
      renderTags();
    }

    function makeRecipes() {
      if (foods.length === 0) {
        alert('食材を1つ以上入力して「追加」を押してください！');
        return;
      }
      const box = document.getElementById('results');
      box.innerHTML = '';
      const main = foods[0];
      const sub = foods.length > 1 ? foods[1] : '玉ねぎや余り野菜';

      const list = [
        {
          title: mode === 'quick' ? `${main}と${sub}の甘辛スピード炒め` : `${main}と${sub}の旨味染み込む照り煮`,
          badge: mode === 'quick' ? '⚡ 10分・和風甘辛' : '🥘 25分・じっくり煮物',
          steps: mode === 'quick' 
            ? ['具材を薄切りにして火の通りを早くする。', 'フライパンで強火で2分炒める。', '醤油・みりん・酒を各大さじ1絡めて照りが出たら完成！']
            : ['具材を大きめに切って香ばしく焼き目をつける。', '水200mlと酒・みりん各大さじ2を加えて15分弱火で煮る。', '醤油大さじ2を加え、煮汁が少なくなるまでコトコト煮詰める。']
        },
        {
          title: `${main}のコク旨マヨ味噌焼き`,
          badge: mode === 'quick' ? '⚡ 12分・コク旨' : '🥘 20分・濃厚オーブン風',
          steps: ['味噌・マヨネーズ各大さじ1を混ぜておく。', 'フライパンで具材を両面しっかり焼く。', '火を止めてタレを余熱でサッと絡めて完成！']
        },
        {
          title: `${main}と${sub}のネギ塩ごま油スープ`,
          badge: '⚡ 8分・さっぱり塩味',
          steps: ['小鍋に水350mlと鶏ガラスープの素小さじ1を沸かす。', '具材を入れて3分煮る。', '塩コショウで味を調え、仕上げにごま油をひと回し！']
        }
      ];

      list.forEach((r, idx) => {
        box.innerHTML += `
          <div class="recipe-card">
            <span class="recipe-badge">${r.badge}</span>
            <div class="recipe-title">${idx + 1}. ${r.title}</div>
            <ol class="recipe-steps">${r.steps.map(s => `<li>${s}</li>`).join('')}</ol>
          </div>
        `;
      });
    }
  </script>
</body>
</html>
