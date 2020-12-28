<template>
	<div>
		<label>
			Выберите шаблон:
			<select class="select large" v-model="blocksType" v-on:change="addClass">
				<option selected value="Large">Большой</option>
				<option value="Carousel">Карусель</option>
				<option value="Graphical_4">Графический 4</option>
				<option value="Horizontal_1">Горизонтальный 1</option>
				<option value="Horizontal_4">Горизонтальный 4</option>
				<option value="Horizontal_5">Горизонтальный 5</option>
				<option value="Horizontal_6">Горизонтальный 6</option>
				<option value="Social">Социальный</option>
				<option value="Smart_1">Smart 1</option>
				<option value="With_date">Объявление с датой публикации</option>
			</select>
			{{ blocksType }}
		</label>
		<div class="box large">
			<div class='container'>
				<div class="box__row">
					<div class="arrow prev"></div>
					<div class="box__column">
						<a href="#" class="box__item item-box item-box_1">
							<div class="item-box__image">
								<div class="item-box__top">
									<div class="item-box__icon">
										<img src="@/assets/images/heart.png" alt="">
									</div>
									<div class="item-box__name">
										<div class="item-box__title">Медицина 24/7</div>
										<div class="item-box__subtitle">2 ч. назад</div>
									</div>
								</div>
								<img src="@/assets/images/01.jpg" alt="">
							</div>
							<div class="item-box__text">
								<div class="item-box__descr">
									Большой живот не от еды! Он уйдёт за 5-10 дней, натощак пейте обычный крепкий...
									<span class="item-box__else">Ещё</span>
								</div>
								<div class="item-box__socials">
									<div class="item-box__social item-box__likes">205</div>
									<div class="item-box__social item-box__comments">33</div>
									<div class="item-box__social item-box__refs">117</div>
								</div>
								<div class="item-box__bottom">
									<div class="item-box__date"><span>3</span> ч. назад</div>
									<div class="item-box__menu"></div>
								</div>
								<div class="item-box__btn">Читать далее</div>
							</div>
							<div class="item-box__shadow"></div>
						</a>
					</div>
					<div class="box__column">
						<a href="#" class="box__item item-box item-box_2">
							<div class="item-box__image">
								<div class="item-box__top">
									<div class="item-box__icon">
										<img src="@/assets/images/heart.png" alt="">
									</div>
									<div class="item-box__name">
										<div class="item-box__title">Медицина 24/7</div>
										<div class="item-box__subtitle">2 ч. назад</div>
									</div>
								</div>
								<img src="@/assets/images/02.jpg" alt="">
							</div>
							<div class="item-box__text">
								<div class="item-box__descr">
									Врачи притихли.. Эта штука восстанавливает суставы в любом возрасте! Пишите рецепт, пока не удалили
									<span class="item-box__else">Ещё</span>
								</div>
								<div class="item-box__socials">
									<div class="item-box__social item-box__likes">412</div>
									<div class="item-box__social item-box__comments">118</div>
									<div class="item-box__social item-box__refs">358</div>
								</div>
								<div class="item-box__bottom">
									<div class="item-box__date"><span>12</span> ч. назад</div>
									<div class="item-box__menu"></div>
								</div>
								<div class="item-box__btn">Читать далее</div>
							</div>
							<div class="item-box__shadow"></div>
						</a>
					</div>
					<div class="box__column">
						<a href="#" class="box__item item-box item-box_3">
							<div class="item-box__image">
								<div class="item-box__top">
									<div class="item-box__icon">
										<img src="@/assets/images/heart.png" alt="">
									</div>
									<div class="item-box__name">
										<div class="item-box__title">Медицина 24/7</div>
										<div class="item-box__subtitle">2 ч. назад</div>
									</div>
								</div>
								<img src="@/assets/images/03.jpg" alt="">
							</div>
							<div class="item-box__text">
								<div class="item-box__descr">
									Студент из г. Краснодар выяснил, как можно вернуть зрение в любом возрасте! Перед сном капайте...                    
									<span class="item-box__else">Ещё</span>
								</div>
								<div class="item-box__socials">
									<div class="item-box__social item-box__likes">153</div>
									<div class="item-box__social item-box__comments">188</div>
									<div class="item-box__social item-box__refs">98</div>
								</div>
								<div class="item-box__bottom">
									<div class="item-box__date"><span>6</span> ч. назад</div>
									<div class="item-box__menu"></div>
								</div>
								<div class="item-box__btn">Читать далее</div>
							</div>
							<div class="item-box__shadow"></div>
						</a>
					</div>
					<div class="box__column">
						<a href="#" class="box__item item-box item-box_4">
							<div class="item-box__image">
								<div class="item-box__top">
									<div class="item-box__icon">
										<img src="@/assets/images/heart.png" alt="">
									</div>
									<div class="item-box__name">
										<div class="item-box__title">Медицина 24/7</div>
										<div class="item-box__subtitle">2 ч. назад</div>
									</div>
								</div>
								<img src="@/assets/images/04.jpg" alt="">
							</div>
							<div class="item-box__text">
								<div class="item-box__descr">
									Уколы не лечат суставы! Суставы излечатся сами за 7 дней, если мазать их обычным 3%-м...
									<span class="item-box__else">Ещё</span>
								</div>
								<div class="item-box__socials">
									<div class="item-box__social item-box__likes">206</div>
									<div class="item-box__social item-box__comments">198</div>
									<div class="item-box__social item-box__refs">109</div>
								</div>
								<div class="item-box__bottom">
									<div class="item-box__date"><span>6</span> ч. назад</div>
									<div class="item-box__menu"></div>
								</div>
								<div class="item-box__btn">Читать далее</div>
							</div>
							<div class="item-box__shadow"></div>
						</a>
					</div>
					<div class="box__column mid">
						<a href="#" class="box__item item-box item-box_5">
							<div class="item-box__image">
								<div class="item-box__top">
									<div class="item-box__icon">
										<img src="@/assets/images/heart.png" alt="">
									</div>
									<div class="item-box__name">
										<div class="item-box__title">Медицина 24/7</div>
										<div class="item-box__subtitle">2 ч. назад</div>
									</div>
								</div>
								<img src="@/assets/images/05.jpg" alt="">
							</div>
							<div class="item-box__text">
								<div class="item-box__descr">
									4 растения, которые восстанавливают суставы и хрящи в 1000 раз лучше врачей!
									<span class="item-box__else">Ещё</span>
								</div>
								<div class="item-box__socials">
									<div class="item-box__social item-box__likes">195</div>
									<div class="item-box__social item-box__comments">137</div>
									<div class="item-box__social item-box__refs">143</div>
								</div>
								<div class="item-box__bottom">
									<div class="item-box__date"><span>9</span> ч. назад</div>
									<div class="item-box__menu"></div>
								</div>
								<div class="item-box__btn">Читать далее</div>
							</div>
							<div class="item-box__shadow"></div>
						</a>
					</div>
					<div class="box__column big">
						<a href="#" class="box__item item-box item-box_6">
							<div class="item-box__image">
								<div class="item-box__top">
									<div class="item-box__icon">
										<img src="@/assets/images/heart.png" alt="">
									</div>
									<div class="item-box__name">
										<div class="item-box__title">Медицина 24/7</div>
										<div class="item-box__subtitle">2 ч. назад</div>
									</div>
								</div>
								<img src="@/assets/images/06.jpg" alt="">
							</div>
							<div class="item-box__text">
								<div class="item-box__descr">
									Военный врач: В советской армии от грибка избавлялись за 3 дня! Грибковые ногти топили в растворе...                    
									<span class="item-box__else">Ещё</span>
								</div>
								<div class="item-box__socials">
									<div class="item-box__social item-box__likes">153</div>
									<div class="item-box__social item-box__comments">59</div>
									<div class="item-box__social item-box__refs">57</div>
								</div>
								<div class="item-box__bottom">
									<div class="item-box__date"><span>7</span> ч. назад</div>
									<div class="item-box__menu"></div>
								</div>
								<div class="item-box__btn">Читать далее</div>
							</div>
							<div class="item-box__shadow"></div>
						</a>
					</div>
					<div class="arrow next"></div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
import Large from '@/components/Large'
import Carousel from '@/components/Carousel'
import Graphical_4 from '@/components/Graphical_4'
import Horizontal_1 from '@/components/Horizontal_1'
import Horizontal_4 from '@/components/Horizontal_4'
import Horizontal_5 from '@/components/Horizontal_5'
import Horizontal_6 from '@/components/Horizontal_6'
import Social from '@/components/Social'
import Smart_1 from '@/components/Smart_1'
import With_date from '@/components/With_date'

export default {
	data () {
		return {
			blocksType: 'Large'
		}
	},
	methods: {
		addClass() {
			let select = document.querySelector('.select');
			let box = document.querySelector('.box')

			if (this.blocksType === 'Large') {
				select.className = 'select large';
				box.className = 'box large';

			} else if (this.blocksType === 'Carousel') {
				select.className = 'select carousel';
				box.className = 'box carousel';

			} else if (this.blocksType === 'Graphical_4') {
				select.className = 'select graphical_4';
				box.className = 'box graphical_4';

			} else if (this.blocksType === 'Horizontal_1') {
				select.className = 'select horizontal_1';
				box.className = 'box horizontal_1';

			} else if (this.blocksType === 'Horizontal_4') {
				select.className = 'select horizontal_4';
				box.className = 'box horizontal_4';

			} else if (this.blocksType === 'Horizontal_5') {
				select.className = 'select horizontal_5';
				box.className = 'box horizontal_5';

			} else if (this.blocksType === 'Horizontal_6') {
				select.className = 'select horizontal_6';
				box.className = 'box horizontal_6';

			} else if (this.blocksType === 'Social') {
				select.className = 'select social';
				box.className = 'box social';

			} else if (this.blocksType === 'Smart_1') {
				select.className = 'select smart_1';
				box.className = 'box smart_1';

			} else if (this.blocksType === 'With_date') {
				select.className = 'select with_date';
				box.className = 'box with_date';
			}
		}
	},
	components: {
		Large,
		Carousel,
		Graphical_4,
		Horizontal_1,
		Horizontal_4,
		Horizontal_5,
		Horizontal_6,
		Social,
		Smart_1,
		With_date
	}
}
</script>

<style>
*,
*:before,
*:after {
-webkit-box-sizing: border-box;
box-sizing: border-box;
}

:focus,
:active {
outline: none;
}

a:focus,
a:active {
outline: none;
}

aside,
nav,
footer,
header,
section {
display: block;
}

html,
body {
height: 100%;
min-width: 320px;
scroll-behavior: smooth;
}

body {
line-height: 1.2;
font-family: Arial;
-ms-text-size-adjust: 100%;
-moz-text-size-adjust: 100%;
-webkit-text-size-adjust: 100%;
}

input,
button,
textarea {
font-family: Arial;
}

input::-ms-clear {
display: none;
}

button {
cursor: pointer;
}

button::-moz-focus-inner {
padding: 0;
border: 0;
}

a {
color: inherit;
font-size: inherit;
}

a,
a:visited {
text-decoration: none;
}

a:hover {
text-decoration: none;
}

ul li {
list-style: none;
}

img {
vertical-align: top;
}

h1,
h2,
h3,
h4,
h5,
h6 {
font-weight: inherit;
font-size: inherit;
margin: 0;
padding: 0;
}

label {
	position: absolute;
	top: 0;
	left: 0;
	z-index: 10;
	background-color: #fff;
	padding: 5px;
}
.select {
	border: 1px solid #000;
}
</style>