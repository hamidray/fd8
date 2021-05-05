<template>
   <form>
       
  <div class="form-group">
    <label for="exampleFormControlFile1">ADD 9GAG</label>
    <input type="file" class="form-control-file" id="exampleFormControlFile1">
  </div>

  <div class="form-group">
    <label for="exampleFormControlInput1">Name</label>
    <input type="text" class="form-control" id="exampleFormControlInput1" placeholder="Name">
  </div>

    <div class="form-group">
    <label for="exampleFormControlTextarea1">Description</label>
    <textarea class="form-control" id="exampleFormControlTextarea1" rows="3"></textarea>
  </div>
 
  <div class="form-group">
    <label for="exampleFormControlTextarea1">Comments</label>
    <textarea class="form-control" id="exampleFormControlTextarea1" rows="1"></textarea>
  </div>

  <div class="form-group">
    <label for="exampleFormControlSelect1">Heat</label>
    <select class="form-control" id="exampleFormControlSelect1">
      <option>1</option>
      <option>2</option>
      <option>3</option>
      <option>4</option>
      <option>5</option>
    </select>
  </div>
 
  <button type="button" class="btn btn-primary btn-lg btn-block">Submit</button>

</form>

  </template>

<script>
export default {
    name: 'Home'
}
</script>

<style>

</style>