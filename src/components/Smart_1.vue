<template>
	<div></div>
</template>

<script>
export default {

}
</script>

<style lang="scss">
* {
	padding: 0px;
	margin: 0px;
	border: 0px;
}

.smart_1 {
	.container {
	  padding: 30px 10px;
	  max-width: 936.02px !important;
	}
	
	.arrow {
	  display: none;
	}
	
	.box__row {
	  display: -webkit-box;
	  display: -ms-flexbox;
	  display: flex;
	  -ms-flex-wrap: wrap;
	      flex-wrap: wrap;
	  margin: 0 -4px;
	}
	
	.box__column {
	  -webkit-box-flex: 0;
	      -ms-flex: 0 1 33.333%;
	          flex: 0 1 33.333%;
	  padding: 4px;
	}
	
	.box__column.mid {
	  -webkit-box-flex: 0;
	      -ms-flex: 0 1 66.667%;
	          flex: 0 1 66.667%;
	}
	
	.box__column.mid .item-box__image {
	  padding: 0px 0px 49.34% 0px;
	}
	
	@media (max-width: 600px) {
	  .box__column.mid .item-box__image {
	    padding: 0px 0px 100% 0px;
	  }
	}
	
	.box__column.big {
	  -webkit-box-flex: 1;
	      -ms-flex: 1 1 100%;
	          flex: 1 1 100%;
	}
	
	.box__column.big .item-box__image {
	  padding: 0px 0px 32.751% 0px;
	}
	
	@media (max-width: 600px) {
	  .box__column.big .item-box__image {
	    padding: 0px 0px 100% 0px;
	  }
	}
	
	@media (max-width: 600px) {
	  .box__column {
	    -webkit-box-flex: 1 !important;
	        -ms-flex: 1 1 100% !important;
	            flex: 1 1 100% !important;
	    min-width: 100%;
	  }
	}
	
	.item-box {
	  display: -webkit-box;
	  display: -ms-flexbox;
	  display: flex;
	  -webkit-box-orient: vertical;
	  -webkit-box-direction: normal;
	      -ms-flex-direction: column;
	          flex-direction: column;
	  position: relative;
	  border-radius: 4px;
	  overflow: hidden;
	  min-height: 100%;
	}
	
	.item-box__image {
	  position: relative;
	  padding: 0px 0px 100% 0px;
	}
	
	.item-box__image img {
	  position: absolute;
	  width: 100%;
	  height: 100%;
	  top: 0;
	  left: 0;
	  -o-object-fit: cover;
	     object-fit: cover;
	}
	
	.item-box__text {
	  position: absolute;
	  width: 100%;
	  bottom: 0;
	  left: 0;
	}
	
	.item-box__descr {
	  text-align: left;
	  text-decoration: none;
	  font-weight: bold;
	  line-height: 1.4;
	  font-size: 19px;
	  margin: 65px 10px 10px;
	  overflow: hidden;
	  -o-text-overflow: ellipsis;
	     text-overflow: ellipsis;
	  display: -moz-box;
	  display: -webkit-box;
	  -webkit-line-clamp: 4;
	  -webkit-box-orient: vertical;
	  line-clamp: 4;
	  box-orient: vertical;
	}
	
	@media (max-width: 768px) {
	  .item-box__descr {
	    font-size: 16px;
	    line-height: 1.2;
	  }
	}
	
	@media (max-width: 600px) {
	  .item-box__descr {
	    font-size: 19px;
	    line-height: 1.4;
	  }
	}
	
	.item-box__shadow {
	  position: absolute;
	  width: 100%;
	  height: 100%;
	  top: 0;
	  left: 0;
	  opacity: 0;
	  -webkit-transition: all 0.2s ease-out 0s;
	  -o-transition: all 0.2s ease-out 0s;
	  transition: all 0.2s ease-out 0s;
	}
	
	.item-box__shadow:hover {
	  opacity: 1;
	}
	
	.item-box__btn {
	  display: none;
	}
	
	.item-box__else {
	  display: none;
	}
	
	.item-box__socials {
	  display: none;
	}
	
	.item-box__top {
	  display: none;
	}
	
	.item-box__title {
	  display: none;
	}
	
	.item-box__subtitle {
	  display: none;
	}
	
	.item-box__bottom {
	  display: none;
	}
	
	.item-box__date {
	  display: none;
	}
	
	.item-box__menu {
	  display: none;
	}
	
	.item-box__icon {
	  display: none;
	}
	
	.item-box__likes {
	  display: none;
	}
	
	.item-box__comments {
	  display: none;
	}
	
	.item-box__refs {
	  display: none;
	}
	
	.item-box_1 .item-box__text {
	  background: -webkit-gradient(linear, left top, left bottom, from(transparent), color-stop(15%, rgba(229, 196, 174, 0.25)), color-stop(50%, #e5c4ae));
	  background: -o-linear-gradient(transparent, rgba(229, 196, 174, 0.25) 15%, #e5c4ae 50%);
	  background: linear-gradient(transparent, rgba(229, 196, 174, 0.25) 15%, #e5c4ae 50%);
	}
	
	.item-box_1 .item-box__shadow {
	  background: rgba(229, 196, 174, 0.4);
	}
	
	.item-box_2 .item-box__text {
	  background: -webkit-gradient(linear, left top, left bottom, from(transparent), color-stop(15%, rgba(199, 169, 120, 0.25)), color-stop(50%, #c7a978));
	  background: -o-linear-gradient(transparent, rgba(199, 169, 120, 0.25) 15%, #c7a978 50%);
	  background: linear-gradient(transparent, rgba(199, 169, 120, 0.25) 15%, #c7a978 50%);
	}
	
	.item-box_2 .item-box__shadow {
	  background: rgba(199, 169, 120, 0.4);
	}
	
	.item-box_3 .item-box__text {
	  background: -webkit-gradient(linear, left top, left bottom, from(transparent), color-stop(15%, rgba(77, 68, 77, 0.25)), color-stop(50%, #4d444d));
	  background: -o-linear-gradient(transparent, rgba(77, 68, 77, 0.25) 15%, #4d444d 50%);
	  background: linear-gradient(transparent, rgba(77, 68, 77, 0.25) 15%, #4d444d 50%);
	  color: #fff;
	}
	
	.item-box_3 .item-box__shadow {
	  background: rgba(77, 68, 77, 0.4);
	}
	
	.item-box_4 .item-box__text {
	  background: -webkit-gradient(linear, left top, left bottom, from(transparent), color-stop(15%, rgba(1, 1, 4, 0.25)), color-stop(50%, #010104));
	  background: -o-linear-gradient(transparent, rgba(1, 1, 4, 0.25) 15%, #010104 50%);
	  background: linear-gradient(transparent, rgba(1, 1, 4, 0.25) 15%, #010104 50%);
	  color: #fff;
	}
	
	.item-box_4 .item-box__shadow {
	  background: rgba(1, 1, 4, 0.4);
	}
	
	.item-box_5 .item-box__text {
	  background: -webkit-gradient(linear, left top, left bottom, from(transparent), color-stop(15%, rgba(97, 126, 83, 0.25)), color-stop(50%, #617e53));
	  background: -o-linear-gradient(transparent, rgba(97, 126, 83, 0.25) 15%, #617e53 50%);
	  background: linear-gradient(transparent, rgba(97, 126, 83, 0.25) 15%, #617e53 50%);
	  color: #fff;
	}
	
	.item-box_5 .item-box__shadow {
	  background: rgba(97, 126, 83, 0.4);
	}
	
	.item-box_6 .item-box__text {
	  background: -webkit-gradient(linear, left top, left bottom, from(transparent), color-stop(15%, rgba(96, 100, 78, 0.25)), color-stop(50%, #60644e));
	  background: -o-linear-gradient(transparent, rgba(96, 100, 78, 0.25) 15%, #60644e 50%);
	  background: linear-gradient(transparent, rgba(96, 100, 78, 0.25) 15%, #60644e 50%);
	  color: #fff;
	}
	
	.item-box_6 .item-box__shadow {
	  background: rgba(96, 100, 78, 0.4);
	}
}
</style>