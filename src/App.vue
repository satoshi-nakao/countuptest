<template>
  <div>
  <h1>カウントアップのテストです。</h1>
  <p>以下はその手順です。</P>
  <ol>
  <li>「templateのPタグの中に{{}}回クリックされていると書く。」</li>
  <li>「buttonタグを用意する」</li>
  <li>「buttonタグの中に@clickを用意し、値にcountupを書く」</li>
  <li>「scriptにdataを用意し、returnでnumberを０で返す」</li>
  <li>「methodsを用意し、{}の中にcountupをつくりnumberがひとつずつ増えていくを記載する」</li>
  </ol>
  <p>{{number}}回クリックされている</P>
  <button @click="countup">カウントボタン</button>
  <hr>
  <button @click="reset">リセット</button>
  <hr>
  <h3>実際のコードは下記の通り</h3>
  <!-- <img src="~/assets/カウントアップ説明文1.jpg"> -->
  <img src="./assets/カウントアップ説明文2.jpg"> 
  <img src="./assets/カウントアップ説明文2.jpg">
  <hr>
  </div>
</template>

<script>


export default {
  data() {
    return {
      number : 0
    };
  },
  methods: {
    countup: function(){
      this.number += 1
    },
    reset:function(){
      this.number = 0
    }
  }
}
</script>


