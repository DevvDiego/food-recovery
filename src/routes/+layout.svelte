<script>
	import './layout.css';
	import favicon from '$lib/assets/favicon.svg';
	
	let { children } = $props();
</script>

<svelte:head>
	<link rel="icon" href={favicon} />
</svelte:head>


<div class="navbar bg-base-100 shadow-sm">
	<div class="flex-1">
		<a class="btn btn-ghost text-xl">Empresa</a>
	</div>

	<div class="flex-none">
	
		<ul class="menu menu-horizontal px-1 text-lg">
			<li>	
				<details>
					<summary>Menu</summary>
					<ul class="bg-base-100 rounded-t-none p-2">
                <li>
                    <a href="register">Registro usuarios</a>
                </li>
                <li>
                    <a href="register">Registro empresas</a>
                </li>
                <li>
                    <a href="alliances">Alianzas</a>
                </li>
                    </ul>
                    </details>
			</li>
		</ul>
	
	</div>
</div>



{@render children()}



<footer class="footer sm:footer-horizontal bg-base-200 text-base-content p-10">
  <nav>
    <h6 class="footer-title">Services</h6>
    <a class="link link-hover">Branding</a>
    <a class="link link-hover">Design</a>
    <a class="link link-hover">Marketing</a>
    <a class="link link-hover">Advertisement</a>
  </nav>
  <nav>
    <h6 class="footer-title">Company</h6>
    <a class="link link-hover">About us</a>
    <a class="link link-hover">Contact</a>
    <a class="link link-hover">Jobs</a>
    <a class="link link-hover">Press kit</a>
  </nav>
  <nav>
    <h6 class="footer-title">Legal</h6>
    <a class="link link-hover">Terms of use</a>
    <a class="link link-hover">Privacy policy</a>
    <a class="link link-hover">Cookie policy</a>
  </nav>
  <form>
    <h6 class="footer-title">Newsletter</h6>
    <fieldset class="w-80">
      <label>Enter your email address</label>
      <div class="join">
        <input
          type="text"
          placeholder="username@site.com"
          class="input input-bordered join-item" />
        <button class="btn btn-primary join-item">Subscribe</button>
      </div>
    </fieldset>
  </form>
</footer>