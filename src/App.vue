<template>
  <Header title='アニメトラッカー'/>
  <NameList :names="names"/>
</template>

<script>
import Header from './components/Header';
import NameList from './components/NameList';

export default {
  name: 'App',
  components: {
    Header,
    NameList,
  },
  data(){
    return {
      names: [],
    }
  },
  created(){
    this.names = [
      {
        id: 1,
        title: 'Yuji Itadori',
        nihongo: '削除'
      },
      {
        id: 2,
        title: 'Midoriya Izuku',
        nihongo: '緑谷出久'
      },
      {
        id: 3,
        title: 'Naruto Uzumaki',
        nihongo: 'うずまきナルト'
      },
      {
        id: 4,
        title: 'Licht Bach',
        nihongo: 'リヒト・バック'
      },
      {
        id: 5,
        title: 'Ichigo Kurusaki',
        nihongo: '黒崎一護'
      },
    ]
  }
}
</script>

<style>

* {
  margin: 0;
  padding: 0;
}

.btn {
  background-color: #000;
  color: #FFF;
  padding: 10px;
  margin: 5px;
  border-radius: 5px;
  border-style: none;
  font-weight: 700;
}

.btn:hover {
  box-shadow: -1px 1px 6px 3px rgba(164,156,156,1);
  -webkit-box-shadow: -1px 1px 6px 3px rgba(164,156,156,1);
  -moz-box-shadow: -1px 1px 6px 3px rgba(164,156,156,1);
}

</style>
