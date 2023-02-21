<template>
  <div class="container">
    <div class="row">
      <div class="col" v-if="isVisible">
        <label>Enter Question</label>
        <textarea class="form-control"></textarea>
        <input type="submit" class="btn btn-primary" value="Submit">
      </div>

      <button @click="toggleQuestion" class="btn btn-dark">Enter New Question</button>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      isVisible: false
    }
  },
  methods: {

    toggleQuestion() {
      this.isVisible = !this.isVisible;
    }
  }
}
</script>
