<template>
  <transition name="modal-fade">
    <div class="modal-backdrop">
      <div class="Myform">
        <h1>Request Demo</h1>
        <div class="inp">
          <form name="regisrration" action="form.php" method="post">
            <input class="log" type="text" required placeholder="Name" name="login" />
            <input
              class="pass"
              type="email"
              required
              placeholder="Email"
              name="password"
            />
            <div class="info">
              <a href="#" @click="close">Close</a>
            </div>
            <input class="btn" type="submit" value="Request" />
          </form>
        </div>
      </div>
    </div>
  </transition>
</template>

<script lang="ts">
export default {
  name: "modalWindow",
  methods: {
    close() {
    
      this.$emit("close");
    },
  },
};
</script>
<style>
.modal-backdrop {
  position: fixed;
  top: 0; 
  bottom: 0;
  left: 0;
  right: 0;
  background-color: rgba(0, 0, 0, 0.3);
  box-sizing: border-box;
  z-index: 1000;
  /* display: flex;
  justify-content: center;
  align-items: center; */
}
.Myform {
  width: 299px; /* ширина блока */
  height: 260px; /* высота блока */
  background: #fff; /* фон блока */
  border-radius: 10px; /* закругленные углы блока */
  margin: 10% auto; /* отступ сверху и выравнивание по середине */
  box-shadow: 2px 2px 4px 0px #161715; /* тень блока */
  padding-right: 20px;
}
.Myform h1 {
  margin: 0; /* убираем отступы */
  margin-right: -20px;
  background-color: #282e28; /* фон заголовка */
  border-radius: 8px 8px 0 0; /* закругляем углы сверху */
  color: #fff; /* цвет текста */
  font-size: 14px; /* размер шрифта */
  padding: 20px; /* отступы */
  text-align: center; /* выравниваем текст по центру */
  text-transform: uppercase;
  /* все символы заглавные */
  font-size: 16px;
  font-weight: 400;
  font-family: 'Source Sans 3';

  color: #ffffff;
}
.inp {
  padding: 20px; /* отступы */
}
.log {
  border: 1px solid #dcdcdc; /* рамка */
  padding: 12px 10px; /* отступы текста */
  width: 260px; /* ширина */
  border-radius: 5px ; /* закругленные */
}
.log:focus{
  background-color: #dcdcdcd3;
}
.pass {
  border: 1px solid #dcdcdc; /* рамка */
  padding: 12px 10px; /* отступы текста */
  width: 260px; /* ширина */
  border-radius: 5px; /* закругленные углы */
}
.pass:focus{
  background-color: #dcdcdcd3;
}
.btn {
  position: relative;
  background: #282e28;
  border: none;
  border-radius: 10px;
  color: #fff;
  float: right;
  padding: 12px 20px;
  margin-top: 10px;
  margin-right: 15px;
  left: 40px;
  font-size: 16px;
  font-weight: 400;
  color: #ffffff;
  font-family: 'Source Sans 3';
  font-weight: 400;

   transition: all 200ms ease;
}
.btn:hover{
  color: #212721;
    background-color: #ffea00;
}
.info {
  width: 50px; /* ширина */
  float: left; /* выравнивание слева */
  padding-top: 20px; /* оступ сверху для текста */
}
.info a {
  color: #999; /* цвет ссылки */
  text-decoration: none; /* убираем подчеркивание */
  font-family: Arial, Helvetica, sans-serif;
}
a:hover {
  color: #ffea00; /* цвет ссылки при наведении */
}
</style>
