<template>
	<body>
	<!--  Preloader  -->
		<div id="preloader">
			<div id="loading"> </div>
		</div>
		<header class="header2">
			<!--  top-header  -->
		<div class="top-header">
			<div class="container">
			        
			    <div class="col-md-6">
			        <div class="top-header-left">
			        </div>
			    </div>
			    <div class="col-md-6">
			        <div class="top-header-right">
			            <ul>
			                <li>
			                    <div class="dropdown">
			                        <a href="#" class="btn btn-default dropdown-toggle" data-toggle="dropdown" data-hover="dropdown">
			                            <i class="icon-settings icons" aria-hidden="true"></i> Setting
			                        </a>
			                        <ul class="dropdown-menu">
			                            <li><a href="#">My Account</a></li>
			                            <li><a href="#">Change Password</a></li>
			                            <li><a href="#">Change Address</a></li>
			                        </ul>
			                    </div>
			                </li>
			            </ul>
			        </div>
			    </div>
			</div>
				<!--  /top-header  -->
			</div>
			<section class="top-md-menu">
				<div class="container">
					<div class="col-sm-3">
						<div class="logo">
							 <h6><img src="https://pic.imgdb.cn/item/65717325c458853aeff3d236.png" style="height: 150px; width: 150px;" alt="logo" /></h6>
						</div>
					</div>
					<div class="col-sm-6">
						<!-- Search box Start -->
						<form>
							<div class="well carousel-search hidden-phone">
								<div class="btn-group">
									<a class="btn dropdown-toggle btn-select" data-toggle="dropdown" href="#">All Categories <span class="caret"></span></a>
									<ul class="dropdown-menu">
										<li><a href="#">Item I</a></li>
										<li><a href="#">Item II</a></li>
										<li><a href="#">Item III</a></li>
										<li class="divider"></li>
										<li><a href="#">Other</a></li>
									</ul>
								</div>
								<div class="search">
									<input type="text" placeholder="Where prodect" />
								</div>
								<div class="btn-group">
									<button type="button" id="btnSearch" class="btn btn-primary"><i class="fa fa-search" aria-hidden="true"></i></button>
								</div>
							</div>
						</form>
						<!-- Search box End -->
					</div>
					<div class="col-sm-3">
						<!-- cart-menu -->
						<div class="cart-menu">
							<ul>
								<li class="dropdown">
									<router-link :to="{name:'ShoppingCart'}" data-toggle="dropdown" data-hover="dropdown">
										<i class="icon-basket-loaded icons" aria-hidden="true"></i>
									</router-link>
									<span class="subno" ref="subnoSpan" >0</span>
									<strong>Your Cart</strong>
								</li>
							</ul>
						</div>
						<!-- cart-menu End -->
					</div>
					<div class="main-menu">
						<!--  nav  -->
						<nav class="navbar navbar-inverse navbar-default">
							<!-- Brand and toggle get grouped for better mobile display -->
							<div class="navbar-header">
								<button type="button" class="navbar-toggle collapsed" data-toggle="collapse" data-target="#bs-example-navbar-collapse-1"> <span class="sr-only">Toggle navigation</span> <span class="icon-bar"></span> <span class="icon-bar"></span> <span class="icon-bar"></span> </button>
							</div>
							<!-- Collect the nav links, forms, and other content for toggling -->
							<div class="collapse navbar-collapse" id="bs-example-navbar-collapse-1" data-hover="dropdown" data-animations=" fadeInLeft fadeInUp fadeInRight">
								<ul class="nav navbar-nav">
									<li class="all-departments dropdown"> <a href="index.html" class="dropdown-toggle" data-toggle="dropdown" role="button" aria-expanded="false"><span> Shop By Department</span> <i class="fa fa-bars" aria-hidden="true"></i> </a>
										<ul class="dropdown-menu dropdownhover-bottom" role="menu">
											<li>
											    <router-link :to="{ name: 'BookList', query: { category: 'Fiction' } }">
													<img src="assets/images/menu-icon1.png" alt="menu-icon1" style="height: 20px; width: 20px;" /> Fiction
											    </router-link>
											</li>
											<li>
											    <router-link :to="{ name: 'BookList', query: { category: 'Science & Technology' } }">
													<img src="assets/images/menu-icon2.png" alt="menu-icon2" style="height: 20px; width: 20px;" /> Science & Technology
												</router-link>
											</li>
											<li>
												<router-link :to="{ name: 'BookList', query: { category: 'History & Biography' } }">
													<img src="assets/images/menu-icon3.png" alt="menu-icon3" style="height: 20px; width: 20px;" /> History & Biography
												</router-link>
											</li>
											<li>
												<router-link :to="{ name: 'BookList', query: { category: 'Children & Young Adult' } }">
													<img src="assets/images/menu-icon4.png" alt="menu-icon4" style="height: 20px; width: 20px;" /> Children & Young Adult
												</router-link>
											</li>
											<li>
											    <router-link :to="{ name: 'BookList', query: { category: 'Travel & Adventure' } }">
													<img src="assets/images/menu-icon5.png" alt="menu-icon5" style="height: 20px; width: 20px;" /> Travel & Adventure
												</router-link>
											</li>
											<li>
												<router-link :to="{ name: 'BookList', query: { category: 'Art & Photography' } }">
													<img src="assets/images/menu-icon6.png" alt="menu-icon6" style="height: 20px; width: 20px;" /> Art & Photography
												</router-link>
											</li>
											<li>
												<router-link :to="{ name: 'BookList', query: { category: 'Health & Beauty' } }">
													<img src="assets/images/menu-icon7.png" alt="menu-icon7" style="height: 20px; width: 20px;" /> Health & Beauty
												</router-link>
											</li>
											<li>
												<router-link :to="{ name: 'BookList', query: { category: 'Business & Economics' } }">
													<img src="assets/images/menu-icon8.png" alt="menu-icon8" style="height: 20px; width: 20px;" /> Business & Economics
												</router-link>
											</li>
											<li>
												<router-link :to="{ name: 'BookList', query: { category: 'Philosophy & Religion' } }">
													<img src="assets/images/menu-icon9.png" alt="menu-icon9" style="height: 20px; width: 20px;" /> Philosophy & Religion
												</router-link>
											</li>
											<li>
												<router-link :to="{ name: 'BookList', query: { category: 'Regional Literature Preferences' } }">
													<img src="assets/images/menu-icon10.png" alt="menu-icon10" style="height: 20px; width: 20px;" /> Regional Literature Preferences
												</router-link>
											</li>
											<li>
												<router-link :to="{ name: 'BookList', query: { category: ' ' } }">
													<img src="assets/images/menu-icon11.png" alt="menu-icon11" style="height: 20px; width: 20px;" /> All
												</router-link>
											</li>
										</ul>
									</li>
									<li><a href="#/Home">Home</a></li>
									<li><a href="#/BookList">BookList</a></li>
								</ul>
								<!-- /.navbar-collapse -->
							</div>
						</nav>
						<!-- /nav end -->
					</div>
				</div>
			</section>
		</header>
		<!-- newsletter -->
		<section class="grid-shop">
			<!-- .grid-shop -->
			<div class="container"  v-for="(product, index) in products" :key="index">
				<div class="row" v-if="String(product.productID) === String(receivedValue)">
					<div class="col-md-12">
						<ol class="breadcrumb">
							<li class="breadcrumb-item"><a href="#/Home">Home</a></li>
							<li class="breadcrumb-item active">Shop Detail.</li>
						</ol>
						<div class="row">						
							<!-- left side -->
							<div class="col-sm-5 col-md-5">
								<!-- product gallery -->
								<div class="connected-carousels">
									<div class="stage">
										<div class="carousel carousel-stage" >
												<ul >
													<li style="height: 600px; width: 500px;" v-for="(image, imageIndex) in product.productImages" :key="imageIndex">
														<img class="zoom_01" :src="image.src" :data-zoom-image="image.src" :alt="image.alt" />
													</li>											
												</ul>
										</div>

									</div>
	
									<div class="navigation">
										<a href="#/ShopDetail" class="prev prev-navigation">&lsaquo;</a>
										<a href="#/ShopDetail" class="next next-navigation">&rsaquo;</a>
										<div class="carousel carousel-navigation" >
											<ul >
												<li v-for="(image, imageIndex) in product.productImages" :key="imageIndex">
													<img :src="image.src" width="110" height="110" alt="">
												</li>											
											</ul>
										</div>
									</div>
								</div>
	
								<!-- / product gallery -->
							</div>
							<!-- left side -->
							<!-- right side -->
							<div class="col-sm-7 col-md-7" >
								<!-- .pro-text -->
								<div class="pro-text product-detail">
									<!-- /.pro-img -->
									<span class="span1">{{product.catogory}}</span>
										<h4>{{ product.name }}</h4>
									<div class="star2">
										<ul>
											<li class="yellow-color"><i class="fa fa-star" aria-hidden="true"></i></li>
											<li class="yellow-color"><i class="fa fa-star" aria-hidden="true"></i></li>
											<li class="yellow-color"><i class="fa fa-star" aria-hidden="true"></i></li>
											<li class="yellow-color"><i class="fa fa-star" aria-hidden="true"></i></li>
											<li><i class="fa fa-star" aria-hidden="true"></i></li>
											<li> <a>Auther: {{product.auther}}</a></li>
											<li> <a>Publishers: {{product.Publishers}}</a></li>
										</ul>
									</div>
									<p><strong>${{product.currentPrice}}</strong><span class="line-through">${{product.originalPrice}}</span></p>
									<p class="in-stock">Availability:   <span>In Stock</span></p>
									<p>{{product.ProductIntroduction}}</p>							
									<form>
										<div class="numbers-row">
											<input type="text" name="french-hens" id="french-hens" value="1" style="border: none;">
										</div>
									</form>
									<a @click="showToast() " class="addtocart2">Add to cart</a>
									<div class="tag">
										<p style="padding-top: 20px;"> </p>
										<p>Categories: <a v-for="(category, index) in product.category" :key="index">{{category}}</a></p>
									</div>
								</div>
								<!-- /.pro-text -->
							</div>
						</div>
					</div>
								<!-- right side -->
				</div>
				
				<!-- 用一种很丑陋的方法了解决了预加载问题  很丑陋的方法开始-->
				
				<div class="row" v-else-if="String(product.productID) === 'model'">
					<div class="col-md-12">
						<ol class="breadcrumb">
							<li class="breadcrumb-item"><a href="#/Home">Home</a></li>
							<li class="breadcrumb-item active">Shop Detail.</li>
						</ol>
						<div class="row">						
							<!-- left side -->
							<div class="col-sm-5 col-md-5">
								<!-- product gallery -->
								<div class="connected-carousels">
									<div class="stage">
										<div class="carousel carousel-stage" >
												<ul >
													<li style="height: 600px; width: 500px;" v-for="(image, imageIndex) in product.productImages" :key="imageIndex">
														<img class="zoom_01" :src="image.src" :data-zoom-image="image.src" :alt="image.alt" />
													</li>											
												</ul>
										</div>
				
									</div>
					
									<div class="navigation">
										<a href="#/ShopDetail" class="prev prev-navigation">&lsaquo;</a>
										<a href="#/ShopDetail" class="next next-navigation">&rsaquo;</a>
										<div class="carousel carousel-navigation" >
											<ul >
												<li v-for="(image, imageIndex) in product.productImages" :key="imageIndex">
													<img :src="image.src" width="110" height="110" alt="">
												</li>											
											</ul>
										</div>
									</div>
								</div>
					
								<!-- / product gallery -->
							</div>
							<!-- left side -->
							<!-- right side -->
							<div class="col-sm-7 col-md-7" >
								<!-- .pro-text -->
								<div class="pro-text product-detail">
									<!-- /.pro-img -->
									<span class="span1">{{product.category}}</span>
										<h4>{{ product.name }}</h4>
									<div class="star2">
										<ul>
											<li class="yellow-color"><i class="fa fa-star" aria-hidden="true"></i></li>
											<li class="yellow-color"><i class="fa fa-star" aria-hidden="true"></i></li>
											<li class="yellow-color"><i class="fa fa-star" aria-hidden="true"></i></li>
											<li class="yellow-color"><i class="fa fa-star" aria-hidden="true"></i></li>
											<li><i class="fa fa-star" aria-hidden="true"></i></li>
											<li> <a>Auther: {{product.auther}}</a></li>
											<li> <a>Publishers: {{product.Publishers}}</a></li>
										</ul>
									</div>
									<p><strong>${{product.currentPrice}}</strong><span class="line-through">${{product.originalPrice}}</span></p>
									<p class="in-stock">Availability:   <span>In Stock</span></p>
									<p>{{product.ProductIntroduction}}</p>							
									<form>
										<div class="numbers-row">
											<input type="text" name="french-hens" id="french-hens" value="1" style="border: none;">
										</div>
									</form>
									<a @click="showToast() " class="addtocart2">Add to cart</a>
									<div class="tag">
										<p style="padding-top: 20px;"> </p>
										<p>Categories: <a v-for="(category, index) in product.category" :key="index">{{category}}</a></p>
									</div>
								</div>
								<!-- /.pro-text -->
							</div>
						</div>
					</div>
								<!-- right side -->
				</div>
				
				
				<!-- 用一种很丑陋的方法了解决了预加载问题  很丑陋的方法结束-->
				
				
				
			</div>
			<!-- /.grid-shop -->
		</section>
		<!-- <notifications></notifications> -->
		<section class="all-product">
            <div class="container">
                <div class="row">
                    <div class="title">
                        <h2>Recommendation</h2>
                        <ul class="nav nav-tabs etabs">
                            <li class="active"><a data-toggle="tab" href="#phones">Hot Sell</a></li>
                        </ul>
                    </div>
                    <div class="electonics">
                        <div class="product-list">
                            <div class="bdr" v-for="product in products_hot" :key="product.id">
                                <div class="e-product">
                                    <div class="pro-img">
                                        <sup class="sale-tag" v-if="product.saleTag">{{ product.saleTag }}</sup>
                                        <img :src="product.imgUrl" style="padding: 10px;" :alt="product.title">
                                        <div class="hover-icon" @click="addRelation(product.title)">
                                            <router-link :to="{ name: 'ShopDetail', query: { index: product.id, bookname: product.title } }"
											  target="_blank">
												<i class="fa fa-search" aria-hidden="true"></i>
											 </router-link>
                                        </div>
                                    </div>
                                    <div class="pro-text-outer">
                                        <span>{{ product.author }}</span>
                                        <router-link :to="{ name: 'ShopDetail', query: { index: product.id, bookname: product.title } }"
											  target="_blank">
											<h4>{{ truncateTitle(product.title) }}</h4>
                                        </router-link>
                                        <p class="wk-price">{{ product.price }}</p>
                                        <a href="#" class="add-btn">Add to cart</a>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <!-- 同样修改其他 tab-pane 内容中的 .bdr 类的容器宽度 -->
                    </div>
                </div>
            </div>
        </section>
		<p id="back-top"> <a href="#top"><i class="fa fa-chevron-up" aria-hidden="true"></i></a> </p>
	</body>
	
</template>

<script>
	import "./assets/css/bootstrap.min.css";
	import "./assets/css/bootstrap-dropdownhover.min.css";
	import "./assets/font/css/font-awesome.min.css";
	import "./assets/simple-line-icon/css/simple-line-icons.css";
	import "./assets/stroke-gap-icons/stroke-gap-icons.css";
	import "./assets/css/animate.min.css";
	import "./assets/css/style.css";
	import "./assets/css/jcarousel.connected-carousels.css";
	import "./assets/css/baguetteBox.css";
	import "./assets/owl-carousel/owl.carousel.css";
	import "./assets/owl-carousel/owl.theme.css";
	
		export default {
			name:"ShopDetall",
			data() {
			    return {
			      receivedValue: null,
				  bookName:null,
				  products:[
					  {
					    productID:'model',
					    category:"",
					    name:"",
					    auther:"",
					    Publishers: "",
					    currentPrice:1.00,
					    originalPrice:1.00,
					    ProductIntroduction: "",
					    productImages: [
					  		{ src: "", alt: "qoute-icon" },
					  		{ src: "", alt: "qoute-icon" },
					  		{ src: "", alt: "qoute-icon" },
					  		{ src: "", alt: "qoute-icon" },
					  		{ src: "", alt: "qoute-icon" },
					  		{ src: "", alt: "qoute-icon" },
					  	],
					  },
				  ],
				  products_hot:[]
			    };
			  },
		  methods: {
		      showToast() {
				  
				const spanElement = this.$refs.subnoSpan
				// 获取当前标签的文本内容并转换为整数
				let currentValue = parseInt(spanElement.innerHTML);
				// 加一
				let newValue = currentValue + 1;
				// 更新标签的内容
				spanElement.innerHTML = newValue.toString();
				
				this.$emit('updateUserInfo', this.receivedValue);
				
				sessionStorage.setItem("index",this.receivedValue);
				
				this.$notify({
				  title: 'succeed',
				  message: this.$createElement('i', { style: 'color: rgb(177, 30, 34)' }, 'Add to cart successfully')
				});
		      },
			  addRelation(target_bookName){
				console.log(this.bookName)
				console.log(target_bookName)

				this.$axios({
				  method: "post",  // 改为POST方法
				  url: 'http://127.0.0.1:5000/api/send_data_bookDetail_add_relation',
				  data: {
						bookA: this.bookName,
						bookB: target_bookName
				  }
				}).then(response => {
				  // 在控制台打印响应数据
				  console.log(response);
				})
				
				
			},
			truncateTitle(title) {
			      if (title.length > 20) {
			        return title.substring(0, 20) + '...';
			      }
			      return title;
			},
		    },
			  
			mounted() {
				console.log(this.receivedValue)
				this.$axios({
				  method: "post",  // 改为POST方法
				  url: 'http://127.0.0.1:5000/api/send_data_bookdetail',
				  data: {
				  // 这里放入需要发送的数据
				  }
				}).then(response => {
				  // 在控制台打印响应数据
				  
				  this.products = response.data;
				  console.log(this.products);
				});
				
				this.receivedValue = this.$route.query.index;
				this.bookName = this.$route.query.bookname;
				
				
				
				this.$axios({
				  method: "post",  // 改为POST方法
				  url: 'http://127.0.0.1:5000/api/send_data_bookDetail_recommend',
				  data: {
						bookName: this.bookName
				  }
				}).then(response => {
				  // 在控制台打印响应数据
				  this.products_hot = response.data;
				  console.log(this.products);
				})
			    
			}
			
			
		}
		
	
</script>

<style scoped>
.product-list {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    padding: 0;
    margin: 0 auto; 
    width: 100%; 
}

.bdr {
    flex: 0 0 23%; 
    margin: 1%; 
    box-sizing: border-box; 
    border: 1px solid #ccc; 
    border-radius: 10px;
    padding: 10px;
    background-color: white; 
    height: auto;
}

.electonics {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
    width: 100%;
    background-color: white; 
}

.e-product {
    box-shadow: none; 
    margin: 0;
    padding: 0;
}

.all-product {
	background: rgb(255, 255, 255) none repeat scroll 0 0;
	padding: 50px 0;
	border: 1px solid #ebebeb;
}
</style>
