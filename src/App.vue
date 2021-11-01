<template>
  <div id="app">
     <AudioRecord />
     <RecordAudio/>
  </div>
</template>

<script>
import AudioRecord from './components/AudioRecord.vue'
import RecordAudio from './components/AudioRecordAgain.vue'
export default {
  name: 'App',
  components: {
    AudioRecord,
    RecordAudio
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
#myVideo {
  background-color: #95DDF5;
}
</style>
