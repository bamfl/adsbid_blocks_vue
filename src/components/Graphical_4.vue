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

.graphical_4 {
	.container {
	  padding: 30px 10px;
	//   max-width: 1512.02px;
	  margin: 0 auto;
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
	
	@media (max-width: 768px) {
	  .box__column {
	    -webkit-box-flex: 1;
	        -ms-flex: 1 1 100%;
	            flex: 1 1 100%;
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
	  max-width: 492px;
	  margin: 0 auto;
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
	  bottom: 0;
	  left: 0;
	  background-color: rgba(255, 255, 255, 0.9);
	  margin: 6px 6px 6px 6px;
	  border-radius: 10px;
	  padding: 10px;
	}
	
	.item-box__descr {
	  text-align: left;
	  text-decoration: none;
	  font-weight: bold;
	  line-height: 1.4;
	  font-size: 19px;
	  min-width: 100%;
	  padding: 0px 60px 0px 0px;
	  overflow: hidden;
	  -o-text-overflow: ellipsis;
	     text-overflow: ellipsis;
	  display: -moz-box;
	  display: -webkit-box;
	  -webkit-line-clamp: 4;
	  -webkit-box-orient: vertical;
	  line-clamp: 4;
	  box-orient: vertical;
	  position: relative;
	}
	
	.item-box__descr::after {
	  content: '';
	  position: absolute;
	  width: 40px;
	  height: 40px;
	  top: 50%;
	  right: 0px;
	  background: url("../assets/images/arrow_blue.svg") 0 0/contain no-repeat;
	  -webkit-transform: translate(0, -50%);
	      -ms-transform: translate(0, -50%);
	          transform: translate(0, -50%);
	}
	
	@media (max-width: 1280px) {
	  .item-box__descr {
	    font-size: 16px;
	  }
	}
	
	@media (max-width: 1024px) {
	  .item-box__descr {
	    font-size: 14px;
	    line-height: 1.2;
	  }
	}
	
	@media (max-width: 768px) {
	  .item-box__descr {
	    font-size: 16px;
	  }
	}
	
	.item-box__shadow {
	  display: none;
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
}
</style>