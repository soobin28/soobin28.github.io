---
layout: default
title: Contact Soo Bin
---

<div id="contact">
  <h1 class="pageTitle">Contact Me</h1>
  <div class="contactContent">
    <p class="intro">문의사항이 있으면 편하게 보내십셔</p>
    <p>양식제공 -> <a href="http://formspree.io/">Formspree.</a> 이 사이트 지침에 따라 사용할 양식 설정할 것.</p>

  </div>
  <form action="http://formspree.io/your@mail.com" method="POST">
    <label for="name">Name</label>
    <input type="text" id="name" name="name" class="full-width"><br>
    <label for="email">Email Address</label>
    <input type="email" id="email" name="_replyto" class="full-width"><br>
    <label for="message">Message</label>
    <textarea name="message" id="message" cols="30" rows="10" class="full-width"></textarea><br>
    <input type="submit" value="Send" class="button">
  </form>
</div>
