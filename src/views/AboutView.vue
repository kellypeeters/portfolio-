<template>
  <div class="about">
    <h1>About me</h1>
    <p>Mijn ambitie om creativiteit te beleven en tegemoet te komen aan de werkelijke 
      behoeften van mensen als het gaat om mediaconsumptie, heeft ertoe geleid dat ik 
      mijn bachelor Multimedia & communicatietechnologie heb afgerond en momenteel
      de opleiding Media & informationdesign volg.</p>
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
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
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
