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
.with_date {
	.container {
	  padding: 30px 10px;
	  max-width: 1536.02px;
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
	  margin: 0 -10px;
	}
	
	.box__column {
	  padding: 0px 10px;
	  display: -webkit-box;
	  display: -ms-flexbox;
	  display: flex;
	  margin: 0px 0px 25px 0px;
	}
	
	@media (max-width: 600px) {
	  .box__column {
	    -webkit-box-flex: 1;
	        -ms-flex: 1 1 100%;
	            flex: 1 1 100%;
	  }
	}
	
	.item-box {
	  margin: 0 auto;
	  max-width: 492px;
	  display: -webkit-box;
	  display: -ms-flexbox;
	  display: flex;
	  -webkit-box-orient: vertical;
	  -webkit-box-direction: normal;
	      -ms-flex-direction: column;
	          flex-direction: column;
	  border-radius: 4px;
	  overflow: hidden;
	  -webkit-box-shadow: 0 4px 15px rgba(0, 0, 0, 0.07), 0 5px 15px rgba(0, 0, 0, 0.07);
	          box-shadow: 0 4px 15px rgba(0, 0, 0, 0.07), 0 5px 15px rgba(0, 0, 0, 0.07);
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
	  padding: 15px;
	  -webkit-box-flex: 1;
	      -ms-flex: 1 1 auto;
	          flex: 1 1 auto;
	  text-align: left;
	  display: -webkit-box;
	  display: -ms-flexbox;
	  display: flex;
	  -webkit-box-orient: vertical;
	  -webkit-box-direction: normal;
	      -ms-flex-direction: column;
	          flex-direction: column;
	  color: #202125;
	}
	
	.item-box__descr {
	  font-size: 18px;
	  line-height: 1.2;
	  font-weight: 400;
	  -webkit-box-flex: 1;
	      -ms-flex: 1 1 auto;
	          flex: 1 1 auto;
	  margin: 0px 0px 15px 0px;
	  overflow: hidden;
	  -o-text-overflow: ellipsis;
	     text-overflow: ellipsis;
	  display: -moz-box;
	  display: -webkit-box;
	  -webkit-line-clamp: 5;
	  -webkit-box-orient: vertical;
	  line-clamp: 5;
	  box-orient: vertical;
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
	  display: -webkit-box;
	  display: -ms-flexbox;
	  display: flex;
	  -webkit-box-pack: justify;
	      -ms-flex-pack: justify;
	          justify-content: space-between;
	  -webkit-box-align: center;
	      -ms-flex-align: center;
	          align-items: center;
	}
	
	.item-box__menu {
	  width: 22px;
	  height: 22px;
	  background: url("../assets/images/menu.png") center/contain no-repeat;
	}
	
	.item-box__icon {
	  display: none;
	}
	
	.item-box__socials {
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