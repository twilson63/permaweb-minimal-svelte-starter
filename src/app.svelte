<script lang="ts">
import { Route, router } from 'tinro'
import Counter from './counter.svelte'
import About from './about.svelte'

// add hash routing for permaweb support
router.mode.hash()

</script>
<nav>
<a href="/">Home</a> | <a href="/about">About</a>
</nav>
<Route path="/"><Counter /></Route>
<Route path="/about"><About /></Route>