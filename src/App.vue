<script setup>

  function yes() { 
    const otevet1 = prompt("5 мнут тебе даю понял?", '')
    
    if(otevet1 === null) { 
      alert('вообще ахуел нажимать отмена, думаешь самый умный?)')
      return
    }

    const otevet = otevet1.trim().toLocaleLowerCase()

    if (otevet !== 'да' && otevet !== 'yes') { 
      alert('не ты вообще прихуеваший')
      return 
    }

    else { 
      alert('молодец')
    }

    return 
  }

  function no () { 
    while(true) { 
      alert ("ахуел, давно не пиздили?")
    }
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
