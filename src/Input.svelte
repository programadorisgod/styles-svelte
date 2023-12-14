<script>

    export let value;
    export let label;
    export let id;

    let invalid = false;

    function updateValue(){

      if (value.length <= 3) {
         invalid = true;
      }else{
         invalid = false;
      }

    }
</script>



<label class="label_input" for={id}>{label}</label>
<input type="text" bind:value id={id}  class:invalid class="input_app" on:keyup={updateValue}>




<style>
  
 .label_input{
    margin: 0.5em 0 0.5em 0;
    color: #000;
 }

 .input_app{
    width: 90%;
    height: 20px;
    border-radius: 10px;
    border: 1px solid #ccc;
    background-color: #ccc;
    color: #000;
    outline: none;
    padding: 0.2em;
 }


 .invalid  {
    background-color: #f75757;
 }
</style>