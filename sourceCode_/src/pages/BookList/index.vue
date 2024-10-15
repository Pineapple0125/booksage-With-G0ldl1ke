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
								<li><router-link :to="{name:'ShoppingCart'}" data-toggle="dropdown" data-hover="dropdown"><i class="icon-basket-loaded icons" aria-hidden="true"></i></router-link><span class="subno">0</span><strong>Your Cart</strong></li>
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
											<li >
												<a href="#/BookList" @click="filterItems('Fiction')"><img src="assets/images/menu-icon1.png" alt="menu-icon1" style="height: 20px; width: 20px;" /> Fiction </a>
											</li>
											<li >
												<a href="#/BookList" @click="filterItems('Science & Technology')"><img src="assets/images/menu-icon2.png" alt="menu-icon2" style="height: 20px; width: 20px;" /> Science & Technology </a>
											</li>
											<li>
												<a href="#/BookList" @click="filterItems('History & Biography')"><img src="assets/images/menu-icon3.png" alt="menu-icon3" style="height: 20px; width: 20px;" /> History & Biography </a>
											</li>
											<li >
												<a href="#/BookList" @click="filterItems('Children & Young Adult')"><img src="assets/images/menu-icon4.png" alt="menu-icon4" style="height: 20px; width: 20px;" /> Children & Young Adult </a>
											</li>
											
											<li>
											    <a href="#/BookList" @click="filterItems('Travel & Adventure')"><img src="assets/images/menu-icon5.png" alt="menu-icon2" style="height: 20px; width: 20px;" /> Travel & Adventure </a>
											</li>
											<li>
											    <a href="#/BookList" @click="filterItems('Art & Photography')"><img src="assets/images/menu-icon6.png" alt="menu-icon2" style="height: 20px; width: 20px;"/> Art & Photography </a>
											</li>
											<li>
											    <a href="#/BookList" @click="filterItems('Health & Beauty')"><img src="assets/images/menu-icon7.png" alt="menu-icon2" style="height: 20px; width: 20px;" /> Health & Beauty </a>
											</li>
											<li>
												<a href="#/BookList" @click="filterItems('Business & Economics')"><img src="assets/images/menu-icon8.png" alt="menu-icon2" style="height: 20px; width: 20px;" /> Business & Economics </a>
											</li>
											<li>
											    <a href="#/BookList" @click="filterItems('Philosophy & Religion')"><img src="assets/images/menu-icon9.png" alt="menu-icon2" style="height: 20px; width: 20px;" /> Philosophy & Religion </a>
											</li>
											<li>
											    <a href="#/BookList" @click="filterItems('Regional Literature Preferences')"><img src="assets/images/menu-icon10.png" alt="menu-icon2" style="height: 20px; width: 20px;" /> Regional Literature Preferences </a>
											</li>
											<li>
											    <a href="#/BookList" @click="filterItems(' ')"><img src="assets/images/menu-icon11.png" alt="menu-icon2" style="height: 20px; width: 20px;" />All</a>
											</li>
										</ul>
									</li>
									<li><a href="#/Home">Home</a></li>
									<li><a href="#/BookList" style="color: rgb(177, 30, 34);">BookList</a></li>
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
			<div class="container">
				<div class="row">
					<div class="col-md-12">
						<ol class="breadcrumb">
							<li class="breadcrumb-item"><a href="#/Home">Home</a></li>
							<li class="breadcrumb-item active">BookList</li>
						</ol>
					</div>
					<div class="col-sm-3 col-md-3">
						<div class="weight">
							<div class="title">
								<h2>screening</h2>
							</div>
							<div class="product-categories">
								<ul>
									<li><a href="#/BookList" @click="soutBypriceUp()" >Upward Price order  <span><i class="fa fa-angle-right" aria-hidden="true"></i></span></a></li>
									<li><a href="#/BookList" @click="soutBypriceDown()" >Falling Price order   <span><i class="fa fa-angle-right" aria-hidden="true"></i></span></a></li>
									<li><a href="#/BookList" @click="soutBysales()">Sales priority <span><i class="fa fa-angle-right" aria-hidden="true"></i></span></a></li>
								</ul>
							</div>
						</div>

					</div>
					<div class="col-sm-9 col-md-9">
						<div class="grid-spr">
							<div class="col-sm-6 col-md-8 text-right"> <strong>CATEGORIES <span class="title_mark">of 20 relults</span></strong> </div>
						</div>
						<div v-for="book in books" :key="book.id">
						      <BookItem :book="book"></BookItem>
						</div>						
	
					</div>
				</div>
			</div>
			<!-- /.grid-shop -->
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
	import BookItem from "./BookItem/index.vue"
	
	
		export default {
			name:"BookList",
			components:{
				BookItem
			},
			data() {
				return{
					books: [],
				}
			},
			methods: {
			    filterItems(category) {
			      this.currentCategory = category;
			
			      // 遍历所有 item，根据分类显示/隐藏
			      const items = document.getElementsByClassName('book-item');
			      for (const item of items) {
			        const itemCategory = item.getAttribute('data-category');
			        if (this.currentCategory === null || itemCategory.includes(this.currentCategory)) {
			          item.style.display = 'block';
			        } else {
			          item.style.display = 'none';
			        }
			      }
			    },
				soutBypriceUp(){
					this.books = this.books.sort((a, b) => parseFloat(a.price.slice(1)) - parseFloat(b.price.slice(1)));
				},
				soutBypriceDown(){
					this.books = this.books.sort((a, b) => parseFloat(b.price.slice(1)) - parseFloat(a.price.slice(1)));
				},
				soutBysales(){
					this.books = this.books.sort((a, b) => parseInt(b.sales) - parseInt(a.sales));
				},
			},
			mounted() {
				const currentCategory = this.$route.query.category;
				if(currentCategory){
					this.filterItems(currentCategory);
				}
				this.$axios({
				  method: "post",  // 改为POST方法
				  url: 'http://127.0.0.1:5000/api/send_data_bookList',
				  data: {
				  // 这里放入需要发送的数据
				  }
				}).then(response => {
				  // 在控制台打印响应数据
				  console.log(response.data);
				  this.books = response.data;
				})	
				console.log("every time fresh the page=>", this.userInfo);
				
				
				
				
				
				
				
			},
		}
		
</script>
<style scoped></style>