# money2uppercase
# **方法1：**
在main.js中引入
import {money2uppercase} from 'money2uppercase'
Vue.prototype.money2uppercase = money2uppercase


    <template>
      <div id="app">
    		<span>{{ num }}</span>
        <img alt="Vue logo" src="./assets/logo.png">
        <HelloWorld msg="Welcome to Your Vue.js App"/>
    		<span></span>
      </div>
    </template>
    
    <script>
    import HelloWorld from './components/HelloWorld.vue'
    
    export default {
      name: 'app',
      components: {
        HelloWorld
      },
    	data(){
    		return{
    			num: ''
    		}
    	},
    	created(){
    		this.num = this.money2uppercase('34546')
    	}
    }
    </script>
	
	
	
	

**方法二：**
单个文件引用


    <template>
      <div id="app">
    		<span>{{ num }}</span>
        <img alt="Vue logo" src="./assets/logo.png">
        <HelloWorld msg="Welcome to Your Vue.js App"/>
    		<span></span>
      </div>
    </template>
    
    <script>
    import {money2uppercase} from 'money2uppercase'
    import HelloWorld from './components/HelloWorld.vue'
    
    export default {
      name: 'app',
      components: {
        HelloWorld
      },
    	data(){
    		return{
    			num: ''
    		}
    	},
    	created(){
    		this.num = money2uppercase('34546')
    	}
    }
    </script>
	

效果：叁万肆仟伍佰肆拾陆元整