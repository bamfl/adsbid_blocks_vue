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

.large {
	.container {
	  padding: 30px 10px;
	  max-width: 512px !important;
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
	  -webkit-box-flex: 1;
	      -ms-flex: 1 1 100%;
	          flex: 1 1 100%;
	  padding: 4px;
	  min-width: 300px;
	}
	
	.box__column:not(:nth-child(2)) {
	  display: none;
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
	  overflow: hidden;
	}
	
	.item-box__image {
	  position: relative;
	  padding: 0px 0px 66.668% 0px;
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
	  font-size: 30px;
	  margin: 65px 10px 10px;
	  overflow: hidden;
	  -o-text-overflow: ellipsis;
	     text-overflow: ellipsis;
	  display: -moz-box;
	  display: -webkit-box;
	  -webkit-line-clamp: 3;
	  -webkit-box-orient: vertical;
	  line-clamp: 3;
	  box-orient: vertical;
	}
	
	@media (max-width: 425px) {
	  .item-box__descr {
	    font-size: 25px;
	  }
	}
	
	@media (max-width: 425px) {
	  .item-box__descr {
	    font-size: 20px;
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
	
	.item-box__descr {
	  color: #fff;
	}
	
	.item-box__text {
	  background: -webkit-gradient(linear, left top, left bottom, from(transparent), color-stop(15%, rgba(77, 68, 77, 0.25)), color-stop(50%, #4d444d));
	  background: -o-linear-gradient(transparent, rgba(77, 68, 77, 0.25) 15%, #4d444d 50%);
	  background: linear-gradient(transparent, rgba(77, 68, 77, 0.25) 15%, #4d444d 50%);
	  color: #fff;
	}
	
	.item-box__shadow {
	  background: rgba(229, 196, 174, 0.4);
	}
}
</style>