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
.horizontal_6 {
	.box {
	  margin: 10px 0px 0px 0px;
	  overflow: hidden;
	}
	
	.container {
		margin: 30px 0px 0px 0px !important;
		max-width: 100% !important;
	}
	
	.box__row {
	  display: -webkit-box;
	  display: -ms-flexbox;
	  display: flex;
	  -ms-flex-wrap: wrap;
	      flex-wrap: wrap;
	  margin: 0 -5px;
	}
	
	.box__column {
	  -webkit-box-flex: 0;
	      -ms-flex: 0 1 33.333%;
	          flex: 0 1 33.333%;
	  padding: 0 5px;
	  margin: 0px 0px 10px 0px;
	}
	
	@media (max-width: 480px) {
	  .box__column {
	    -webkit-box-flex: 1;
	        -ms-flex: 1 1 100%;
	            flex: 1 1 100%;
	  }
	}
	
	.container {
	  max-width: 100%;
	  padding: 0 10px;
	}
	
	.arrow {
	  display: none;
	}
	
	.item-box {
	  min-width: 100%;
	}
	
	.item-box__image {
	  position: relative;
	  padding: 0px 0px 60% 0px;
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
	
	.item-box__descr {
	  margin: 5px 0px 0px 0px;
	  font-size: 20px;
	  line-height: 1.2;
	  font-weight: 600;
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
	
	@media (max-width: 768px) {
	  .item-box__descr {
	    font-size: 16px;
	  }
	}
	
	.item-box__descr:hover {
	  color: #529299;
	}
	
	.item-box__else {
	  display: none;
	}
	
	.item-box__socials {
	  display: none;
	}
	
	.item-box__date {
	  display: none;
	}
	
	.item-box__btn {
	  display: none;
	}
}
</style>