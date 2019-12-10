<template>
  <div class="asideArticle">
    <h2>热门文章</h2>
    <ul>
      <li>
        <a href="/">
            <span>
              <img src="../static/img/6.jpg" />
            </span>
          <p class="txt">故不积跬步，无以至千里；不积小流，无以成江海。</p>
        </a>
      </li>
      <li>
        <a href="/">
            <span>
              <img src="../static/img/6.jpg" />
            </span>
          <p class="txt">故不积跬步，无以至千里；不积小流，无以成江海。</p>
        </a>
      </li>
      <li>
      <a href="/">
            <span>
              <img src="../static/img/6.jpg" />
            </span>
        <p class="txt">故不积跬步，无以至千里；不积小流，无以成江海。</p>
      </a>
    </li>
      <li>
      <a href="/">
            <span>
              <img src="../static/img/6.jpg" />
            </span>
        <p class="txt">故不积跬步，无以至千里；不积小流，无以成江海。</p>
      </a>
    </li>
      <li>
      <a href="/">
            <span>
              <img src="../static/img/6.jpg" />
            </span>
        <p class="txt">故不积跬步，无以至千里；不积小流，无以成江海。</p>
      </a>
    </li>
      <li>
      <a href="/">
            <span>
              <img src="../static/img/6.jpg" />
            </span>
        <p class="txt">故不积跬步，无以至千里；不积小流，无以成江海。</p>
      </a>
    </li>
      <li>
      <a href="/">
            <span>
              <img src="../static/img/6.jpg" />
            </span>
        <p class="txt">故不积跬步，无以至千里；不积小流，无以成江海。</p>
      </a>
    </li>
      <li>
      <a href="/">
            <span>
              <img src="../static/img/6.jpg" />
            </span>
        <p class="txt">故不积跬步，无以至千里；不积小流，无以成江海。</p>
      </a>
    </li>
      <li>
      <a href="/">
            <span>
              <img src="../static/img/6.jpg" />
            </span>
        <p class="txt">故不积跬步，无以至千里；不积小流，无以成江海。</p>
      </a>
    </li>
      <li>
      <a href="/">
            <span>
              <img src="../static/img/6.jpg" />
            </span>
        <p class="txt">故不积跬步，无以至千里；不积小流，无以成江海。</p>
      </a>
    </li>
    </ul>
  </div>
</template>

<script>
    export default {
        name: "SlideContent"
    }
</script>

<style scoped>
  .asideArticle {
    background-color: #FAFAFA;
    padding: 0;
  }
  .asideArticle h2 {
    color: #000;
    font-size: 18px;
    font-weight: bold;
    padding: 20px 0 0;
  }
  .asideArticle ul li{
    padding: 20px 0;
    border-top: 1px solid #ebebeb;
    font-size: 14px;
    color: #555;
    line-height: 24px;
  }
  .asideArticle ul li:first-child{
    border-top: 0;
  }
  .asideArticle ul li span{
    display: inline-block;
    vertical-align: middle;
    width: 17%;
  }
  .asideArticle ul li span img{
    display: inline-block;
    width: 90%
  }
  .asideArticle ul li p.txt{
    display: inline-block;
    vertical-align: middle;
    width: 83%;
  }
  .asideArticle ul li p:hover {
    color:#555;
  }
</style>
