<form method="post">
	<div class="form-group">
		<input type="text" required />
		<label for="input">名</label>
		<div class="bar" />
	</div>

	<div class="form-group">
		<input type="text" required />
		<label for="input">性</label>
		<div class="bar" />
	</div>
</form>

<style>
	.form-group {
		position: relative;
		margin-top: 45px;
	}

	input {
		font-size: 18px;
		padding: 10px 10px 10px 5px;
		display: block;
		width: 300px;
		border: none;
		border-bottom: 1px solid #757575;
	}

	input:focus {
		outline: none;
	}

	label {
		color: #999;
		font-size: 18px;
		font-weight: normal;
		position: absolute;
		pointer-events: none;
		left: 5px;
		top: 10px;
		transition: 0.2s ease all;
	}

	/* active state */
	input:focus ~ label,
	input:valid ~ label {
		top: -20px;
		font-size: 14px;
		color: #5264ae;
	}

	.bar {
		position: relative;
		display: block;
		width: 300px;
	}
</style>
