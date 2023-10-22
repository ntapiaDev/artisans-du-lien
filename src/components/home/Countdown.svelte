<script lang="ts">
	import { onDestroy } from 'svelte';

	let targetDate = new Date('2023-11-13T08:30:00').getTime();
	let timeRemaining = targetDate - Date.now();
	let days = Math.floor(timeRemaining / (1000 * 60 * 60 * 24));
	let hours = Math.floor((timeRemaining % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
	let minutes = Math.floor((timeRemaining % (1000 * 60 * 60)) / (1000 * 60));
	let seconds = Math.floor((timeRemaining % (1000 * 60)) / 1000);

	const updateCountdown = () => {
		timeRemaining = targetDate - Date.now();
		days = Math.floor(timeRemaining / (1000 * 60 * 60 * 24));
		hours = Math.floor((timeRemaining % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
		minutes = Math.floor((timeRemaining % (1000 * 60 * 60)) / (1000 * 60));
		seconds = Math.floor((timeRemaining % (1000 * 60)) / 1000);
	};

	const toStringWithTwoDigits = (value: number) => value.toString().padStart(2, '0');
	const getFirstDigit = (value: number) => toStringWithTwoDigits(value)[0];
	const getSecondDigit = (value: number) => toStringWithTwoDigits(value)[1];

	const interval = setInterval(updateCountdown, 1000);

	onDestroy(() => {
		clearInterval(interval);
	});
</script>

<div class="countdown">
	<div class="time">
		<img src="icons/time.png" alt="" />
		<div>Rejoignez nous</div>
	</div>
	<div class="digits">
		<div>
			<div>{getFirstDigit(days)}</div>
			<div>{getSecondDigit(days)}</div>
		</div>
		<div>Jours</div>
	</div>
	<div class="colon">:</div>
	<div class="digits">
		<div>
			<div>{getFirstDigit(hours)}</div>
			<div>{getSecondDigit(hours)}</div>
		</div>
		<div>Heures</div>
	</div>
	<div class="colon">:</div>
	<div class="digits">
		<div>
			<div>{getFirstDigit(minutes)}</div>
			<div>{getSecondDigit(minutes)}</div>
		</div>
		<div>Minutes</div>
	</div>
	<div class="colon">:</div>
	<div class="digits">
		<div>
			<div>{getFirstDigit(seconds)}</div>
			<div>{getSecondDigit(seconds)}</div>
		</div>
		<div>Secondes</div>
	</div>
</div>

<style lang="scss">
	.countdown {
		padding: 1em;
		background-color: var(--secondary-color);
		color: #FFFFFF;
		border-radius: 1em;
		display: flex;
		align-items: center;
		justify-content: center;
		gap: 1em;

		@media screen and (max-width: 768px) {
			padding: 0.5em;
			font-size: 0.9em;
			gap: 0.5em;
		}

		.time {
			width: 60px;
			margin-right: 0.5em;
			display: flex;
			flex-direction: column;
			align-items: center;
			gap: 0.5em;

			img {
				width: 30px;
				height: 30px;
			}

			div {
				font-weight: bold;
				text-transform: uppercase;
				text-align: center;
				font-style: italic;
			}
		}

		.digits {
			div {
				display: flex;
				justify-content: center;
				gap: 0.25em;

				div {
					width: 20px;
					height: 40px;
					font-weight: bold;
					font-size: 1.25em;
					background-color: var(--primary-color);
					color: var(--secondary-color);
					display: flex;
					align-items: center;
					justify-content: center;
				}
			}
		}

		.colon {
			position: relative;
			top: -14px;
			color: var(--primary-color);
			font-weight: bold;
		}
	}
</style>
