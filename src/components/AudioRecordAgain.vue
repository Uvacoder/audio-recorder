<template>
  <div>
    <audio-recorder
      v-if="showRecorder"
      upload-url="https://jsonplaceholder.typicode.com/todos"
      filename="hasaskaskakls"
      format="wav"
      :attempts="1"
      :time="60"
      :headers="headers"
      :before-recording="callback"
      :pause-recording="callback"
      :after-recording="callback"
      :select-record="callback"
      :before-upload="callback"
      :successful-upload="callback"
      :failed-upload="callback"
      :bit-rate="192"
      
    />
  </div>
</template>

<script>
export default {
  name: "RecordAudio",
  data() {
    return {
      mp3: "/demo/example.mp3",
      showRecorder: true,
      headers: {
        "X-Custom-Header": "some data"
      }
    };
  },
  methods: {
    callback(msg) {
      console.debug("Event: ", msg);
    },
  }
}
</script>

<style>

</style>