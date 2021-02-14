<template>
  <div
    class="nanumsquare"
    style="padding-top:15%; padding-left:10%;"
  >
    <div
      style="font-size: 24px;"
    >
      안녕하세요. 알고리즘을 좋아하는 예비 개발자 구태완입니다. <br> (키워드적으로 다시 쓰기.)
    </div>
    <br><br>
    <table
      style="font-size: 20px;"
    >
      <tr>
        <td>
          취미
        </td>
        <td>
          알고리즘, 농구, 춤, 블로그
        </td>
      </tr>
      <br>
      <tr>
        <td>
          알고리즘
        </td>
        <td>
          20년 7월 입문 <br>
          BOJ 366문제 sol : <span style="color:gold;"> Gold 2 </span> <br>
          codeforce : <span style="color:green;"> pupil </span>
        </td>
      </tr>
      <br>
      <tr>
        <td>
          연혁
        </td>
        <td>
          2013 ~ 2020 <br>
          2018 ~ 2019 <br>
          2019 ~ 2019 <br> <br>
          2020 ~ 2021
        </td>
        <td>
          부경대학교 컴퓨터공학과 <br>
          미국 교환학생 <br>
          한국정보통신학회 논문 제출 : <br>
          한글 형태소 분석을 통한 식당 키워드 추출 <br>
          삼성 청년 Software 아카데미
        </td>
      </tr>
      <br>
    </table>
    <table
      style="font-size: 20px;"
    >
      <tr>
        <td>
          주 스택
        </td>
        <td style="word-spacing: 50px;">
          Python Django Vuejs
        </td>
      </tr>
      <br>
      <tr>
        <td>
          사용해본 <br> 스택
        </td>
        <table>
          <tr>
            <td>Java</td> <td>c/c++</td> <td>JS</td> <td>React-Native</td>
          </tr>
          <tr>
            <td>Firebase</td> <td>Mysql</td> <td>Jenkins</td> <td>Git</td>
          </tr>
          <tr>
            <td>Docker</td> <td>Gradle</td> <td>JSP</td> <td>Spring-Boot</td>
          </tr>
        </table>
      </tr>
      <br>
      <tr>
        <td>
          관련 주소
        </td>
        <td>
          (버튼형식으로 깔삼하게 만들기) <br>
          <div 
            class="goto-git-event-hover"
            style="width: 150px"
            @click="openBrowser('https://github.com/fksk94')"
          > Github 바로가기</div>
          <div 
            class="goto-git-event-hover"
            style="width: 150px"
            @click="openBrowser('https://txegg.tistory.com')"
          > 블로그 바로가기</div>
        </td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name:'Info',
  methods: {
    openBrowser: function (url) {
      open(url)
    }
  }

}
</script>

<style>
.nanumsquare {
    font-family: 'NanumSquare', sans-serif !important;
}

td {
  min-width: 120px;
}

.goto-git {
  border: 1px solid;
  font-weight: bold;
}

.goto-git-event-hover:hover {
  color:blue;
  transform: scale(1.1) !important;
  transition: 0.5s ease;
  cursor: pointer;
}
</style>