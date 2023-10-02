<template>
  <link rel="stylesheet" href="/styles.css">
  <div class="portfolio">
    <h1>Welcome to my personal portfolio website!</h1>
    <p>My name is Motheo Boikhutso, and I am a student currently studying a Bachelor of Information Technology at Deakin University.</p>

    <table>
      <tr>
        <th>Languages</th>
        <th>Technologies</th>
      </tr>
      <tr>
        <td>HTML, CSS, JavaScript, Vue</td>
        <td>VS Code, Git</td>
      </tr>
    </table>
  </div>
  <footer>
    <p>&copy; Motheo Boikhutso</p>
    <p>Student ID: 218400235</p>
  </footer>
</template>

<script>

</script>

<style scoped>
  .portfolio {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    height: 100vh;
    text-align: center;
  }

  h1 {
    font-size: 2rem;
    color: #b8bfc4;
    margin-bottom: 10px;
  }

  p {
    font-size: 1.2rem;
    color: #b8bfc4;
  }

  table {
    border-collapse: collapse;
    margin-top: 20px;
    border-radius: 8px;
    box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
    width: 80%;
    background-color: #041a30;
  }

  th, td {
    padding: 12px 24px;
    text-align: left;
  }

  footer {
    margin-top: 20px;
    font-size: 14px;
    color: #b8bfc4;
    text-align: center;
  }
</style>