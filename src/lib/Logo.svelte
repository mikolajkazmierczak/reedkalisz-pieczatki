<script>
  export let align = 'left';
</script>

<div class="logo" class:right={align == 'right'}>
  - pieczątki - <img src="/logo_red.svg" alt="logo" /> - tabliczki znamionowe - grawal -
  <img src="/logo_red.svg" alt="logo" />
  - automaty samotuszujące - datowniki - <img src="/logo_red.svg" alt="logo" /> - tuszownice wymienne - numeratory -
  <img src="/logo_red.svg" alt="logo" />
  - Horray - Colop - Trodat - <img src="/logo_red.svg" alt="logo" /> - automaty stemplarskie - numeratory -
</div>

<style>
  .logo {
    overflow: hidden;
    display: flex;
    justify-content: flex-start;
    padding: 1rem 0.5rem;
    gap: 1rem;
    font-size: 1rem;
    white-space: nowrap;
  }
  .logo.right {
    justify-content: flex-end;
  }
  img {
    height: 1rem;
  }
</style>
