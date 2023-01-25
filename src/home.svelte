<script>
import Header from "./components/header.svelte";
export let CTA_Name = "Get Started";
// const team1 = "./public/img/team-1-800x800.jpg";
// const team2 = "./public/img/team-2-800x800.jpg";
// const team3 = "./public/img/team-3-800x800.jpg";
// const team4 = "./public/img/team-4-470x470.png";
// export let location;
</script>

<!-- <Header /> -->

<!-- <h1 style="margin-top:100px;">This is the Home page</h1> -->
<main>
	<div class="left_side">
		<h1>Wellcome to <span>ENTRIES</span></h1>
        <h2>Your digital Kanban board.</h2>
		<p><span>Create the perfect agile workflow to improve project management 
            & get your team's workflow on track!</span>
            <br />Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ac dui iaculis, condimentum sapien ac, interdum libero. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ac dui iaculis, condimentum sapien ac, interdum libero. 
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ac dui iaculis, condimentum sapien ac, interdum libero. Lorem ipsum dolor sit amet, consectetur adipiscing elit. Vivamus ac dui iaculis, condimentum sapien ac, interdum libero. 
        </p>

		<button>{CTA_Name}</button>
	</div>
	<div class="right_side">
		<img src="./public/Base.png" width="100%"  alt="Mobile diplay"/>
	</div>
</main>



<footer>
	<div>
		<h3>Summary</h3>
		<h5>About Us</h5>
		<h5>Blog</h5>
		<h5>Pricing</h5>
	</div>

	<div>
		<h3>Social Links</h3>
		<h5>Facebook</h5>
		<h5>Twitter</h5>
	</div>

	<div>
		<h3>Blog</h3>
		<h5>How to select a phone ?</h5>
		<h5>Why is our company phone better ?</h5>
		<h5>Top 10 budget phones to buy in 2021 ?</h5>
	</div>

	<div>
		<button>Scroll to Top</button>
	</div>
</footer>

<style>
	main {
		display: flex;
		flex-direction: row;
		color: #000;
        margin-top:100px;
	}

	div {
		padding: 2rem;
		flex: 1;
		/* background-color: #363062; */
	}
    .left_side{
        margin-top: 80px;
    }
    main p {
        margin-top: 30px;
        /* padding: 0px 20px; */
    }
    main div h1 span {
        color: #8447ff;
        font-family: roboto;
    }
    main div h1 {
        font-size: 50px;
    }
    main h2 {
        margin-top: 20px;
        font-size: 25px;
    }
    .left_side p span {
        font-size: 20px;
        font-weight: 500;
    }
	.right_side {
		/* background-color: #ae9ec5; */
	}

	img {
		box-shadow: 0px 4px 10px #333;
	}

	button {
		margin-top: 2rem;
		min-width: 200px;
		border-radius: 2rem;
		background-color: #8447ff;
		color: white;
		font-weight: bold;
		font-size: 1.2rem;
		border: 0px;
		box-shadow: 2px 4px 5px black;
	}

    footer {
		display: flex;
        justify-content: space-around;
        background-color: #8447ff;
        color: white;
        width: 100%;
        bottom: 0;
        position: fixed;
        height: 163px;
	}

	footer h3 {
		text-transform: uppercase;
	}

	footer div {
		/* padding: 5rem 2rem; */
	}

	footer button {
		margin-top: 1rem;
		min-width: 120px;
		border-radius: 2rem;
		background-color: #8447ff;
		color: white;
		border: 0px;
	}
</style>