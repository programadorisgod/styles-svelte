<script>
  import Input from "./Input.svelte";

 let name = "John";
 let lastname = "Doe";

</script>

<main class="main_app">
   <h1 class="title_app">Hi! {name}</h1>
   
   <fieldset class="fieldset_app">
   <Input  id="name"  label="Name" bind:value={name}  />
    <Input id="lastname" label="Lastname" bind:value={lastname} />
   </fieldset>

   <span class="span_main_app">You are <strong> {name} {lastname} </strong> </span>
</main>

<style>

  .title_app{
    color: #000;
    margin-bottom: 1.5em;
  }
 
  .fieldset_app{
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin-bottom: 1.5em;
    width: 100%;
    height: 200px;
    border-radius: 10px;
    border: 1px solid #ccc;
    box-shadow: 0 0 10px #ccc;
  }

  .span_main_app{
    color: #000;
  }

</style>
