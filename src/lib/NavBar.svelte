<script>
    // const toggleBtn = document.querySelector('.toggle_btn');
    // const toggleBtnIcon = document.querySelector('.toggle_btn i');
    // const dropDownMenu = document.querySelector('.dropdown_menu');

    // toggleBtn.onclick = function() {
    //     dropDownMenu.classList.toggle('open') 
    //     const isOpen = dropDownMenu.classList.contains('open');

    //     toggleBtnIcon.classList = isOpen 
    //         ? 'fa-solid fa-xmark'
    //         : 'fa-solid fa-bars'
    // }

</script>

<div class="navbar">
	<div class="logo"><a href="/pagina">Web dev Creative</a></div>
	<ul class="links">
		<li><a href="hero">Home</a></li>
		<li><a href="about">About</a></li>
		<li><a href="services">Services</a></li>
		<li><a href="contact">Contact</a></li>
	</ul>
	<a href="/pagina" class="action_btn">Get Started</a>
	<div class="toggle_btn">
		<i class="fa-solid fa-bars" />
	</div>
</div>

<div class="dropdown_menu">
	<li><a href="hero">Home</a></li>
	<li><a href="about">About</a></li>
	<li><a href="services">Services</a></li>
	<li><a href="contact">Contact</a></li>
	<li><a href="/pagina" class="action_btn">Get Started</a></li>
</div>

<style>
	li {
		list-style: none;
	}

	a {
		text-decoration: none;
		color: #fff;
		font-size: 1rem;
	}
	a:hover {
		color: orange;
	}

	.navbar {
		width: 100%;
		height: 60px;
		max-width: 1200;
		margin: 0 auto;
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
	.navbar .logo a {
		font-size: 1.5rem;
		font-weight: bold;
	}

	.navbar .links {
		display: flex;
		gap: 2rem;
	}

	.navbar .toggle_btn {
		color: #fff;
		font-size: 1.5rem;
		cursor: pointer;
		display: none;
	}

	.action_btn {
		background-color: orange;
		color: #fff;
		padding: 0.5rem 1rem;
		border: none;
		outline: none;
		border-radius: 20px;
		font-size: 0.8rem;
		font-weight: bold;
		cursor: pointer;
		transition: scale 0.2 ease;
	}

	.action_btn:hover {
		scale: 1.05;
		color: #fff;
	}

	.action_btn:active {
		scale: 0.95;
	}

	.dropdown_menu {
		display: none;
		position: absolute;
		right: 2rem;
		top: 60px;
		height: 0;
		width: 300px;
		background: rgba(255, 255, 255, 0.1);
		backdrop-filter: blur(15px);
		border-radius: 10px;
		overflow: hidden;
		transition: height 0.2s cubic-bezier(0.175, 0.885, 0.32, 1.275);

	}
    .dropdown_menu.open{
        height: 240px;
    }  

	.dropdown_menu li {
		padding: 0.7rem;
		display: flex;
		align-items: center;
		justify-content: center;
	}
	.dropdown_menu .action_btn {
		width: 100%;
		display: flex;
		justify-content: center;
	}

	@media (max-width: 992px) {
		.navbar .links,
		.navbar .action_btn {
			display: none;
		}

		.navbar .toggle_btn {
			display: block;
		}

		@media (max-width: 992px) {
			.dropdown_menu {
				display: block;
			}
		}
	}
</style>
