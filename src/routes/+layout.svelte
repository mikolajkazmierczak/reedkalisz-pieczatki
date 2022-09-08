<script>
  import '$lib/global.css';

  import Ribbon from '$lib/Ribbon.svelte';
</script>

<Ribbon />

<slot />

<footer>
  <a href="/obowiazek-informacyjny">Obowiązek informacyjny</a>
  <a href="/polityka-prywatnosci">Polityka prywatności</a>
  <p>Dariusz Kaźmierczak i Artur Fornalczyk sp.j.<br />Wszystkie prawa zastrzeżone © 2022</p>
</footer>

<Ribbon />

<style>
  footer,
  footer * {
    text-align: center;
    font-size: 0.85rem;
  }
  footer a {
    white-space: nowrap;
  }
</style>
