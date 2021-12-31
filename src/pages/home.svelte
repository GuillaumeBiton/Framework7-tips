<script>
  import {
    Page,
    Navbar,
    NavTitle,
    NavTitleLarge,
  } from 'framework7-svelte'

  import Navigation from '../components/navigation.svelte'
</script>

<Page name="home">
  <!-- Top Navbar -->
  <Navbar large>
    <NavTitle>Framework7 Tips</NavTitle>
    <NavTitleLarge>Framework7 Tips</NavTitleLarge>
  </Navbar>

  <!-- Page content -->
  <!-- Navigation list -->
  <Navigation></Navigation>
</Page>