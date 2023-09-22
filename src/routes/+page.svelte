<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
</script>

<svelte:head>
	<title>UNO</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<!-- <div class="parallax"></div> -->
	<div class="bg-section1">
		<div class="text-white mx-10">
			<span class="bg-black">
				Every year, the world generated about 2.3 billion tonnes of municipal solid waste, of which
			</span>
			<span class="bg-sky">45% is mismanaged.</span>
		</div>
	</div>
	<div class="bg-section2">
		<div class="flex flex-row section2-content items-center justify-center mx-10">
			<p class="text-white">
				<span class="bg-black">This resulted in an estimated</span>
				<span class="bg-sky">60 million tonnes of plastic per year from the municipal solid waste stream</span>
				<span class="bg-black">pollute the environment including water bodies, due to lack of collection services and mismanagement of solid waste."</span>
			</p>
		</div>
		<div class="section2-notes mx-7 rounded-md flex flex-row items-center py-5 px-10">
			<small>
				*According to a study conducted by UN-Habitat and the University of Leeds in 2022 using the Spatio-temporal Quantification of Plastic Pollution Origins and Transportation (SPOT) model with recently collected Waste Wise Cities Tool data inputs.
			</small>
		</div>
	</div>
	<div class="bg-section3">
		<div class="section3-content1 mx-10 text-white">
			<span class="bg-black">
				This number would be even higher without the informal waste and recovery sector (IWRS), which significantly contributes to improving solid waste management by collecting, segregating, processing and recycling plastic and other discarded materials globally.
			</span>
		</div>
		<div class="section3-content2 mx-10 text-white">
			<p>
				Conservative estimates suggest that the IWRS consist of 15 million people, recovering up to 58% of the recycled waste globally.
			</p>
		</div>
	</div>
	<div class="bg-section4">
		<div class="section4-content1 mx-10 text-white">
			<p class="text-white">
				<span class="bg-black">This resulted in an estimated</span>
				<span class="bg-sky">60 million tonnes of plastic per year from the municipal solid waste stream</span>
				<span class="bg-black">pollute the environment including water bodies, due to lack of collection services and mismanagement of solid waste."</span>
			</p>
		</div>
		<div class="section4-content2 mx-10 text-white">
			<p>
				<span class="bg-sky">This number would be even higher</span>
				<span class="bg-black">
					without the informal waste and recovery sector (IWRS), which significantly contributes to improving solid waste management by collecting, segregating, processing and recycling plastic and other discarded materials globally.
				</span>
			</p>
		</div>
		<div class="section4-notes mx-7 rounded-md flex flex-row items-center py-7 px-10">
			<small>
				*According to a study conducted by UN-Habitat and the University of Leeds in 2022 using the Spatio-temporal Quantification of Plastic Pollution Origins and Transportation (SPOT) model with recently collected Waste Wise Cities Tool data inpu
			</small>
		</div>
	</div>
</section>

<style>
	/* .parallax {
		background-image: url($lib/images/mountains.jpg);
		min-height: 500px; 
		background-attachment: fixed;
		background-position: center;
		background-repeat: no-repeat;
		background-size: cover;
	} */
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	.bg-section1{
		background-color: rgba(0,0,0,0.5);
		height:calc(100vh - 70px);
		display: flex;
		flex-direction:row;
		justify-content: center;
		align-items:center;
		margin-top:70px;
	}

	p{
		font-size:16px;
		font: normal normal medium 16px/23px var(--font-body);
	}

	.bg-sky{
		background-color: #00B2E3;
	}
	
	.bg-section2{
		background-color: rgba(0,0,0,0.5);
		height:calc(100vh - 70px);
		display: flex;
		flex-direction:column;
	}

	.bg-section2 .section2-content{
		height:680px;
	}

	.bg-section2 .section2-notes{
		/* height:calc(100vh - 750px); */
		/* background-color: #0E38A4; */
		background-color: #FF0000;
		color:#fff;
	}

	.bg-section3{
		background-color: rgba(0,0,0,0.5);
		height:calc(100vh - 70px);
		display: flex;
		flex-direction:column;
	}

	.bg-section3 .section3-content1{
		height:200px;
	}

	.bg-section3 .section3-content2{
		height:calc(100vh - 270px);
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}

	.bg-section4{
		background-color: rgba(0,0,0,0.5);
		height:calc(100vh - 70px);
		display: flex;
		flex-direction:column;
		justify-content: space-between;
	}

	.bg-section4 .section4-notes{
		/* height:calc(100vh - 750px); */
		/* background-color: #0E38A4; */
		background-color: #FF0000;
		color:#fff;
	}
</style>
