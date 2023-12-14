<script>

    export let value;
    export let label;
    export let id;
   

</script>



<label class="label_input" for={id}>{label}</label>
<input type="text" bind:value id={id}  class:invalid={value.length === 0} class="input_app">




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
    background-color: #f11111;
    
 }
</style>