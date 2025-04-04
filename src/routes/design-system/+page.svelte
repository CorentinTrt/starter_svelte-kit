<svelte:head>
	<title>Svelte Starter - Design System</title>
	<meta name="description" content="Display all colors of the design system." />
</svelte:head>

<section>
	<div class="primary color-group">
		<div class="primary__color color-block">
			<p class="label">primary</p>
		</div>
		<div class="primary__color--hover color-block">
			<p class="label">primary-hover</p>
		</div>
		<div class="primary__color--on color-block">
			<p class="label">on-primary</p>
		</div>
		<div class="primary__color--outline color-block">
			<p class="label">outline-primary</p>
		</div>
	</div>

	<div class="secondary color-group">
		<div class="secondary__color color-block">
			<p class="label">secondary</p>
		</div>
		<div class="secondary__color--hover color-block">
			<p class="label">secondary-hover</p>
		</div>
		<div class="secondary__color--on color-block">
			<p class="label">on-secondary</p>
		</div>
		<div class="secondary__color--outline color-block">
			<p class="label">outline-secondary</p>
		</div>
	</div>

	<div class="success color-group">
		<div class="success__color color-block">
			<p class="label">success</p>
		</div>
		<div class="success__color--on color-block">
			<p class="label">on-success</p>
		</div>
		<div class="success__color--outline color-block">
			<p class="label">outline-success</p>
		</div>
	</div>

	<div class="warning color-group">
		<div class="warning__color color-block">
			<p class="label">warning</p>
		</div>
		<div class="warning__color--on color-block">
			<p class="label">on-warning</p>
		</div>
		<div class="warning__color--outline color-block">
			<p class="label">outline-warning</p>
		</div>
	</div>

	<div class="error color-group">
		<div class="error__color color-block">
			<p class="label">error</p>
		</div>
		<div class="error__color--on color-block">
			<p class="label">on-error</p>
		</div>
		<div class="error__color--outline color-block">
			<p class="label">outline-error</p>
		</div>
	</div>

	<div class="disabled color-group">
		<div class="disabled__color color-block">
			<p class="label">disabled</p>
		</div>
		<div class="disabled__color--on color-block">
			<p class="label">on-disabled</p>
		</div>
		<div class="disabled__color--outline color-block">
			<p class="label">outline-disabled</p>
		</div>
	</div>

	<div class="surface color-group">
		<div class="surface__color color-block">
			<p class="label">surface</p>
		</div>
		<div class="surface__color--bright color-block">
			<p class="label">surface-bright</p>
		</div>
		<div class="surface__color--dim color-block">
			<p class="label">surface-dim</p>
		</div>
		<div class="surface__color--on color-block">
			<p class="label">on-surface</p>
		</div>
		<div class="surface__color--outline color-block">
			<p class="label">outline-surface</p>
		</div>
	</div>
</section>

<style lang="scss">
	section {
		--size-gap: 1rem;

		width: 100%;
		padding: 3rem 0 0 0;
		display: flex;
		flex-direction: column;
		gap: var(--size-gap);
		flex: 1;

		@media screen and (min-width: 600px) {
			flex-direction: row;
			flex-wrap: wrap;

			.color-group {
				flex: 0 0 calc(50% - calc(var(--size-gap) / 2));
			}
		}

		.primary {
			&__color {
				background-color: var(--color-primary);
				.label {
					color: var(--color-on-primary);
				}
				&--hover {
					background-color: var(--color-primary-hover);
					.label {
						color: var(--color-on-primary);
					}
				}
				&--on {
					background-color: var(--color-on-primary);
				}
				&--outline {
					background-color: var(--color-outline-primary);
				}
			}
		}

		.secondary {
			&__color {
				background-color: var(--color-secondary);
				.label {
					color: var(--color-on-secondary);
				}
				&--hover {
					background-color: var(--color-secondary-hover);
					.label {
						color: var(--color-on-secondary);
					}
				}
				&--on {
					background-color: var(--color-on-secondary);
				}
				&--outline {
					background-color: var(--color-outline-secondary);
				}
			}
		}

		.success {
			&__color {
				background-color: var(--color-success);
				.label {
					color: var(--color-on-success);
				}
				&--on {
					background-color: var(--color-on-success);
				}
				&--outline {
					background-color: var(--color-outline-success);
				}
			}
		}

		.warning {
			&__color {
				background-color: var(--color-warning);
				.label {
					color: var(--color-on-warning);
				}
				&--on {
					background-color: var(--color-on-warning);
				}
				&--outline {
					background-color: var(--color-outline-warning);
				}
			}
		}

		.error {
			&__color {
				background-color: var(--color-error);
				.label {
					color: var(--color-on-error);
				}
				&--on {
					background-color: var(--color-on-error);
				}
				&--outline {
					background-color: var(--color-outline-error);
				}
			}
		}

		.disabled {
			&__color {
				background-color: var(--color-disabled);
				.label {
					color: var(--color-on-disabled);
				}
				&--on {
					background-color: var(--color-on-disabled);
				}
				&--outline {
					background-color: var(--color-outline-disabled);
				}
			}
		}

		.surface {
			&__color {
				background-color: var(--color-surface);
				.label {
					color: var(--color-on-surface);
				}
				&--bright {
					background-color: var(--color-surface-bright);
					.label {
						color: var(--color-on-surface);
					}
				}
				&--dim {
					background-color: var(--color-surface-dim);
					.label {
						color: var(--color-on-surface);
					}
				}
				&--on {
					background-color: var(--color-on-surface);
					.label {
						color: var(--color-white);
					}
				}
				&--outline {
					background-color: var(--color-outline-surface);
				}
			}
		}

		.label {
			font-family: var(--font-family-mono);
		}

		.color-block {
			height: 5rem;
			padding: 0.3rem;
		}
	}
</style>
