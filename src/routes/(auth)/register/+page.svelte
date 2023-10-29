<script lang="ts">
	import type { PageData } from './$types';

	export let data: PageData;
</script>

<main>
	<div class="card p-4">
		<h1>Sign Up</h1>
		<form action="?/register" method="POST" class="auth-form">
			<label for="email" class="label"
				><span>Email</span>
				<input class="input" type="text" name="email" />
			</label>

			<label for="password" class="label"
				><span>Password</span>
				<input class="input" type="password" name="password" />
			</label>

			<button type="button" class="btn variant-filled">Sign Up</button>
		</form>
	</div>
</main>
