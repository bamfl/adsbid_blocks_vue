<template>
	<div>
		<div class="options">
			<div class="template">
				<label>
					<span>Выберите шаблон:</span>
					<select :class="['select', blocksType]" v-model="blocksType" @change="typeChange">
						<option value="large" selected>Большой</option>
						<option value="carousel">Карусель</option>
						<option value="graphical_4">Графический 4</option>
						<option value="horizontal_1">Горизонтальный 1</option>
						<option value="horizontal_4">Горизонтальный 4</option>
						<option value="horizontal_5">Горизонтальный 5</option>
						<option value="horizontal_6">Горизонтальный 6</option>
						<option value="social">Социальный</option>
						<option value="smart_1">Smart 1</option>
						<option value="with_date">Объявление с датой публикации</option>
					</select>
				</label>
			</div>
			<div class="cols">
				<label>
					<span>Количество тизеров в строке:</span>
					<input :disabled="blocksType === 'horizontal_1' || blocksType === 'horizontal_4'" type="range" min="1" max="3" v-model="columnsValue" @change="transformStart">
					<div v-if="blocksType === 'carousel'">{{ columns.length }}</div>
					<div v-else-if="blocksType === 'horizontal_1'">1</div>
					<div v-else-if="blocksType === 'horizontal_4'">1</div>
					<div v-else>{{columnsValue}}</div>
				</label>
			</div>
			<div class="rows">
				<label>
					<span>Количество строк:</span>
					<input :disabled="blocksType === 'carousel'" type="range" min="1" max="5" v-model="rowsValue">
					<div v-if="blocksType === 'carousel'">1</div>
					<div v-else>{{rowsValue}}</div>
				</label>
			</div>
			<div class="border">
				<label class="border__width">Толщина рамки<input type="number" v-model="border.width"></label>
				<label class="border__color">Цвет рамки<input type="color" v-model="border.color"></label>
				<label class="border__type">Тип рамки
					<select v-model="border.type">
						<option selected value="solid">Сплошная</option>
						<option value="dotted">Пунктирная</option>
						<option value="dashed">Штриховая</option>
						<option value="double">Двойная</option>
						<option value="groove">Вдавленная</option>
						<option value="ridge">Рельефная</option>
						<option value="inset">Внутрь</option>
						<option value="outset">Наружу</option>
					</select>
				</label>
			</div>
			<div class="text">
				<label>Отступы от текста: сверху<input type="number" v-model="text['padding-top']"></label>
				<label>справа<input type="number" v-model="text['padding-right']"></label>
				<label>снизу<input type="number" v-model="text['padding-bottom']"></label>
				<label>слева<input type="number" v-model="text['padding-left']"></label>
				<label>Цвет текста<input type="color" v-model="text.color"></label>
				<label>Размер шрифта текста<input type="number" v-model="text.size"></label>
			</div>
			<div class="image">
				<label>Отступы от картинки: сверху<input type="number" v-model="image['padding-top']"></label>
				<label>справа<input type="number" v-model="image['padding-right']"></label>
				<label>снизу<input type="number" v-model="image['padding-bottom']"></label>
				<label>слева<input type="number" v-model="image['padding-left']"></label>
			</div>
		</div>

		<div :class="['box', blocksType]">
			<div class='container' :style="{'max-width': `${containerSize}px`}">
				<div class="box__row">
					<div class="arrow prev" @click="prevBtn"></div>
					<Column
						v-for="column of columns" :key="column.id"
						:column="column"
						:columnsValue="+columnsValue"
						:border="border"
						:text="text"
						:image="image"
						:style="blocksType === 'carousel' ? {transition: `transform 0.5s`, transform: `translateX(-${transformSize}px)`} : ''"
					/>
					<div class="arrow next" @click="nextBtn"></div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
import Column from '@/components/Column'

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
			blocksType: 'large',
			columnsValue: 3,
			rowsValue: 1,
			border: {
				width: '',
				color: '',
				type: 'solid'
			},
			text: {
				color: "",
				size: "",
				'padding-top': '',
				'padding-right': '',
				'padding-bottom': '',
				'padding-left': ''
			},
			image: {
				'padding-top': '',
				'padding-right': '',
				'padding-bottom': '',
				'padding-left': ''
			},
			arrowsCounter: 0,
			transformSize: 0,
		}
	},
	methods: {
		typeChange () {
			if (this.blocksType === 'carousel') {
				this.rowsValue = 5
				this.columnsValue = 2
			} else if (this.blocksType === 'horizontal_1' || this.blocksType === 'horizontal_4') {
				this.rowsValue = 1
				this.columnsValue = 1
			} else {
				this.rowsValue = 1
				this.columnsValue = 3
			}
		},
		transformStart() {
			this.transformSize = 0
			this.arrowsCounter = 0
		},
		prevBtn () {
			if (this.arrowsCounter > 0) {
				this.arrowsCounter--
				this.transformSize -= 208
			}
		},
		nextBtn () {
			if (this.arrowsCounter < this.columns.length - 5) {
				this.arrowsCounter++
				this.transformSize += 208
			}
		}
	},
	components: {
		Column
	},
	computed: {		
		columns() {
			let result = [];

			for (let i = 0; i < this.columnsValue * this.rowsValue; i++) {
				result.push({id: i+1, title: 'Большой живот не от еды! Он уйдёт за 5-10 дней, натощак пейте обычный крепкий... '})
			}

			return result
		},
		containerSize () {
			let baseContainerSize = 512

			if (this.columnsValue == 1 && this.blocksType == `smart_1`) {
				return `320`
			} else if (this.columnsValue == 2 && this.blocksType == `smart_1`) {
				return `628`
			} else if (this.columnsValue == 3 && this.blocksType == `smart_1`) {
				return `936.05`
			} else if (this.columnsValue == 1) {
				return `${baseContainerSize}`
			} else if (this.columnsValue == 2) {
				return `${baseContainerSize + 500}`
			} else if (this.columnsValue == 3) {
				return `${baseContainerSize + 1000}`
			}
		}
	}
}
</script>

<style lang="scss">
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
-ms-text-size-adjust: 100%;
-moz-text-size-adjust: 100%;
-webkit-text-size-adjust: 100%;
}

input,
button,
textarea {
font-family: inherit;
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

.options {
	background-color: #fff;
	padding: 5px;
	width: 100%;
	top: 0;
	left: 0;

	.border, .text, .image {
		display: flex;
		flex-wrap: wrap;
	}
}

select {
	border: 1px solid #000;
	margin: 0px 0px 0px 3px;
}

label {
	margin: 0px 50px 10px 0px;
	display: flex;
	flex-wrap: wrap;
	align-items: center;

	input {
		margin: 0px 0px 0px 3px;
		border: 1px solid #000;
		padding: 2px;
		width: 100px;
	}
}
</style>
