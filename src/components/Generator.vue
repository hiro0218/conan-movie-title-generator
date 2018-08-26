<template>
  <div>
    <div class="result">{{ result }}</div>
    <div class="form">
      <button @click="generate">生成</button>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Generator',
  data() {
    return {
      result: '時計じかけの摩天楼',
      title: {
        head: [
          '時計じかけ',
          '14番目',
          '世紀末',
          '瞳の中',
          '天国へ',
          'ベイカー街',
          '迷宮',
          '銀翼',
          '水平線上',
          '探偵たち',
          '紺碧',
          '戦慄',
          '漆黒',
          '天空',
          '沈黙',
          '11人目',
          '絶海',
          '異次元',
          '業火',
          '純黒',
          'から紅',
          'ゼロ',
        ],
        tail: [
          '摩天楼',
          '標的',
          '魔術師',
          '暗殺者',
          'カウントダウン',
          '亡霊',
          '十字路',
          '奇術師',
          '陰謀',
          '鎮魂歌',
          '棺',
          '楽譜',
          '追跡者',
          '難破船',
          '15分',
          'ストライカー',
          '探偵',
          '狙撃手',
          '向日葵',
          '悪夢',
          '恋歌',
          '執行人',
        ],
      },
      conjunction: 'の',
    };
  },
  methods: {
    generate: function() {
      let head = this.title.head[this.getRandomInt(this.title.head.length)]
      let tail = this.title.tail[this.getRandomInt(this.title.tail.length)]

      this.result = head + this.conjunction + tail
    },
    getRandomInt: function(length) {
      return Math.floor(Math.random() * Math.floor(length));
    },
  }
}
</script>

<style scoped>
.result {
  font-size: 1.8rem;
}
</style>
