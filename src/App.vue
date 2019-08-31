<template>
  <div>
    <p>click {{count}} times,count is {{oddOrEven}}</p>
      <button @click="inc">+</button>
      <button @click="dec">-</button>
  </div>
</template>

<script>
  export default {
		data() {
			return {
				count: 0
			}
		},
		methods: {
			//增加
			inc() {
				const count = this.count
				this.count = count + 1
			},
			//减少
			dec() {
				const count = this.count
				this.count = count - 1
			}
		},
	}
</script>

<style>

</style>
