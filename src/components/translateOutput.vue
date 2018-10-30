<template>
    <div id="translateOutput">
        123
        <h2>{{translatedText}}</h2>
    </div>
</template>

<script>
export default {
  name: 'translateOutput',
  props: [
    'translatedText'
  ]
}
</script>
