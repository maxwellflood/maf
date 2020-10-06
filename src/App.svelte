<script>
	import Nav from './Shared/Nav.svelte'
	import PageHeader from './Shared/PageHeader.svelte'
	import Loader from './Shared/Loader.svelte'
	import ProfileHeader from './Profile/ProfileHeader.svelte'
	import ProfileContent from './Profile/ProfileContent.svelte'

</script>

<main>
	<Loader></Loader>
	<Nav></Nav>
	<PageHeader>
		<ProfileHeader/>
	</PageHeader>
	<ProfileContent>
	</ProfileContent>
</main>

<style>
	
</style>