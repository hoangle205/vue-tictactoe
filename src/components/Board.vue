<template>
  <div>
		<div v-for="i in 3" :key="i">
			<div v-for="j in 3" :key="j" >
				<Square :value="board[i][j]"></Square>
			</div>
		</div>
  </div>
</template>






<script>
import Square from './Square.vue'

export default {
  
	name: 'Board',

	components: {
    Square
  },

  data() {
		return {
			board: [
        ['','',''],
        ['','',''],
        ['','',''],
      ]
    }
  },

  
}


</script>