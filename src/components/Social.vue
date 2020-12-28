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
.social {
	.container {
	  padding: 30px 10px;
	  max-width: 1536.05px !important;
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
	  -webkit-box-flex: 0;
	      -ms-flex: 0 1 33.333%;
	          flex: 0 1 33.333%;
	  padding: 0px 10px;
	  display: -webkit-box;
	  display: -ms-flexbox;
	  display: flex;
	  margin: 0px 0px 25px 0px;
	}
	
	@media (max-width: 750px) {
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
	}
	
	@media (max-width: 750px) {
	  .item-box {
	    min-width: 100%;
	  }
	}
	
	.item-box__image {
	  position: relative;
	  padding: 0px 0px 66.87% 0px;
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
	  border: 1px solid #ddd;
	  border-radius: 0 0 4px 4px;
	  overflow: hidden;
	}
	
	.item-box__descr {
	  font-weight: 600;
	  line-height: 20px;
	  -webkit-box-flex: 1;
	      -ms-flex: 1 1 auto;
	          flex: 1 1 auto;
	  margin: 0px 0px 15px 0px;
	  padding: 0px 0px 15px 0px;
	  border-bottom: 1px solid #dddddd;
	}
	
	.item-box__shadow {
	  display: none;
	}
	
	.item-box__btn {
	  display: none;
	}
	
	.item-box__else {
	  color: #365899;
	}
	
	.item-box__top {
	  position: absolute;
	  width: 100%;
	  top: 0;
	  left: 0;
	  display: -webkit-box;
	  display: -ms-flexbox;
	  display: flex;
	  z-index: 1;
	  padding: 10px;
	  background: -webkit-gradient(linear, left top, left bottom, from(rgba(0, 0, 0, 0.75)), to(rgba(0, 0, 0, 0)));
	  background: -o-linear-gradient(top, rgba(0, 0, 0, 0.75) 0%, rgba(0, 0, 0, 0) 100%);
	  background: linear-gradient(to bottom, rgba(0, 0, 0, 0.75) 0%, rgba(0, 0, 0, 0) 100%);
	}
	
	.item-box__icon {
	  position: relative;
	  height: 32px;
	  width: 32px;
	}
	
	.item-box__icon img {
	  position: absolute;
	  width: 100%;
	  height: 100%;
	  top: 0;
	  left: 0;
	  -o-object-fit: contain;
	     object-fit: contain;
	}
	
	.item-box__name {
	  margin: 0px 0px 0px 10px;
	  color: #fff;
	  font-weight: 600;
	  text-align: left;
	}
	
	.item-box__subtitle {
	  font-weight: 500;
	}
	
	.item-box__bottom {
	  display: none;
	}
	
	.item-box__menu {
	  width: 22px;
	  height: 22px;
	  background: url("../assets/images/menu.png") center/contain no-repeat;
	}
	
	.item-box__socials {
	  display: -webkit-box;
	  display: -ms-flexbox;
	  display: flex;
	}
	
	.item-box__social {
	  padding: 0px 23px;
	  line-height: 1.4;
	  position: relative;
	}
	
	.item-box__social::before {
	  content: '';
	  position: absolute;
	  width: 100%;
	  height: 100%;
	  top: 0px;
	  left: 0;
	  -o-object-fit: contain;
	     object-fit: contain;
	}
	
	@media (max-width: 1024px) {
	  .item-box__social {
	    font-size: 12px;
	  }
	  .item-box__social::before {
	    top: -2px;
	  }
	}
	
	.item-box__likes::before {
	  background: url("../assets/images/likes.png") 0 0 no-repeat;
	}
	
	.item-box__comments::before {
	  background: url("../assets/images/comments.png") 0 0 no-repeat;
	}
	
	.item-box__refs::before {
	  background: url("../assets/images/refs.png") 0 0 no-repeat;
	}
}
</style>