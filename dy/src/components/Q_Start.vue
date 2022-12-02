<template>
    <div class="miniroom" id="startpage" v-if="!isshow">
        <div class="mini_tit">
            <p>Mini Room</p>
            <p>START</p>
        </div>
        <div class="mini_img">
        </div>
        <div class="say_wrap">
            <p>What frirends say <span>한마디로 표현해봐~</span></p>
            <p class="notice">정답은 영문 또는 숫자로만 입력할 수 있습니다. ex.답 : 도영 > ehdud</p>
            <div class="form_control">
                <input v-model="answer0" type="text" @blur="answerValid0">
                <button v-if="!answerValidFlag">확인2</button>
                <button v-if="answerValidFlag" @click="isshow = !isshow">확인</button>
            </div>
        </div>
    </div>
    <div class="miniroom" id="stage01" v-if="isshow">
        <div class="mini_tit">
            <p>Mini Room</p>
            <p>STAGE01</p>
        </div>
        <div class="mini_img">
        </div>
        <div class="say_wrap">
            <p>What frirends say <span>한마디로 표현해봐~</span></p>
            <p class="notice">정답은 영문 또는 숫자로만 입력할 수 있습니다. ex.답 : 도영 > ehdud</p>
            <div class="form_control">
                <input v-model="answer1" type="text" @blur="answerValid1">
                <button type="button" v-if="!answerValidFlag">확인2</button>
                <button type="button" v-if="answerValidFlag" @click="Gostage02">확인</button>
            </div>
        </div>
    </div>
</template>
<script>
export default {
  data () {
    return {
      answer0: '',
      answer1: '',
      answerValidFlag: false,
      answerCheck0: 'ehekdlwptmxm',
      answerCheck1: '171028',
      isshow: false
    }
  },
  methods: {
    answerValid0 () {
      if (this.answer0 === this.answerCheck0) {
        this.answerValidFlag = true
      } else {
        this.answerValidFlag = false
      }
    },
    answerValid1 () {
      if (this.answer1 === this.answerCheck1) {
        this.answerValidFlag = true
      } else {
        this.answerValidFlag = false
      }
    }
  }
}
</script>