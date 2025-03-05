<script setup>
import { ref } from 'vue';

const selectedUrl = ref("");
const showModal = ref(false);
const rootRoute = "/free-bundle/";

const openInModal = (url) => {
  selectedUrl.value = url;
  showModal.value = true;
};

const closeModal = () => {
  showModal.value = false;
};
</script>

<template>
  <ol>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}001 elaadmin-master/index.html`)">001 elaadmin</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}002 applab/public/index.html`)">002 applab</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}003 jadoo/public/index.html`)">003 jadoo</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}004 laslesVPN-v1.0.0/public/index.html`)">004 laslesVPN</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}005 PurpleAdmin-Free-Admin-Template-1.0.0/index.html`)">005 PurpleAdmin</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}006 foodwagon-v1.0.0/public/index.html`)">006 foodwagon</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}007 eshopper-1.0.0/index.html`)">007 eshopper</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}008 sneat-1.0.0/index.html`)">008 sneat</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}009 skydash/index.html`)">009 skydash</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}010 little-squirrel-v1.0.0/public/index.html`)">010 little-squirrel</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}011 Zay.Shop/templatemo_559_zay_shop/index.html`)">011 Zay.Shop</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}012 titan-master/index.html`)">012 titan</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}013 karma-master/index.html`)">013 karma</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}014 original-master/index.html`)">014 original</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}015 shoppers-gh-pages/index.html`)">015 shoppers</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}016 seogram-1.0.0/html/index.html`)">016 seogram</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}017 cakezone-1.0.0/index.html`)">017 cakezone</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}018 ecohosting-main/ecohosting-main/index.html`)">018 ecohosting</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}019 foodeiblog-master/index.html`)">019 foodeiblog</a></li>
    <li><a href="#" @click.prevent="openInModal(`${rootRoute}020 softy-pinko-master/index.html`)">020 softy-pinko</a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
    <li><a href="#" @click.prevent="openInModal(``)"></a></li>
  </ol>

  <!-- Modal -->
  <div v-if="showModal" class="modal">
    <div class="modal-content">
      <span class="close" @click="closeModal">&times;</span>
      <iframe :src="selectedUrl" width="100%" height="100%"></iframe>
    </div>
  </div>
</template>

<style scoped>
 .modal {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5);
  display: flex;
  justify-content: center;
  align-items: center;
}

.modal-content {
  background: white;
  padding: 20px;
  width: 80%;
  height: 80%;
  position: relative;
}

.close {
  position: absolute;
  top: 10px;
  right: 20px;
  font-size: 24px;
  cursor: pointer;
}

ol {
  list-style: none;
}

iframe {
  width: 100%;
  height: 100%;
} 
</style>
