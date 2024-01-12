<script>
import feather from 'feather-icons';
import ContactDetails from '@/components/contact/ContactDetails.vue';

export default {
	components: {
		ContactDetails,
	},
	data: () => {
		return {
			contacts: [
				{
					id: 1,
					name: 'Rio Grande do Norte, Brasil',
					icon: 'map-pin',
				},
				{
					id: 2,
					name: 'welenalmeida2210@gmail.com',
					icon: 'mail',
				},
				{
					id: 3,
					name: '(84) 9 8646-0846 - (84) 9 8151-3313',
					icon: 'phone',
				},
			],
		};
	},
	mounted() {
		feather.replace();
	},
	updated() {
		feather.replace();
	},
	methods: {},
};
</script>

<template>
	<div
		class="container mx-auto flex flex-col-reverse md:flex-row py-5 md:py-10 md:mt-10"
	>
		<!-- Contact details -->
		<ContactDetails :contacts="contacts" />
	</div>
</template>
