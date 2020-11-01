<template>
	<v-app-bar app>
		<v-toolbar-item>
			<v-container id="logo">
				<v-img  
					src="@/assets/logo.png"
					height="100%" 
					max-height="80px"
					max-width="50px"
					contain></v-img>
			</v-container>
		</v-toolbar-item>
		<v-toolbar-title>
			Robin Academic
		</v-toolbar-title>
		<v-spacer></v-spacer>
		<v-toolbar-item>
			<v-container>
				<v-content>
					SignIn/SignOut
				</v-content>
			</v-container>
		</v-toolbar-item>
	</v-app-bar>
</template>

<script>
export default {
  name: 'NavBar',

  components: {
    
  },

  data() {
    return {
        
    }
  },

}
</script>
