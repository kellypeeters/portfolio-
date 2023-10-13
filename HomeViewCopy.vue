<script setup>
</script>

<template>
  <main> 

<div>
  <h1 class="titel">KELLY <br> PEETERS</h1>
</div>

  <div>
  <p> Hallo, </P>
  <p> Ik ben Kelly Peeters, <br> een grafisch designer student <br> gespecialiseerd in datavisualisatie. </P>
  </div>

  <div class="wrapper">
<ul>
  <li>
    <input type="checkbox" id="list-item-1">
    <label for="list-item-1" class="first">Opleidingen</label>
    <ul>
      <li>Moderne talen in Sint-Godelieve-Instituut Lennik, 2012 - 2014</li>
      <li>Economie Heilig-Hart&College Halle 2014 - 2016</li>
      <li>Handel Heilig-Hart&College Halle 2016 - 2018</li>
      <li>Multimedia & communicatietechnologie Erasmushogeschool Anderlecht, 2018 - 2021</li>
      <li>Media & informationdesign Sint-Lukas Schaarbeek, 2022 - ...</li>
    </ul>
  </li>
  <li>
    <input type="checkbox" id="list-item-2">
    <label for="list-item-2">Werk ervaringen</label>
    <ul>
      <li>WZC Armonea Eyckenborch | 2016 - 2021 <br> Jobstudent keukenhulp / bar en zaalmedewerker</li>
      <li>BDO Belgium | 2020 <br> Jobstudent digital marketeer</li>
      <li>BDO Belgium | 2021 <br> Stage graphic designer</li>
      <li>Ter Heyden | 2023 <br> Jobstudent bar</li>
      <li>Bpost | 2023 <br> Koerier</li>
    </ul>
  </li>
  <li>
    <input type="checkbox" id="list-item-3">
    <label for="list-item-3" class="last">Kwaliteiten</label>
    <ul>
      <li>Stressbestendig</li>
      <li>Leergierig</li>
      <li>Creatief</li>
      <li>Flexibel</li>
      <li>Ordelijk</li>
    </ul>
  </li>
</ul>
</div>
  </main>
</template>

<style scoped>

.titel{
  letter-spacing: 0.4em;
  font-size: 52px;
  float: left;
}
.wrapper{
  margin: 10% auto;
}

ul{
  list-style: none;
  margin: 0;
  padding: 0;
}

label{
  display: block;
  cursor: pointer;
  padding: 10px;
  border: 1px solid #fff;
  border-bottom: none;
}

label:hover{
  background: white;
  color: black;
}

label.last{
  border-bottom: 1px solid #fff;
}

ul ul li{
  padding: 12px;
}
 
ul{
  border: 1px solid grey;
}

input[type="checkbox"]{
  position: absolute;
  left: -9999px;
}

input[type="checkbox"] ~ ul{
  height: 0;
  transform: scaleY(0);
}

input[type="checkbox"]:checked ~ ul{
  height: 100%;
  transform-origin: top;
  transition: transform .2s ease-out;
  transform: scaleY(1); 
}

input[type="checkbox"]:checked + label{
  color: black;
  background: white;
  border-bottom: 1px solid #fff;
}

</style>
