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
		<div class="flex flex-row section1-content fade-in-text items-center justify-center text-white mx-10 lg:mx-36">
			<p>
				<span class="bg-black">
					Every year, the world generated about 2.3 billion tonnes of municipal solid waste, of which
				</span>
				<span class="bg-sky">45% is mismanaged.</span>
			</p>
		</div>
	</div>
	<div class="bg-section2">
		<div class="flex flex-row section2-content items-center justify-center mx-10 lg:mx-36">
			<p class="text-white">
				<span class="bg-black">This resulted in an estimated</span>
				<span class="bg-sky">60 million tonnes of plastic per year from the municipal solid waste stream</span>
				<span class="bg-black">pollute the environment including water bodies, due to lack of collection services and mismanagement of solid waste."</span>
			</p>
		</div>
		<div class="section2-notes mx-7 lg:mx-36 rounded-md flex flex-row items-center py-5 px-10">
			<small>
				* According to a study conducted by UN-Habitat and the University of Leeds in 2022 using the Spatio-temporal Quantification of Plastic Pollution Origins and Transportation (SPOT) model with recently collected Waste Wise Cities Tool data inputs.
			</small>
		</div>
	</div>
	<div class="bg-section3">
		<div class="section3-content1 mx-10 lg:mx-36 text-white">
			<span class="bg-black">
				This number would be even higher without the informal waste and recovery sector (IWRS), which significantly contributes to improving solid waste management by collecting, segregating, processing and recycling plastic and other discarded materials globally.
			</span>
		</div>
		<div class="section3-content2 mx-10 lg:mx-36 text-white">
			<p>
				Conservative estimates suggest that the IWRS consist of 15 million people, recovering up to 58% of the recycled waste globally.
			</p>
		</div>
		<div class="section3-content3 mx-10 lg:mx-36 text-white">
			<div>
				<span class="bg-sky heading p-1">
					IWRS
				</span>
			</div>
			<div>
				<span class="bg-black subheading">
					INFORMAL WASTE AND RECOVERY SECTOR
				</span>
			</div>
			<div class="mt-2">
				<span class="bg-black">
					is a sector of the informal economy where workers and economic units are involved in solid waste collection and recovery activities which are – in law or in practice – not covered or insufficiently covered by formal arrangements.
				</span>
			</div>
		</div>
		<div class="section3-content4 mx-10 lg:mx-36 text-white">
			<div>
				A
				<span class="heading">
					 JUST TRANSITION
				</span>
			</div>
			<div>
				of the IWRS means that the transition to sustainable production and consumption of plastic is designed in a manner that is as fair, inclusive and equitable as possible to the IWRS, generating and preserving decent work opportunities, and leaving no one behind.
			</div>
		</div>
		<div class="section3-content5 mx-10 lg:mx-36 text-white">
			<div class="my-20">
				<span class="bg-black">
					Solutions can only be sustainable if those who are affected are able to contribute to the decision-making process with thoughts, knowledge and expectations.
				</span>
			</div>
			<div class="my-20">
				<span class="bg-black">
					Though their contribution to public health, cleaning communities, resource efficiency and circular economy is clear, they are disproportionately affected by the plastic pollution. Many of those are women, youth, and often children.
				</span>
			</div>
			<div class="my-20">
				<span class="bg-black">
					They often face unhealthy working conditions and are exposed to severe occupational and health impacts from hazardous materials.
				</span>
			</div>
		</div>
	</div>
	<div class="bg-section4">
		<div class="section4-content1 mx-10 lg:mx-36 text-white">
			<p class="text-white">
				<span class="bg-black">This resulted in an estimated</span>
				<span class="bg-sky">60 million tonnes of plastic per year from the municipal solid waste stream</span>
				<span class="bg-black">pollute the environment including water bodies, due to lack of collection services and mismanagement of solid waste."</span>
			</p>
		</div>
		<div class="section4-content2 mx-10 lg:mx-36 text-white">
			<p>
				<span class="bg-sky">This number would be even higher</span>
				<span class="bg-black">
					without the informal waste and recovery sector (IWRS), which significantly contributes to improving solid waste management by collecting, segregating, processing and recycling plastic and other discarded materials globally.
				</span>
			</p>
		</div>
		<div class="section4-notes mx-7 lg:mx-36 rounded-md flex flex-row items-center py-7 px-10">
			<small>
				* According to a study conducted by UN-Habitat and the University of Leeds in 2022 using the Spatio-temporal Quantification of Plastic Pollution Origins and Transportation (SPOT) model with recently collected Waste Wise Cities Tool data inpu
			</small>
		</div>
	</div>
</section>

<style>
	.parallax {
		background-image: url($lib/images/mountains.jpg);
		position: absolute;
		top:100vh;
		min-height: 100vh; 
		width:100%;
		background-attachment: fixed;
		background-position: center;
		background-repeat: no-repeat;
		background-size: cover;
	}
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	.bg-section1{
		/* background-color: rgba(0,0,0,0.5); */
		background-image: url($lib/images/mountains.jpg);
		background-position: center;
		background-repeat: no-repeat;
		background-size: cover;
		height:calc(100vh - 70px);
		width:100%;
		display: flex;
		flex-direction:row;
		align-items:center;
		z-index:1;
		margin-top:70px;
	}

	.fade-in-text{
		animation: fadeIn 5s;
		-webkit-animation: fadeIn 5s;
		-moz-animation: fadeIn 5s;
		-o-animation: fadeIn 5s;
		-ms-animation: fadeIn 5s;
	}

	@keyframes fadeIn {
		0% { opacity: 0; }
		100% { opacity: 1; }
	}

	@-moz-keyframes fadeIn {
		0% { opacity: 0; }
		100% { opacity: 1; }
	}

	@-webkit-keyframes fadeIn {
		0% { opacity: 0; }
		100% { opacity: 1; }
	}

	@-o-keyframes fadeIn {
		0% { opacity: 0; }
		100% { opacity: 1; }
	}

	@-ms-keyframes fadeIn {
		0% { opacity: 0; }
		100% { opacity: 1; }
	}

	p{
		font-size:16px;
		font: normal normal medium 16px/23px var(--font-body);
	}

	.bg-sky{
		background-color: #00B2E3;
	}
	
	.bg-section2{
		/* background-color: rgba(0,0,0,0.5); */
		background-image: url($lib/images/mountain2.jpeg);
		background-position: center;
		background-repeat: no-repeat;
		background-size: cover;
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
		/* background-color: rgba(0,0,0,0.5); */
		background-image: url($lib/images/view.jpeg);
		background-position: center;
		background-repeat: no-repeat;
		background-size: cover;
		min-height:calc(100vh - 70px);
		overflow-y:auto;
		display: flex;
		flex-direction:column;
	}

	.bg-section3 .section3-content1{
		height:200px;
	}

	.bg-section3 .section3-content2{
		height:calc(100vh - 470px);
		display: flex;
		flex-direction: column;
		justify-content: center;
	}

	.bg-section3 .section3-content3{
		padding:50px 0;
	}

	.bg-section3 .section3-content3 .heading{
		font: normal normal 900 40px/160px var(--font-body);
	}

	.bg-section3 .section3-content3 .subheading{
		font: normal normal 900 26px/32px var(--font-body);
	}

	.bg-section3 .section3-content4{
		padding:100px 0;
	}

	.bg-section3 .section3-content4 .heading{
		font: normal normal 900 26px/32px Roboto;
	}

	.bg-section4{
		/* background-color: rgba(0,0,0,0.5); */
		background-image: url($lib/images/mountain2.jpeg);
		background-position: center;
		background-repeat: no-repeat;
		background-size: cover;
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
