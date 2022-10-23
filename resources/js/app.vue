<template>
    <div class="flex gap-5 flex-wrap flex-col">
        <h1 class="text-3xl font-bold">Convert Link:</h1>
        <input v-model="text" class="border-solid border-2 border-sky-500 rounded-lg" type="text">
        <button class="border-solid border-2 border-sky-500 rounded-lg font-bold" @click="convert()">Convert</button>
    </div>
    
</template>

<script>
export default {
    data() {
    return {
      text :""
    }
  },
  methods: {
    convert() {
        this.text = this.text.replace("www.dropbox", "dl.dropboxusercontent"); 
    },
  },
  
};
</script>
