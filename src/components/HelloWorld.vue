<template>
    <div class="timeline">
      <div v-for="(value,i) in dataRoadMap"  :key="i" :class="value.active?'active-con':null">
        <div  class="container" :key="i" :class="i%2===0?'left':'right'">
          <div class="content" :class="value.active?'active':null">
            <h2>{{ value.title1 }}</h2>
            <p>
              {{value.title2 }}
            </p>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data(){
    return{
      dataRoadMap:[
        {
          title1:"NOV 2021",
          title2:"Lorem ipsum dolor sit amet elit. Aliquam odio dolor, id luctus erat sagittis non. Ut blandit semper pretium.",
          active:true
        },
        {
          title1:"NOV 2021",
          title2:"Lorem ipsum dolor sit amet elit. Aliquam odio dolor, id luctus erat sagittis non. Ut blandit semper pretium.",
          active:false
        },
        {
          title1:"NOV 2021",
          title2:"Lorem ipsum dolor sit amet elit. Aliquam odio dolor, id luctus erat sagittis non. Ut blandit semper pretium.",
          active:false
        },
        {
          title1:"NOV 2021",
          title2:"Lorem ipsum dolor sit amet elit. Aliquam odio dolor, id luctus erat sagittis non. Ut blandit semper pretium.",
          active:false
        },
        {
          title1:"NOV 2021",
          title2:"Lorem ipsum dolor sit amet elit. Aliquam odio dolor, id luctus erat sagittis non. Ut blandit semper pretium.",
          active:false
        }, {
          title1:"NOV 2021",
          title2:"Lorem ipsum dolor sit amet elit. Aliquam odio dolor, id luctus erat sagittis non. Ut blandit semper pretium.",
          active:false
        }, {
          title1:"NOV 2021",
          title2:"Lorem ipsum dolor sit amet elit. Aliquam odio dolor, id luctus erat sagittis non. Ut blandit semper pretium.",
          active:false
        }
      ]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="css" src="@/components/style.css">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
