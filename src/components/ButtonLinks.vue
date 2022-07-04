<template>
  <div class="buttons">
    <button class="invbtn" id="basebtn">
      <a href="https://discord.com/oauth2/authorize?client_id=960533661109878805&scope=bot%20applications.commands&permissions=336886885630">
        <span>Invite Nyx</span>
      </a>
    </button>
  </div>
</template>

<style scoped>
.buttons {
  display: flex;
  justify-content: center;
}

#basebtn {
  text-decoration: none;
  text-align: center;

  border: none;
  border-radius: 16px;
}

.invbtn {
  display: inline-block;
  background-color: #9edb25;

  color: white;
  padding: 14px 30px;
  font-size: 1.5rem;
  font-family: monospace;

  transition: ease 0.5;

  margin-top: -50px;
}

.invbtn span {
  cursor: pointer;
  display: inline-block;
  position: relative;
  transition: 0.5s;
}

.invbtn span:after {
  content: "→";
  position: absolute;
  opacity: 0;
  top: 0;
  right: -20px;
  transition: 0.5s;
}

.invbtn:hover span {
  padding-right: 25px;
}

.invbtn:hover span:after {
  opacity: 1;
  right: 0;
}
</style>
