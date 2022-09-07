<main>
  <section id="firma">
    <div class="left">
      <h1>Pieczątki Kalisz</h1>
      <p>Lata obecności na rynku to szereg doświadczeń, które przekładają się na&nbsp;wysoką jakość naszych usług.</p>
      <p>
        Na przestrzeni lat dostarczyliśmy tysiące różnych pieczątek zaspokajając w&nbsp;pełni wymagania naszych
        klientów.
      </p>
      <p>
        Najnowocześniejszy sprzęt laserowy sprawia, że nasze wyroby i usługi stoją na najwyższym poziomie jakościowym.
      </p>
    </div>
    <div class="right">
      <img src="/img/stamp.svg" alt="pieczątki" />
    </div>
  </section>

  <section id="uslugi">
    <div class="left">
      <h1>Tabliczki znamionowe</h1>
      <p>
        Wykonujemy znakowanie tabliczek i paneli metalowych, z metalu z pokryciami powierzchniowymi, laminatu oraz folii
        grawerskiej.
      </p>
      <p>Nasze systemy laserowe pozwalają na oznakowanie niewielkich elementów przy zachowaniu wyjątkowej precyzji.</p>
      <p>Efekt końcowy jest estetyczny i trwały.</p>
    </div>
    <div class="right">
      <img src="/img/plate.svg" alt="tabliczka" />
    </div>
  </section>

  <section id="kontakt">
    <div class="left">
      <h1>Kontakt</h1>
      <div class="row">
        <img src="/img/letter.png" alt="letter" />
        <div>
          <b>Email</b>
          <a href="mailto:info@reed.kalisz.pl">info@reed.kalisz.pl</a>
        </div>
      </div>
      <div class="row">
        <img src="/img/phone.png" alt="phone" />
        <div>
          <b>Telefon</b>
          <a href="tel:+48627531591">tel. 62 753 15 91</a>
          <a href="tel:+48608612625">tel. 608 612 625</a>
        </div>
      </div>
      <div class="row">
        <img src="/img/compass.png" alt="letter" />
        <div>
          <b>62-800 Kalisz<br />ul. Dobrzecka 95</b><br />
          <small>Poniedziałek - Piątek</small><br />
          8:30-16:00<br />
          <small>Sobota - Niedziela</small><br />
          Zamknięte<br />
        </div>
      </div>
    </div>

    <div class="right">
      <iframe
        title="map"
        src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d2469.6677393224336!2d18.061981!3d51.757399!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x0%3A0x47ae65b30eb92c8b!2sReed!5e0!3m2!1sen!2spl!4v1662171164031!5m2!1sen!2spl"
        width="450"
        height="450"
        style="border:0;"
        allowfullscreen=""
        loading="lazy"
        referrerpolicy="no-referrer-when-downgrade"
      />
    </div>
  </section>
</main>

<style>
  main {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 2rem;
    padding: 4rem 0;
  }

  section {
    padding: 0 2rem;
    width: 100%;
    max-width: 950px;
  }

  h1 {
    font-size: 2.25rem;
    font-weight: bold;
  }
  p {
    margin: 1.5rem 0;
  }
  .right {
    display: flex;
    justify-content: flex-end;
    width: 100%;
  }
  .right img {
    max-width: 12.5ch;
  }

  #kontakt {
    overflow: hidden;
  }
  #kontakt img {
    display: block;
    width: 2.5rem;
  }
  #kontakt .row {
    display: grid;
    grid-template-columns: 2.5rem 1fr;
    margin: 1rem 0;
  }
  #kontakt .row div {
    margin-left: 1rem;
    white-space: nowrap;
  }
  #kontakt .row a {
    display: block;
  }
  #kontakt .row a:hover {
    text-decoration: none;
  }

  @media (min-width: 700px) {
    section {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 2rem;
    }
    .left {
      gap: 1.5rem;
      max-width: 40ch;
    }
    .right img {
      max-width: 20ch;
    }
    #kontakt {
      align-items: flex-start;
    }
  }
</style>
