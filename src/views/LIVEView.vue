<template>
  <div class="live-view">
    <h1>FATTW 2024 Group Photo</h1>
    <div class="zoom-section">
    <img src="../assets/image/groupphotocopy.jpg" style="width:760px" alt="">
    </div>
    <h1 style="margin-top: 30px">FATTW 2024 Opening</h1>
    <div class="zoom-section">
      <video
        ref="videoPlayer"
        class="zoom-section-video"
        controls
        controlslist="nodownload"
        @contextmenu.prevent
        autoplay
        src="https://media.githubusercontent.com/media/fattw2024/fattw2024.github.io/refs/heads/main/docs/Opening.mp4?download=true"
      ></video>
    </div>
    <h1 style="margin-top: 30px">FATTW 2024 Highlights Review</h1>
    <div class="zoom-section">
      <video
        class="zoom-section-video"
        controls
        controlslist="nodownload"
        @contextmenu.prevent
        src="https://media.githubusercontent.com/media/fattw2024/fattw2024.github.io/refs/heads/main/docs/review.mp4?download=true"
      ></video>
    </div>

    <!-- <div class="schedule-section">
      <h2>Session Schedule</h2>
      <p>Our live session is scheduled for:</p>
      <p><strong>Date:</strong> TBD</p>
      <p><strong>Time:</strong> TBD (Time Zone)</p>
    </div> -->
  </div>
</template>

<script lang="ts" setup>
// 如果需要任何响应式数据或方法，可以在这里添加
// 例如：
// import { ref } from 'vue'
// const meetingId = ref('your-meeting-id')
// const passcode = ref('your-passcode')
</script>

<style scoped>
.live-view {
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  text-align: center;
  font-family: Arial, sans-serif;
}

h1 {
  color: #2c3e50;
  margin-bottom: 20px;
}

h2 {
  color: #34495e;
  margin-top: 30px;
}

.zoom-section {
  margin-top: 30px;
  background-color: #f8f8f8;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  overflow: auto;
}
.zoom-section-video {
  width: 760px;
  height: 100%;
}

.zoom-button {
  display: inline-block;
  padding: 15px 30px;
  background-color: #2d8cff;
  color: white;
  text-decoration: none;
  border-radius: 5px;
  font-weight: bold;
  margin: 20px 0;
  transition: background-color 0.3s ease, transform 0.2s ease;
}

.zoom-button:hover {
  background-color: #2681f2;
  transform: translateY(-2px);
}

.meeting-info {
  margin: 20px 0;
  font-size: 1.1em;
}

.instructions {
  font-size: 0.9em;
  color: #666;
  margin-top: 20px;
}

.schedule-section {
  margin-top: 40px;
  padding: 20px;
  background-color: #e9f7fe;
  border-radius: 8px;
}
</style>