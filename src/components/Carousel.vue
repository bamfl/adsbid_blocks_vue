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

.carousel {
	.container {
	padding: 30px 10px;
	position: relative;
	overflow: hidden;
	}

	.arrow {
	  position: absolute;
	  z-index: 100;
	  top: 50%;
	  font-size: 0;
	  width: 44px;
	  height: 68px;
	  background-color: #fff !important;
	  border-radius: 4px;
	  -webkit-transform: translate(0, -50%);
	  -ms-transform: translate(0, -50%);
	  transform: translate(0, -50%);
	  -webkit-transition: all 0.5s;
	  -o-transition: all 0.5s;
	  transition: all 0.5s;
	  -webkit-box-shadow: 0px 0px 1px 1px rgba(0, 0, 0, 0.1);
	  box-shadow: 0px 0px 1px 1px rgba(0, 0, 0, 0.1);
	  cursor: pointer;
	}
	
	.arrow.prev {
	  left: -50px;
	}
	
	.arrow.prev::before {
	  content: '';
	  position: relative;
	  top: 50%;
	  width: 12px;
	  height: 18px;
	  border-style: solid;
	  border-width: 9px 12px 9px 0;
	  border-color: transparent #000 transparent transparent;
	  margin: 0px 3px 0px 0px;
	}
	
	.arrow.next {
	  right: -50px;
	}
	
	.arrow.next::before {
	  content: '';
	  position: relative;
	  width: 12px;
	  height: 18px;
	  top: 50%;
	  border-style: solid;
	  border-width: 9px 0 9px 12px;
	  border-color: transparent transparent transparent #000;
	  margin: 0px 0px 0px 3px;
	}
	
	.box__row {
	  display: -webkit-box;
	  display: -ms-flexbox;
	  display: flex;
	  overflow-x: scroll;
	  margin: 0 -8px;
	  padding: 0px 10px 0px 0px;
	}
	
	@media (min-width: 1024px) {
	  .box__row:hover .arrow.prev {
	    left: 40px;
	  }
	  .box__row:hover .arrow.next {
	    right: 40px;
	  }
	}
	
	@media (max-width: 1023px) {
	  .box__row .arrow.prev {
	    left: 35px;
	  }
	  .box__row .arrow.next {
	    right: 35px;
	  }
	}
	
	@media (max-width: 599px) {
	  .box__row .arrow.prev {
	    left: 40px;
	  }
	  .box__row .arrow.next {
	    right: 40px;
	  }
	}
	
	@media (max-width: 425px) {
	  .box__row .arrow {
	    display: none !important;
	  }
	  .box__row .arrow.prev {
	    left: 15px;
	  }
	  .box__row .arrow.next {
	    right: 15px;
	  }
	}
	
	.box__column {
	  padding: 0 8px;
	  -webkit-box-flex: 0;
	      -ms-flex: 0 1 20%;
	          flex: 0 1 20%;
	}
	
	.item-box {
	  position: relative;
	  display: block;
	  border-radius: 4px;
	  overflow: hidden;
	  min-width: 192px;
	}
	
	.item-box__image {
	  position: relative;
	  height: 300px;
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
	
	.item-box__top {
	  display: none;
	}
	
	.item-box__text {
	  position: absolute;
	  width: 100%;
	  bottom: 0;
	  left: 0;
	  background: -webkit-gradient(linear, left bottom, left top, from(#000), to(rgba(0, 0, 0, 0)));
	  background: -o-linear-gradient(bottom, #000, rgba(0, 0, 0, 0));
	  background: linear-gradient(0deg, #000, rgba(0, 0, 0, 0));
	}
	
	.item-box__descr {
	  color: #fff;
	  font-weight: 600;
	  font-size: 16px;
	  line-height: 1.2;
	  margin: 12px;
	  text-align: left;
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
	
	.item-box__else {
	  display: none;
	}
	
	.item-box__socials {
	  display: none;
	}
	
	.item-box__bottom {
	  display: none;
	}
	
	.item-box__btn {
	  display: none;
	}
}
</style>