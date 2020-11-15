<template>
<v-container fluid>
	<v-layout
	class="d-flex flex-wrap justify-space-around">
		<!-- Author Photo floating-->
		<v-flex
		class="d-flex flex-wrap justify-center px-0 mx-0">
			<!-- This is an author profile img -->
			<v-avatar
			class="profile ml-2 mt-5"
			size="188"
			rounded="lg">
				<v-img
				src="https://ma-v3-images.azureedge.net/images/2286237009.jpg"
				></v-img>
			</v-avatar>
		</v-flex>

		<!-- Author Profile -->
		<v-flex
		class="d-flex flex-wrap justify-center"
		>
			<v-card flat
			max-width="900px">
						<v-card-title
						class="text-h3"
						>
							<i
							class="fa fa-user" aria-hidden="true"
							></i>
							Zhi-hua Zhou
						</v-card-title>
						<v-card-subtitle>
							Nanjing University
						</v-card-subtitle>
						<v-list>
							<v-list-item>
								<i class="fa fa-newspaper-o" aria-hidden="true"></i>
								610 Publications
								<v-spacer></v-spacer>
								<i class="fa fa-quote-right" aria-hidden="true"></i>
								50802 Ciations
								<v-spacer
								v-for="i in 10"
								:key="i"></v-spacer>
							</v-list-item>



							<v-list-item>
								<v-list-item-title
								class="text-h6">
									Biography
								</v-list-item-title>
							</v-list-item>

							<v-list-item>
								<v-card flat>
								Zhou Zhi-Hua (周志华; born November 20, 1973) is a Professor of Computer Science at Nanjing University. He is the Standing Deputy Director of the National Key Laboratory for Novel Software Technology, and Founding Director of the LAMDA Group. His research interests include artificial intelligence, machine learning and data mining.
								</v-card>
							</v-list-item>

							<v-list-item two-line>
								<v-list-content>
								<v-list-item-title
								class="text-h6"
								>
									Website Links
								</v-list-item-title>
								<v-container>
									<v-list-actions>
										en.wikipedia.org
									</v-list-actions>
								</v-container>
							</v-list-content>
							</v-list-item>


							<v-list-item>
								<v-list-content>
								<v-list-item-title
								class="text-h6"
								>
									Related Topics
								</v-list-item-title>
								<v-layout
								class="flex-wrap">
									<v-flex
									v-for="item in rearchTopics"
									:key="item">
									<v-container>
										<v-btn>{{item}}</v-btn>
									</v-container>
									</v-flex>
								</v-layout>
							</v-list-content>
							</v-list-item>
							
						</v-list>
			</v-card>
		</v-flex>
	</v-layout>

	<v-spacer></v-spacer>
		
	<!-- divider -->
	<v-layout>
			<v-flex>
			<v-divider></v-divider>
			</v-flex>
	</v-layout>

	<!-- Author achievement -->
	<v-layout
	class="d-flex flex-wrap"
	yellow>
	<!-- Article List -->
		<v-flex
		class=""
		blue>
		<v-tabs>
			<v-tab>PUBLICATIONS</v-tab>
			<v-tab>CITATED BY</v-tab>
			<v-tab>CONFERENCES</v-tab>
			<v-tab>JOURNALS</v-tab>
		</v-tabs>
		</v-flex>
		<v-flex
		class="d-none d-md-block"
		green>
			This is author analyse.
		</v-flex>
	</v-layout>

</v-container>
</template>


<script>

export default {
  name: 'ScholarProfile',

  components: {
    
  },

  data() {
    return {
        rearchTopics: [
        'Computer science',
        'Artificial intelligence',
        'Machine learning',
      ],
    }
  },
}
</script>