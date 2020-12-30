<template>
 	<div class="box__column" v-bind:style="{flex: `${flexProps}`}">
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
</template>

<script>
export default {
	props: {
		column: Object,
		columnsValue: Number
	},
	computed: {
		flexProps() {
			let flexBasis = (100 / this.columnsValue);

			if (this.columnsValue == 1) {
				return `1 1 ${flexBasis}%`;
			} else {
				return `0 1 ${flexBasis}%`;
			}
		}
	}
}
</script>

<style>

</style>