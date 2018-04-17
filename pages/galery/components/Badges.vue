<template>
	<div class="badges">
		<div class="badge" v-for="badge in badges">
			<div class="badge-photo" :style="{backgroundImage: 'url(' + badge.url + ')'}">
			</div>
			<h3 class="badge-title">
				{{ badge.title }}
			</h3>
			<p class="badge-text">
				{{ badge.text }}
			</p>
		</div>
	</div>
</template>

<script>
export default {
	data () {
		return {
			badges: [
				{
					title: "Значок ГТО",
					text: 'Выдается за сдачу экзамена "Готов к труду и обороне!"',
					url: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRr8RqBf9n-YP9-Xf0JW3rL6jRy8BCCJxq7IP8fa2M9DDIK9IQVmQ"
				},
				{
					title: "Знаменка 2017",
					text: 'Ежегодный фестиваль отрядной песни.',
					url: "https://meshok.net/pics/cache/73992646.208x208.jpg"
				},
				{
					title: "Кирпич 2010",
					text: 'Всероссийский студенческий отряд 2010.',
					url: "https://meshok.net/pics/35489943.jpg"
				},
				{
					title: "Кирпич 2011",
					text: 'Имени 50-летия полета Ю.Гагарина.',
					url: "https://pp.userapi.com/c630729/v630729098/34aeb/ibOLZg782JM.jpg"
				},
				{
					title: "Значок ГТО",
					text: 'Выдается за сдачу экзамена "Готов к труду и обороне!"',
					url: "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRr8RqBf9n-YP9-Xf0JW3rL6jRy8BCCJxq7IP8fa2M9DDIK9IQVmQ"
				},
				{
					title: "Знаменка 2017",
					text: 'Ежегодный фестиваль отрядной песни.',
					url: "https://meshok.net/pics/cache/73992646.208x208.jpg"
				},
				{
					title: "Кирпич 2010",
					text: 'Всероссийский студенческий отряд 2010.',
					url: "https://meshok.net/pics/35489943.jpg"
				},
				{
					title: "Кирпич 2011",
					text: 'Имени 50-летия полета Ю.Гагарина.',
					url: "https://pp.userapi.com/c630729/v630729098/34aeb/ibOLZg782JM.jpg"
				}
			]
		}
		
	}
}
</script>

<style>
.badges{
	display: flex;
	flex-wrap: wrap;
	justify-content: space-around;
}
.badge {
	padding: 10px;
	margin: 0 20px 20px 20px;
	width: 240px;
	display: flex;
	justify-content: flex-start;
	flex-flow: column;
	/*align-items: flex-start;*/
	background: #F8FAFF;
	border: 1px solid transparent;
	border-radius: 15px;
	transition: 0.2s border ease-in-out;
	color: #34314c;
}
.badge:hover {
	border: 1px solid #6a60a9;
}
.badge-photo {
	position: relative;
	height: 160px;
	background-position: center center;
	background-size: contain;
	background-repeat: no-repeat;
	box-shadow: inset 0px 0px 14px 0px rgba(0,0,0,0.5);
	margin-bottom: 10px;
	border-radius: 10px;
	overflow: hidden;
}
.badge-photo::after {
	content: "";
	position: absolute;
	width: 100%;
	height: 100%;
	background: rgba(0, 0, 0, 0.15);
	transition: 0.2s background ease-in;
}
.badge:hover .badge-photo::after{
	background: none;
}

.badge-title {
	text-align: center;
	margin-bottom: 10px;
}
</style>