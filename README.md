<script>
  // 選択肢のリスト
  const drinks = [
    "生ビール",
    "カクテル",
    "ハイボール(ジャパニーズウイスキー中心)",
    "日本酒",
    "麦焼酎(ソーダ割)",
    "芋焼酎(ソーダ割)",
    "麦焼酎(ソーダ割 / 梅干し入)"
    "芋焼酎(ソーダ割 / 梅干し入)",
    "缶酎ハイ(男梅サワー)",
    "缶酎ハイ(お茶割り)",
    "缶酎ハイ(氷結)"
  ];

  // ランダムに一つ選ぶ
  const randomIndex = Math.floor(Math.random() * drinks.length);
  const resultDrink = drinks[randomIndex];

  // 結果を画面に表示
  document.addEventListener('DOMContentLoaded', (event) => {
    document.getElementById('result').textContent = `今日は山本で【${resultDrink}】！`;
  });
</script>

<h1 id="result"></h1>
