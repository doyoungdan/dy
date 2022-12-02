<template>
    <section class="right_contents">
        <div class="border_right">
            <div class="gray_bg_right">
                <div class="home_title">
                    <p>김도영님의 미니홈피</p>
                    <p>http://www.cyworld.com/do0_nct</p>
                </div>
                <div class="white_bg_right">
                    <div class="right_top">
                        <div class="update">
                            <p>Updated news</p>
                            <ul>
                                <li><span class="tag01">사진첩</span>제목제목제목</li>
                                <li><span class="tag02">게시판</span>제목제목제목</li>
                                <li><span class="tag02">게시판</span>제목제목제목</li>
                                <li><span class="tag01">사진첩</span>제목제목제목</li>
                            </ul>
                        </div>
                        <div class="counting">
                            <ul>
                                <li>다이어리 <span>0/0</span></li>
                                <li>사진첩 <span>0/0</span></li>
                            </ul>
                            <ul>
                                <li>게시판 <span>0/0</span></li>
                                <li>방명록 <span>0/0</span></li>
                            </ul>
                            <ul>
                                <li>&nbsp;</li>
                                <li>&nbsp;</li>
                            </ul>
                            <ul>
                                <li>&nbsp;</li>
                                <li>&nbsp;</li>
                            </ul>
                        </div>
                    </div>
                    <div>                    
                        <QStart />     
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import QStart from './Q_Start.vue'

export default {
  components: {
    QStart
  }
}
</script>