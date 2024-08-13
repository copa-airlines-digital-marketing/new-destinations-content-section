<script>
	import DestinationActivities from "$lib/components/DestinationActivities/DestinationActivities.svelte";
import DestinationsDescription from "$lib/components/DestinationDescription/DestinationsDescription.svelte";
import * as Header from "$lib/components/MainHeader";
	import TouringSection from "$lib/components/TouringSection/TouringSection.svelte";
</script>

<Header.Root image='53eaa676-56c4-486c-901b-14428c0257d0'>
    <Header.Title>Raleigh-Durham</Header.Title>
    <Header.Description>¡Bienvenidos a Raleigh-Durham, también conocido como el “Triángulo de la Investigación”! ¡La ciudad donde la historia, la cultura vibrante y la autenticidad culinaria se entrelazan para ofrecerte una experiencia inolvidable! Explora estas ciudades cautivadoras en Carolina del Norte, Estados Unidos.</Header.Description>
</Header.Root>


<DestinationsDescription/>
<DestinationActivities/>
<TouringSection/>


