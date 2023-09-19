<!-- <script>
    const toggleBtn = document.querySelector('.toggle_btn');
    const toggleBtnIcon = document.querySelector('.toggle_btn i');
    const dropDownMenu = document.querySelector('.dropdown_menu');

    toggleBtn.onclick = function() {
        dropDownMenu.classList.toggle('open') 
        const isOpen = dropDownMenu.classList.contains('open');

        toggleBtnIcon.classList = isOpen 
            ? 'fa-solid fa-xmark'
            : 'fa-solid fa-bars'
    }

</script>

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

    .dropdown_menu{
        display: none;
        position: absolute;
        right: 2rem;
        top: 60px;
        height: 0;
        width: 300px;
        background: rgba(255,255,255,0.1);
        backdrop-filter: blur(15px);
        border-radius: 10px;
        overflow: hidden;
        transition: height 0.2s cubic-bezier(0.175, 0.885, 0.32, 1.275);
    }

    /* .dropdown_menu.open{
        height: 240px;
    } */

    .dropdown_menu li{
        padding: 0.7rem;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .dropdown_menu .action_btn{
        width: 100%;
        display: flex;
        justify-content: center;
    }

    @media (max-width: 992px){
        .dropdown_menu {
            display: block;
        }
    }
</style> -->
