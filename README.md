# Intern-project
<div id="app">
  <form>
    <input id="inputFile" type="file" id="myFile" name="filename" />
    <input type="button" onclick="dataUpload()" name="" title="name" />
  </form>
</div>
<script type="text/javascript">
  function readFile(file) {
    const reader = new FileReader();
    reader.addEventListener('load', (event) => {
      const result = event.target.result;
      console.log(result);
    });
  }

  function dataUpload() {
    const fileInput = document.getElementById('inputFile');
    const selectedFile = fileInput.files[0];
    readFile(selectedFile);
  }
</script>
