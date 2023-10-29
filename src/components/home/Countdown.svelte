<script lang="ts">
	import { onDestroy } from 'svelte';
	import Digit from './Digit.svelte';

	let update = 0;

	let targetDate = new Date('2023-11-13T09:30:00').getTime();
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
		update++;
	};

	const toStringWithTwoDigits = (value: number) => value.toString().padStart(2, '0');
	const getFirstDigit = (value: number) => parseInt(toStringWithTwoDigits(value)[0]);
	const getSecondDigit = (value: number) => parseInt(toStringWithTwoDigits(value)[1]);

	const interval = setInterval(updateCountdown, 500);

	onDestroy(() => {
		clearInterval(interval);
	});
</script>

<div class="countdown">
	<img class="sticky" src="icons/sticky.png" alt="">
	<div class="time">
		<img src="icons/time.gif" alt="" />
		<div>Rejoignez nous</div>
	</div>
	<div class="digits">
		<div>
			<Digit digit={getFirstDigit(days)} {update} />
			<Digit digit={getSecondDigit(days)} {update} />
		</div>
		<span>Jours</span>
	</div>
	<div class="colon">:</div>
	<div class="digits">
		<div>
			<Digit digit={getFirstDigit(hours)} {update} />
			<Digit digit={getSecondDigit(hours)} {update} />
		</div>
		<span>Heures</span>
	</div>
	<div class="colon">:</div>
	<div class="digits">
		<div>
			<Digit digit={getFirstDigit(minutes)} {update} />
			<Digit digit={getSecondDigit(minutes)} {update} />
		</div>
		<span>Minutes</span>
	</div>
	<div class="colon">:</div>
	<div class="digits">
		<div>
			<Digit digit={getFirstDigit(seconds)} {update} />
			<Digit digit={getSecondDigit(seconds)} {update} />
		</div>
		<span>Secondes</span>
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
		gap: 0.5em;
		position: relative;

		@media screen and (max-width: 768px) {
			padding: 0.5em;
			font-size: 0.9em;
		}

		.sticky {
			width: 150px;
			height: 40px;
			position: absolute;
			top: -20px;

			@media screen and (max-width: 768px) {
				display: none;
			}
		}

		.time {
			width: 60px;
			margin-right: 1em;
			position: relative;
			top: 0.125em;
			display: flex;
			flex-direction: column;
			align-items: center;
			gap: 0.5em;

			@media screen and (max-width: 768px) {
				margin-right: 0.5em;
			}

			img {
				width: 30px;
				height: 30px;
				transform: scale(1.5);

				@media screen and (max-width: 768px) {
					transform: scale(1.2);
				}
			}

			div {
				font-weight: bold;
				text-transform: uppercase;
				text-align: center;
				font-style: italic;
			}
		}

		.digits {
			position: relative;
			top: 8px;

			@media screen and (max-width: 768px) {
				top: 0px;
			}

			div {
				display: flex;
				justify-content: center;
				gap: 0 0.25em;
				height: 40px;
				overflow: hidden;
			}

			span {
				display: flex;
				justify-content: center;
			}
		}

		.colon {
			position: relative;
			top: -6px;
			color: var(--primary-color);
			font-weight: bold;

			@media screen and (max-width: 768px) {
				top: -14px;
			}
		}
	}
</style>
