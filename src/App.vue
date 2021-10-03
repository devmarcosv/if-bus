<template>
<div>
  <!-- Overlay for fixed sidebar -->
<figure class="snip1336">
  <img src="https://i.pinimg.com/564x/6c/dd/21/6cdd21b01f5984494674b4b02259b4cd.jpg" alt="sample87" />
  <figcaption>
    <img src="https://i.pinimg.com/564x/c5/57/fb/c557fbfc19e9679f1779ecf009deebc1.jpg" alt="profile-sample4" class="profile" />
    <h2>Mikey Manjiro<span>Motorista</span></h2>
    <p> Tenho ansiedade.</p>
    <a href="#" class="follow">Denúnciar</a>
    <router-link to="/profile"> Mais informações </router-link>
  </figcaption>
</figure>
<figure class="snip1336 hover"><img src="https://i.pinimg.com/564x/6c/dd/21/6cdd21b01f5984494674b4b02259b4cd.jpg" alt="sample74" />
  <figcaption>
    <img src="https://i.pinimg.com/564x/c1/b2/2c/c1b22c9fecde10a4a6eff1f537f88370.jpg" alt="profile-sample2" class="profile" />
    <h2>Draken<span>Motorista</span></h2>
    <p>Linha 17.</p>
    <a href="#" class="follow">Denúnciar</a>
    <a href="#" class="info">Mais informações</a>
  </figcaption>
</figure>
<figure class="snip1336"><img src="https://i.pinimg.com/564x/6c/dd/21/6cdd21b01f5984494674b4b02259b4cd.jpg" alt="sample69" />
  <figcaption>
    <img src="https://s3-us-west-2.amazonaws.com/s.cdpn.io/331810/profile-sample5.jpg" alt="profile-sample5" class="profile" />
    <h2>Desmond Eagle<span>Accountant</span></h2>
    <p>If you want to stay dad you've got to polish your image. I think the image we need to create for you is "repentant but learning".</p>
    <a href="#" class="follow">Denúnciar</a>
    <a href="#" class="info">Mais informações</a>
  </figcaption>
</figure>
  <router-view />


</div> 
</template>
<script>
  export default {
    name: 'App',
    data: () => ({
      admins: [
        ['Management', 'mdi-account-multiple-outline'],
        ['Settings', 'mdi-cog-outline'],
      ],
      cruds: [
        ['Create', 'mdi-plus-outline'],
        ['Read', 'mdi-file-outline'],
        ['Update', 'mdi-update'],
        ['Delete', 'mdi-delete'],
      ],
    }),
  }
</script>
<style>
@import url(https://fonts.googleapis.com/css?family=Roboto:300,400,600);
.snip1336 {
  font-family: 'Roboto', Arial, sans-serif;
  position: relative;
  overflow: hidden;
  margin: 10px;
  min-width: 230px;
  max-width: 315px;
  width: 100%;
  color: #ffffff;
  text-align: left;
  line-height: 1.4em;
  background-color: #141414;
}
.snip1336 * {
  -webkit-box-sizing: border-box;
  box-sizing: border-box;
  -webkit-transition: all 0.25s ease;
  transition: all 0.25s ease;
}
.snip1336 img {
  max-width: 100%;
  vertical-align: top;
  opacity: 0.85;
}
.snip1336 figcaption {
  width: 100%;
  background-color: #141414;
  padding: 25px;
  position: relative;
}
.snip1336 figcaption:before {
  position: absolute;
  content: '';
  bottom: 100%;
  left: 0;
  width: 0;
  height: 0;
  border-style: solid;
  border-width: 55px 0 0 400px;
  border-color: transparent transparent transparent #141414;
}
.snip1336 figcaption a {
  padding: 5px;
  color: #ffffff;
  font-size: 0.7em;
  text-transform: uppercase;
  margin: 10px 0;
  display: inline-block;
  opacity: 0.65;
  width: 55%;
  text-align: center;
  text-decoration: none;
  font-weight: 600;
  letter-spacing: 1px;
}
.snip1336 figcaption a:hover {
  opacity: 1;
}
.snip1336 .profile {
  border-radius: 100%;
  position: absolute;
  bottom: 100%;
  left: 25px;
  z-index: 1;
  max-width: 75px;
  opacity: 1;
  box-shadow: 0 0 15px rgba(0, 0, 0, 0.3);
}
.snip1336 .follow {
  margin-right: 4%;
  background: red;
  color: #ffffff;
}
.snip1336 h2 {
  margin: 0 0 5px;
  font-weight: 300;
}
.snip1336 h2 span {
  display: block;
  font-size: 0.5em;
  color: #2980b9;
}
.snip1336 p {
  margin: 0 0 10px;
  font-size: 0.8em;
  letter-spacing: 1px;
  opacity: 0.8;
}

</style>