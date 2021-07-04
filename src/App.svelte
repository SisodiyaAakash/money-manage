<script>
	let src='bg.jpg';
	var income = 0;
	var needs = 50/100;
	var wants = 30/100;
	var invest = 20/100;

	var interest = 0;
	var rule=72;
</script>


<h1 class="name">Money Matters</h1>
<div class="container">
	<div class="hero">
		<h2>We know you need help <br /> to manage your earnings</h2>
		<img src="{src}" alt="">
	</div>
	<div class="input-earn">
		<input type="number" bind:value={income} placeholder="Your monthly earning" />
		<div class="result">
			<div class="result-itm needs">
				<p>
					Keep
					<br/>
					<span class="big">{income * needs}</span>
					<br/>
					for needs
				</p>
			</div>
			<div class="result-itm wants">
				<p>
					Keep
					<br/>
					<span class="big">{income * wants}</span>
					<br/>
					for wants
				</p>
			</div>
			<div class="result-itm invest">
				<p>
					Keep
					<br/>
					<span class="big">{income * invest}</span>
					<br/>
					for invest
				</p>
			</div>
		</div>
	</div>

</div>

<div class="rule-72">
	<div class="container">
		<h2>Rule 72 : Interest to double the money</h2>
		<div class="input-double">
			<input type="number" bind:value={interest} placeholder="Interest rate %">
			<h4>{interest} / 72 = {rule/interest}</h4>
			<br />
			<h4>Your money is doubled in {interest}% rate in {rule/interest} Years</h4>
		</div>
	</div>
</div>