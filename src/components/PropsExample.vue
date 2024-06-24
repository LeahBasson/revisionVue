<template>
  <div>
    <p>
        <span v-if="numb1>0">
            Numb1: {{ numb1 }}
        </span>
        <span v-else>
            Please provide numb1's value
        </span>
    </p>
    <p>Numb2: {{ numb2 }}</p>
    <p>Sum: {{ addition }}</p>
  </div>
</template>

<script>
export default {
    props: ["numb1", "numb2"],
    computed: {
        addition() {
            return +this.numb1 + +this.numb2
        }
    }
}
</script>

<style scoped>

</style>