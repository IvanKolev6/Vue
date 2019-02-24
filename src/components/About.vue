<template>
	<div class="content">
		 <div class="page-title">
		  	<h2>About</h2>
		  </div>
		<p>My first vue single page application</p>
	</div>
</template>

<script>
  export default {
    	created(){
    		this.$emit('loadingStart'); // Initiate loading
    		this.$emit('resetSearch'); // Initiate loading
    		setTimeout(() => {this.$emit('loadingEnd');}, 600); // Close Loading animation
    	}
  }
</script>