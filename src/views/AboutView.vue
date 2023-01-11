<template>
  <div class="about">
    <h1>About Me</h1>

    <div class="container">
      <div class="rightSide">
        <h4>Right</h4>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum porro,
          praesentium quod quisquam maiores dolorum corrupti. Deleniti nostrum accusamus
          voluptate obcaecati consequuntur excepturi incidunt placeat fuga, veritatis aut
          quisquam a!
        </p>
      </div>
      <div class="rightSideCenter">
        <h4>RightCenter</h4>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Harum porro,
          praesentium quod quisquam maiores dolorum corrupti. Deleniti nostrum accusamus
          voluptate obcaecati consequuntur excepturi incidunt placeat fuga, veritatis aut
          quisquam a!
        </p>
      </div>
      <div class="leftSideCenter">
        <h4>leftCenter</h4>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. A reiciendis laborum
          odio beatae voluptatibus cumque distinctio totam itaque aspernatur suscipit
          dolorum hic, minima deleniti fugit corporis omnis! Maxime, a ea.
        </p>
      </div>
      <div class="leftSide">
        <h4>left</h4>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. A reiciendis laborum
          odio beatae voluptatibus cumque distinctio totam itaque aspernatur suscipit
          dolorum hic, minima deleniti fugit corporis omnis! Maxime, a ea.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.about {
  min-height: 90vh;
}

.container {
  display: grid;
  grid-template-columns: auto auto auto auto;
  grid-gap: 10px;
}

.rightSide {
  float: right;
  margin: auto;
  padding: 20px 30px;
  color: black;
  background: lightgray;
  border-radius: 5%;
}

.rightSideCenter {
  padding: 20px 20px;
}

.leftSideCenter {
  padding: 20px 20px;
}

.leftSide {
  float: left;
  margin: auto;
  padding: 20px 70px;
}
</style>
