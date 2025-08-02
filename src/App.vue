<script setup>

  function yes() { 
    const otevet = prompt("5 мнут тебе даю понял?", ' ')

    if (otevet !== 'да' && otevet !== 'yes' && otevet !== 'Да') { 
      alert('не ты вообще прихуеваший')
      return 
    }
    else { 
      alert('молодец')
    }

    return 
  }

  function no () { 
    alert ("ахуел, давно не пиздили?")
    return 
  }

</script>

<template>
  <div>
    <h1 class="text">В кс пойдешь?</h1>
    <button class="yes" @click="yes"> yes my bro</button>
    <button class="no" @click="no"> no sorry</button>
  </div>
</template>

<style scoped>

</style>
