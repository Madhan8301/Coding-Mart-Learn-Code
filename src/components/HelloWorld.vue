<template>
  <form class="box1">
    <form>
      <table>
        <tr>
          <td align="left">District Name &emsp;</td>
          <td align="right"><input type="text" name="first" /></td>
        </tr>
        <tr>
          <td align="left">Area (sq mt)</td>
          <td align="right"><input type="text" name="last" /></td>
        </tr>

        <tr>
          <td align="left">Population</td>
          <td align="right"><input type="text" name="email" /></td>
        </tr>
      </table>
    </form>
    <div class="wrap">
      <button class="button">SAVE</button>
    </div>
    <br /><br />
    <form class="box">
      <label>Biggest District (Area wise)<br /><br /></label>
      <input type="radio" value="Chennai" class="radio-inline" />Chennai
      <input type="radio" value="Coimbatore" class="radio-inline" />Coimbatore
      <input type="radio" value="salem" class="radio-inline" />Salem
    </form>
    <br /><br />
    <form class="box">
      Highly populated District<br /><br />
      <input type="radio" value="chennai" class="radio-inline" />Chennai
      <input type="radio" value="coimbatore" class="radio-inline" />Coimbatore
      <input type="radio" value="salem" class="radio-inline" />Salem
    </form>
  </form>
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
input[type="text"] {
  width: 200%;
  padding: 11px;
  margin: 10px 0;
  border: 0px;
  background-color: rgb(210, 211, 209);
  border-radius: 20px;
}
input:focus {
  outline: none;
}

.button {
  background-color: rgb(210, 211, 209);
  border: none;
  color: black;
  padding: 10px 32px;
  text-align: center;
  border-radius: 20px;
}
.wrap {
  text-align: center;
}
.box {
  border-style: solid;
  width: 800px;
  padding: 35px;
  text-align: left;
  font-size: 20px;
}
.box1 {
  border-style: solid;
  width: 1000px;
  padding: 35px;
  text-align: center;
  margin-top: 60px;
  margin-left: 270px;
}

input[type="radio"]:after {
  width: 200px;
  height: 10px;
  border-radius: 12px;
  top: -2px;
  left: -1px;
  position: relative;
  background-color: rgb(235, 248, 186);
  display: inline-block;
}
.radio-inline {
  margin-left: 70px;
}

input[type="radio"]:checked:after {
  width: 12px;
  height: 12px;
  border-radius: 12px;
  top: -2px;
  left: -1px;
  position: relative;
  background-color: lightgreen;
  content: "";
  border: 2px solid green;
}
</style>
