<script lang="ts">
</script>

<main>
	<div class="mx-auto max-w-2xl py-32 sm:py-48 lg:py-40 text-center">
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
	</div>
</main>
