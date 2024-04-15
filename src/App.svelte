<script>
import {syntaxColoring} from "./syntaxColoring.js"
let input = ""
let output = ""

$:{
  output = syntaxColoring(input)
}

</script>

<main>
  <div class="container">
    Input:
    <textarea bind:value={input}></textarea>
  </div>
  <div class="container">
    Output:
    <textarea bind:value={output}></textarea>
  </div>
</main>

<style>
main{
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
.container{
  display: flex;
  flex-direction: column;
}
textarea{
  resize: none;
  width: calc(100% - 20px);
  height:  calc(100% - 20px);
  min-width: 800px;
  min-height: 600px;
  margin: 10px;
  outline: none;
}
</style>
