<template>
  <section sectionHeader>
    <header id="Header">
      <div id="divPhoto">??</div>
      <div id="headerNav">
        <nav id="nav">
          <ul id="ul">
            <li class="menu">
              <a href="#">Menu1</a>
            </li>
            <li class="menu">
              <a href="#">Menu2</a>
              <ul id="subMenu">
                <li class="subMenu">
                  <a href="#">Sub menu1</a>
                </li>
                <li class="subMenu">
                  <a href="#">Sub menu2</a>
                </li>
                <li class="subMenu">
                  <a href="#">Sub menu3</a>
                </li>
              </ul>
            </li>
            <li class="menu">
              <a href="#">Menu3</a>
            </li>
            <li class="menu">
              <a href="#">Menu4</a>
            </li>
            <li class="menu">
              <a href="#">Menu5</a>
            </li>
          </ul>
        </nav>
      </div>
      <div id="headerButton">
        <input type="button" value="Button" class="button" />
      </div>
    </header>
  </section>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "headerPage",
});
</script>

<style scoped>
#Header {
  height: 15vh;
  background-color: rgb(203, 198, 198);
  display: flex;
  justify-content: space-around;
  align-items: center;
}

#divPhoto {
  width: 10%;
  height: 100%;
  display: flex;
  align-items: center;
}

#headerPhoto {
  height: 60px;
  width: auto;
}

#headerNav {
  text-decoration: none;
}

#ul {
  width: 80%;
  height: 100%;
  padding: 0%;
  display: flex;
  align-items: center;
}

.menu {
  font-size: 25px;
  padding: 20px;
  list-style-type: none;
}

.menu ul {
  list-style-type: none;
  padding: 10px 0;
}

#nav ul ul {
  display: none;
  position: absolute;
  padding: 20px 0px;
}

#nav ul li:hover ul {
  display: block;
  background-color: rgb(203, 198, 198);
}

#nav ul ul {
  padding-left: 10px;
  padding-right: 10px;
  border-radius: 20px;
}

#nav ul ul li a {
  display: block;
}

#nav ul ul li {
  transition: background 0.3s;
}

a:hover {
  color: gray;
}

#headerButton {
  width: 10%;
  height: 100%;
  display: flex;
  align-items: center;
}

.button {
  font-size: 20px;
  padding: 10px 55px;
  border: 0px;
  border-radius: 30px;
  color: white;
  background-color: black;
}

.button:hover {
  background-color: rgba(0, 0, 0, 0.616);
}
</style>
