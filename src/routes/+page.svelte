<head>
	<style>
		:root {
 	  --background: #323834;
  	--white: #ffffff;
		}


		body{
  	  background: var(--background);
    	background-size: 400% 400%;
	    size: 10vh;
		}
		.div{
			display: flex;
  		justify-content: center;
  		align-items: center;
  		text-align: center;
  		min-height: 100vh;
			flex-wrap: wrap;
			margin: 10px;
  		padding: 20px;
		}
		button{
			margin: 10px;
  		padding: 20px;

			background: var(--background);
			border-radius: 50px;
			border-width: 5px;
			border-color: var(--background);
			border-style: solid;
			min-width: 150px;
			min-height: 50px;
			position:relative;
			box-shadow: 10px 10px 15px #212121, -10px -10px 15px #424242, inset 2px 2px 15px var(--background), inset -2px -2px 15px var(--background);
						transition:  all .2s;
			color: white;
			-webkit-appearance: none;

			}
			button:hover{
											box-shadow: 5px 5px 15px #212121, -5px -5px 15px #424242, inset 10px 10px 15px #212121, inset -10px -10px 15px #424242;
			}
			.input{
							margin: 10px;
  		padding: 20px;
			color: white;
			background: var(--background);
			border-radius: 50px;
			border-width: 5px;
			border-color: var(--background);
			border-style: solid;
			min-width: 150px;
			position:relative;
			box-shadow: 10px 10px 15px #212121, -10px -10px 15px #424242, inset 2px 2px 15px var(--background), inset -2px -2px 15px var(--background);
			transition:  all .2s;

			}
			.input:focus{
											box-shadow: 5px 5px 15px #212121, -5px -5px 15px #424242, inset 10px 10px 15px #212121, inset -10px -10px 15px #424242;

			}
			textarea:focus, input:focus{
    outline: none;
}


	</style>
	<title>Home</title>
</head>
<body class="background">
<div class="div">
<input class="input" bind:value={Name} placeholder="Input Name Here">
<button on:click={Button}>Show {Name}</button>
</div>
</body>


<script>
function Button(){
	alert("You " + Name + "!")
}
let Name = "";
</script>