<script lang="ts">
  async function sumbit() {
    const response = await fetch('http://localhost:3000', {
      method: 'GET',
    });
    const data = await response.json();
    console.log(data);
  }
</script>

<button on:click={sumbit}> Отправить </button>
