<template>
  <!-- <div> Hello {{ name }}</div>
  <div v-html="channel"></div>
  <button v-bind:disabled="isDisabled"> bind</button>
  <h2 v-bind:class="status">Status </h2>
  <h2 v-bind:class="isPromoted && 'promoted'">Promoted movie</h2>
  <h2 v-bind:class="['new', 'promoted']"> Newly promoted movie</h2>
  <h2 v-bind:class="{promoted: isPromoted,
                      new: isSoldout,
                      'sold-out': isSoldout}"> Object conditional movie</h2>
  <h2 v-bind:style="{
    color: hightlightColor,
    'font-size': headerSize +'px'}">
      Inline style</h2>

  <h2 v-bind:style="headerStyleObject">Style object</h2>
    <div v-bind:style="[baseStyleObject,successStyleObject]">Success Style</div>
    <div v-bind:style="[baseStyleObject,dangerStyleObject]">Danger Style</div>
    
    <h2 v-if="num === 0"> The number is 0</h2>
    <h2 v-else-if="num < 0"> The number is negative</h2>
    <h2 v-else-if="num > 0"> The number is positive</h2>
    <h2 v-else> not a number</h2>
    <h2 v-for="(name,index) in names" :key="name"> {{ index }} {{ name }}</h2>
    <h2 v-for="name in fullNames" :key="name.first"> {{name.first}} {{ name.last }}</h2>

    <div v-for="actor in actors" :key="actor.name">
      <h2>{{ actor.name }}</h2>
       <h3 v-for="movie in actor.movies" :key="movie"> {{ movie }}</h3>
    </div>
    <h2 v-for="name in names" :key="name">
      <h2 v-if="name === 'Bruce'"> {{ name }}</h2>
    </h2> -->
  
  <!-- <div>
    <pre>
      {{ JSON.stringify(formValues, null, 2) }}
    </pre>
  </div>
  <form @submit="submitForm">
    <div>
      <label for="name">Name</label>
      <input type="text" id="name" v-model.trim.lazy="formValues.name">
    </div>
    
    <div>
        <label for="age">Age</label>
        <input @keyup.enter="submitForm" type="number" id="age" v-model.number="formValues.age">
    </div>

    <div>
      <label for="name">Profile Summary</label>
      <textarea id="profile" v-model.trim="formValues.profileSummary"/>
    </div>

    <div>
      <label for="country">Country</label>
      <select id="country" v-model="formValues.country">
        <option value="">Select a country</option>
          <option value="india"> India</option>
          <option value="vietnam"> Vietname</option>
          <option value="france"> France</option>
      </select>
    </div>

    <div>
      <label for="job_location">Job Location</label>
      <select id="job_location" multiple v-model="formValues.jobLocation">
          <option value="india"> India</option>
          <option value="vietnam"> Vietname</option>
          <option value="france"> France</option>
      </select>
    </div>

    <div>
      <input type="checkbox" id="remoteWork" v-model="formValues.remoteWork" true-value="yes" false-value="no"/>
      <label for="remoteWork">Open to remote work?</label>
    </div>

    <div>
      <label>Skill set</label>
      <input type="checkbox" id="html" value="html" v-model="formValues.skillSet" />
      <label for="html">HTML</label>
      <input type="checkbox" id="css" value="css" v-model="formValues.skillSet"/>
      <label for="css">CSS</label>
      <input type="checkbox" id="javascript" value="javascript" v-model="formValues.skillSet"/>
      <label for="javascript">javascript</label>
    </div>

    <div>
      <label>Years of Experience</label>
      <input
        type="radio"
        id="0-2"
        value="0-2"
        v-model="formValues.yearsofExperience"/>

        <label>0-2</label>
      <input
        type="radio"
        id="3-5"
        value="3-5"
        v-model="formValues.yearsofExperience"/>

        <label>3-5</label>
      <input
        type="radio"
        id="6-10"
        value="6-10"
        v-model="formValues.yearsofExperience"/>
        <label>6-10</label>
      </div>

  </form> -->
  <!-- <h2>Volume Tracker (0-20)</h2>
  <h3>Current Volume : {{ volume }}</h3>
  <div>
    <button @click="volume += 2"> Increase</button>
    <button @click="volume -= 2"> Decrease</button>
  </div>

  <div>
    <input type="text" v-model="movie"/>
    <input type="text" v-model="movieInfo.title"/>
    <input type="text" v-model="movieInfo.actor"/>

  </div>

  <div>
    <button @click="movieList = movieList.concat(['Wonder Woman'])"> Add movie</button>

  </div> -->
  <!-- <Greet name="Elwin" heroName="Batman"/>
  <Greet name="Cyprien" heroName="Superman" />
  <Greet name="Noan" heroName="Wonder Woman"/>
  <Greet :name="name" :heroName="channel"/> -->
  <!-- <Article id="my-article" title="Article title" :likes="50" :isPublished="true"/>
  <h3>Appcomponent username {{  name }}</h3>
  <ComponentC></ComponentC> -->
  <!-- <button @click="showPopup = true">Show popup</button>
  <Popup v-show="showPopup" @close="closePopup"/> -->
  <!-- <Input v-model="name"/> -->
  <!-- <Card></Card>
  <Card>Card content</Card>
  <Card>
    <h2>Card content</h2>
  </Card>
  <Card>
    <img src="https://picsum.photos/200"/>
  </Card>
  <Card>
    <template v-slot:header>
      <h3>Header</h3>
    </template>
    <template v-slote:default>
      <img src="https://picsum.photos/200"/>
    </template>
    <template v-slot:footer>
      <button>View details</button>
    </template>
  </Card> -->
  <!-- <NameList>
    <template v-slot:default="slotProps">
    {{ slotProps.firstName }} {{ slotProps.lastName }}
    </template>
  </NameList>

  <NameList>
    <template v-slot:default="slotProps">
      {{ slotProps.lastName }} {{ slotProps.firstName }}
    </template>
  </NameList>

  <NameList>
    <template v-slot:default="slotProps">
      {{ slotProps.firstName }}
    </template>
  </NameList> -->
  
    <!-- <h4>App Component text</h4>
    <ChildStyles>
      <h4>App Component text</h4>
    </ChildStyles> -->

    <!-- <button @click="activeTab ='TabA'">Tab A</button>
    <button @click="activeTab ='TabB'">Tab B</button>
    <button @click="activeTab ='TabC'">Tab C</button>
    <keep-alive>
      <component :is="activeTab" />
    </keep-alive> -->
    <!-- <Portal to="#portal-root"></Portal> -->
    <!-- <CreatePost></CreatePost>
    <PostList></PostList> -->
    <!-- <TemplateRef></TemplateRef> -->
    <ClickCount></ClickCount>
    <HoverCounter></HoverCounter>
    <!-- <Data></Data> -->
    <!-- <DemoTwo></DemoTwo> -->
    <!-- <Methods></Methods> -->
    <!-- <Watch></Watch> -->
</template>
<script>
// import Article from './components/A conterticle.vue';
// import ComponentC from './components/ComponentC.vue';
// import Greet from './components/Greet.vue';
// import Input from './components/Input.vue';
// import Card from './components/Card.vue';
// import NameList from './components/NameList.vue';
// import ChildStyles from './components/ChildStyles.vue';
// import TabA from './components/TabA.vue';
// import TabB from './components/TabB.vue';
// import TabC from './components/TabC.vue';
// import Portal from './components/Portal.vue';
// import TemplateRef from './components/TemplateRef.vue';
import ClickCount from './components/ClickCounter.vue';
import HoverCounter from './components/HoverCounter.vue';
// import Data from './components/Data.vue';
// import DemoTwo from './components/DemoTwo.vue';
// import Methods from './components/Methods.vue';
// import Watch from './components/Watch.vue';

export default {
  name: 'App',
  components: {
    // Greet,
    // Article,
    // ComponentC,
    // Popup,
    // Input
    // Card,
    // NameList,
    // ChildStyles,
    // TabA,
    // TabB,
    // TabC,
    // Portal,
    // PostList,
    // CreatePost,
    // TemplateRef,
    ClickCount,
    HoverCounter
    // Data,
    // DemoTwo
    // Methods
    // Watch
  },
  data() {
    return {
      activeTab: 'TabA',
      showPopup: false,
      name: '',
      channel: 'Codevolution',
      isDisabled: false,
      isPromoted: false,
      hightlightColor: 'orange',
      headerSize: 50,
      headerStyleObject: {
        color: 'orange',
        fontSize: '50px',
        padding: '20px'
      },
      baseStyleObject: {
        fontSize: '50px',
        padding: '10px',
      },
      successStyleObject: {
        color:'green',
        backgroundColor: 'lightgreen',
        border: '1px solid green',
        padding: '20px',
      },
      dangerStyleObject: {
        color: 'darkred',
        backgroundColor: 'red',
        border: '1 px solid darkred',
      },
      num: 5,
      names: [ 'Bruce', 'Clark', 'Diana'],
      fullNames: [
        { first: 'Bruce', last:'Wayne'},
        { first: 'Clark', last:'Kent'},
        { first: 'Princess', last:'Diana'},
      ],
      actors: [
        { name: 'Christian Bale',
          movies: ['Batman', 'The Prestige'],
        },
        { name: 'Di Caprio',
          movies: ['Titanic', 'Inception'],
        },
      ],
      formValues: {
        name: '',
        age: null,
        profileSummary: '',
        country:'',
        jobLocation: [],
        remoteWork: "no",
        skillSet: [],
        yearsofExperience: ''
      },
      firstName: 'Bruce',
      lastName: 'Wayne',
      volume: 0,
      movie:'Batman',
      movieInfo:{
        title: '',
        actor: '',
      },
      movieList: ['Batman', 'Superman']
    };
  },
  methods:{
    submitForm() {
      // event.preventDefault()
      console.log('Form values', this.formValues)
    },
    closePopup(name) {
      this.showPopup = false;
      console.log('name', name)
    }
  },
  computed:{
    fullName(){
      return `${this.firstName} ${this.lastName}`
    }
  },
  watch:{
    volume(newValue, oldValue){
      if(newValue === 16 && oldValue < newValue){
        alert('Listening to a high volume for a long time is harmful')
      }
    },
    movie: {
      handler(newValue) {
        console.log(`Calling API with movie name = ${newValue}`)
      },
      immediate:true,
    },
    movieInfo:{
     handler(newValue){
      console.log(`Calling API with movie title = ${newValue.title} and actor = ${newValue.actor}`)
     },
     deep: true
    },
    movieList: {
      handler(newValue){
        console.log(`updated list ${newValue}`)
      },
      deep: true
    }
  },
  provide() {
    return {
      username: this.name
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.promoted {
  font-style: italic;
}

h4 {
  color: orange;
}
</style>
