
<template>
 
 <section class="about">
    <div class="heading">
      <br>
      <h1>Abo<span>ut</span></h1><br>
      <h2 class="eoe"><br>
        Eden On Earth is small decorative “planets”,<br> designed as an alternative to to ordinary houseplant.
      </h2>
      <p class="eoe"><br><br>
        By presenting the plants as little flying planets, they become magic hanging sculptures. We make the
        planteplaneter by hand in Denmark,
        and they are based on traditional Japanese techniques with a modern, Scandinavian twist. They can be
        hung from shelves, hooks from the
        ceiling and are perfect for unused spaces. Planteplaneter gives a poetic and decorative feeling to your
        home and are a different way to grow
        and display plants.
      </p>
    </div>
    <div class="shipp">
      <div class="con">
        <h3>
          FREE SHIPPING IN DK
        </h3>
        <p>
          We are shipping all around Europe <br>within 1-10 working days. Shipping in all of Denmark with GLS
          <br>is
          free and we have a flat rate of 120kr for the rest of Europe with UPS.
        </p>
      </div>
      <div class="cons">
        <h3>GREEN CARE</h3>
        <p>
          We handle all our handgrown plants carefully. <br>If you have any questions or concerns we are
          here to help. Please send an email to info@edenonearth.co.za <br>and we will get back to you as
          quickly as
          possible.
        </p>
      </div>
    </div>
    <div class="people">
      <img src="/assets/Billede-08.09.2021-10.33 1 (2).png">
    </div>
    <div>
      <h1 class="name">Zulaigah Benja<span>min</span></h1><br>
      <div>
        <p class="names">
          The Danish architect Zulaigah Benjamin works in the field of interior design with a special focus on
          materials
          and the interaction with space.
          She works in a variety of materials and has developed such diverse products as planteplaneter, wall
          structures, stone sculptures, mobiles and furniture.
          In 2015, Zulaigah founded her own company, where she among other things, produces and sells the
          plant
          planets - a freely suspended decorative houseplant, inspired by an old Japanese method.
          Zulaigah has recently been nominated to Danish Design Award in September 2016. In 2013, she was
          nominated to
          RIBA Presidents Silvermedal.
          Zulaigah lives and works in South London where he id marrid to the famous artist known as Santan
          Dave,
          where she has her own studio in Vesterbro.
        </p>
      </div>

    </div>
  </section>

  <div class="parent">
    <img class="car" src="https://i.postimg.cc/L5C5XNYq/Billede-08-09-2021-17-48-2.png">
    <img class="hi" src="https://i.postimg.cc/KzCs2yQ4/Billede-09-09-2021-07-04-1.png">
  </div>

</template>
<script>
export default {
  
}
</script>
<style>
  .heading {
    background-image: url("https://i.postimg.cc/NLhPz7dh/output-onlinepngtools-1.png");
    
    background-repeat: no-repeat;
    height: 100vh;
}
span {
    color: white;
}
h1 {
    margin-left: 100px;
    font-size: 60px;
}
.eoe {
    margin-left: 500px;
}
.shipp {
    background-image: url("https://i.postimg.cc/VN5DfZ0C/Hanging-on-Wall.jpg");
    background-repeat: no-repeat;
    background-size: 100% 90%;
    height: 100vh;
    padding-top: 10%;
}
.parent {
  display:grid;
  grid-template-columns: repeat(2, 1fr);
  margin-top:20px;
}
 
.con,
.cons {
    height: 25%;
    border-radius: 5px;
    background-color: rgba(145, 146, 145, 0.783);
    width: 40%;
    opacity: 1;
    margin-left: 20px;
}
.cons {
    float: right;
    margin-right: 30px;
}
.people {
    float: right;
    margin-right: 20px;
}
.names {
    background-color: rgb(222, 222, 222);
    opacity: 1.5;
    border-radius: 5px;
    padding: 20px;
    
    margin-left: 50%;
}
.age,
.agee {
    display: flex;
    flex-wrap: wrap;
    margin-top: 20px;
    padding: 20px;
    margin-right: 20%;
    margin-left: 20%;
}
.agee {
    float: right;
}
.info {
    margin-left: 20px;
    text-align: center;
}
.infoe {
    margin-right: 100%;
    width: 50%;
}
</style>