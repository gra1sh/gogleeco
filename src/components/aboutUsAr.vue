<template>
	<div>
		<!-- about us -->
	<div id='About_us'>
		<div>
			<v-parallax src="/static/aboutUs.png">
				<v-layout
				      align-center
				      column
				      justify-center
				    >
				      <h1 class="display-2 font-weight-thick mb-3 Title bgTitle" >أحداث عالمية المستوى</h1>
				      <img class='gr'src='/static/GraphicElAbout.png' style="margin: auto;">
				    </v-layout>
			</v-parallax>
		</div>

		<v-layout row wrap>
		  <v-flex xs12 sm6>
			  <div >
			  	<v-container>
			  		<v-layout justify-center>
			  			<img src="/static/ICONus.png" style="height: 50px;">
			  		</v-layout>
			  		<h2 class="text-xs-center font-weight-thin or">رؤيتنا</h2>
			  		<v-container>
			  			<p class="text-xs-center"><span><img src='/static/logo.png' style="height:16px;"></span> &nbsp {{aboutUsTxt}}</p>
			  		</v-container>
			  	</v-container>
			  </div>
		  </v-flex>

		  <v-flex xs12 sm6>
			  <div>
			  	<v-container>
			  		<v-layout justify-center>
			  			<!-- <v-icon style='font-size: 50px; color: #ef8000;'>supervisor_account</v-icon> -->
			  			<img src="/static/ICONvision.png" style="height: 50px;">
			  		</v-layout>
			  		<h2 class="text-xs-center font-weight-thin or">من نحن</h2>
			  		<v-container>
			  			<p class="text-xs-center"><span><img src='/static/logo.png' style="height:16px;"></span> &nbsp{{visionTxt}}</p>
			  			<v-layout justify-center>
			  			<img src='/static/2030_LOGO.png' style="height: 60px;">
			  		</v-layout>
			  		</v-container>
			  	</v-container>
			  </div>
		  </v-flex>
		</v-layout>
	</div>

		<div>
		<div id='Our_values' >
			<v-parallax src="/static/2nd_bg.png" class='our_vals' >
				<v-layout
				      align-center
				      column
				    >

				      <h3 class=" display-1 or" style="padding: 10px;">قيمنا الجوهرية</h3>
				      <p class="hr caption" style="max-width:900px;"><span>&nbsp {{coreValues}} &nbsp</span></p>

				      <v-layout wrap>
					      <v-flex xs12 sm6>
					      	<div style=" float: right;" class='bg2el'>
					      		<v-container>
					      		<v-layout column align-center>
						      		<img src='/static/Icon_learning.png' style='height: 60px;'/>
						      		<p class="or" style="padding: 10px; margin:auto;">التعلم والتطور</p>
						      		<p class="text-xs-center" >{{LearningAndDev}}</p>
						      	</v-layout>
						      	</v-container>
					      	</div>
					      </v-flex>

					      <v-flex xs12 sm6>
					      	<div style="" class='bg2el'>
					      		<v-container>
					      		<v-layout column align-center>
						      		<img src='/static/icon_iniciative.png' style='height: 60px;'/>
						      		<p class="or" style="padding: 10px; margin:auto;">المبادرة والإبداع</p>
						      		<p class="text-xs-center" >{{initiativesTxt}}</p>
						      	</v-layout>
						      	</v-container>
					      	</div>
					      </v-flex>

					      <v-flex xs12 sm6>
					      	<div style=" float: right;" class='bg2el'>
					      		<v-container>
					      		<v-layout column align-center>
						      		<img src='/static/Icon_tech.png' style='height: 60px;'/>
						      		<p class="or" style="padding: 10px; margin:auto;">التقنية والابتكار</p>
						      		<p class="text-xs-center" >{{techText}}</p>
						      	</v-layout>
						      	</v-container>
					      	</div>
					      </v-flex>

					      <v-flex xs12 sm6>
					      	<div style="" class='bg2el'>
					      		<v-container>
					      		<v-layout column align-center>
						      		<img src='/static/Icon_partner.png' style='height: 60px;'/>
						      		<p class="or" style="padding: 10px; margin:auto;">الشراكة والتعاون</p>
						      		<p class="text-xs-center" >{{partnerTxt}}</p>
						      	</v-layout>
						      	</v-container>
					      	</div>
					      </v-flex>

					  </v-layout>

				    </v-layout>
			</v-parallax>
		</div>

			<div id='Services'>
				<v-layout align-center column>
					<h3 class=" display-1 or" style="padding: 10px;">خدماتنا</h3>
					<p class="hr2 caption" style="max-width:900px;"><span>&nbsp {{ourServices}} &nbsp</span></p>
				</v-layout>

				<div>
					<v-parallax src="/static/bg3.png" class='services' style='background: #f08000;'>
						<v-layout wrap>
							<v-flex xs6 sm4 v-for='d in ourServicesArray'>
								<div>
									<v-container>
										<v-layout column align-center>
											<img :src='`/static/${d.icon}`' style="height: 70px;" />
											<p class="black--text text-xs-center subheading" style="padding: 10px;">{{d.title}}</p>
										</v-layout>
									</v-container>
								</div>
							</v-flex>
						</v-layout>
					</v-parallax>
				</div>

			</div>

		</div>

		<div id='Contact_us'>
			<v-parallax src="/static/bg4.png" class='bg4 contact_us'>
				<v-layout column style='padding: 10px;'>
					<p class="display-1 or">لنبقى على تواصل!</p>
					<p class="body-2" style="max-width: 600px;">{{stayConnectedTxt}}</p>

					<v-layout row wrap>
					  <v-flex sm6 xs12>
					  		<div style="margin-top: 50px;">
							    <p class='display-1 or'>الرياض</p>
							    <p class="body-2">شارع موسى بن نصير ،<br> الرياض - المملكة العربية السعودية</p>
							</div>

							<div style='margin-top:50px;'>
								<v-layout>
									<img src='/static/Phone_Icon.png' style="height: 18px;">
									<p style="margin-left: 10px;">+966920009177</p>
								</v-layout>

								<v-layout>
									<img src='/static/Fax_Icon.png' style="height: 18px;">
									<p style="margin-left: 10px;">+9664177177</p>
								</v-layout>

								<v-layout>
									<img src='/static/email_icon.png' style="height: 18px;">
									<p style="margin-left: 10px;">info@gogleeco.com</p>
								</v-layout>
								
							</div>
					  </v-flex>
 
					  <v-flex sm6 xs12>
					  	<v-text-field
			  	            label="Solo"
			  	            single-line
			  	            solo
			  	            background-color='white'
			  	            light
			  	            color='black'
			  	            placeholder='الاسم الكامل'
			  	            style='opacity: 0.7'
			  	            v-model='contact.fullName'
					  	></v-text-field>

					  	<v-text-field
			  	            label="Solo"
			  	            single-line
			  	            solo
			  	            background-color='white'
			  	            light
			  	            color='black'
			  	            type='number'
			  	            placeholder='رقم الهاتف'
			  	            style='opacity: 0.7'
			  	            v-model='contact.phone'
					  	></v-text-field>

					  	<v-text-field
			  	            label="Solo"
			  	            single-line
			  	            solo
			  	            background-color='white'
			  	            light
			  	            color='black'
			  	            placeholder='البريد الإلكتروني'
			  	            :rules="[rules.required, rules.email]"
			  	            style='opacity: 0.7'
			  	            v-model='contact.email'
					  	></v-text-field>



					  	<v-text-field
			  	            label="Solo"
			  	            single-line
			  	            solo
			  	            background-color='white'
			  	            light
			  	            color='black'
			  	            placeholder='موضوع'
			  	            style='opacity: 0.7'
			  	            v-model='contact.subject'
					  	></v-text-field>

					  	<v-card class='white' style='opacity: 0.7'>
					  	 <div style='padding-left: 10px;'>
					  	   
					  	<v-textarea
					  	          name="input-7-1"
					  	          placeholder='كيف يمكننا مساعدتك؟'
					  	          color='black'
					  	          v-model='contact.disc'
					  	></v-textarea>
					  	 </div>
					  	</v-card>


					  		<v-btn class='black--text'style='background: #ef8000; margin-left: 0; margin-top: 10px;' @click='send'>إرسال</v-btn>

					  </v-flex>

					</v-layout>
				</v-layout>
			</v-parallax>
		</div>

		<v-card>
			<v-layout justify-center column align-center>
				<h3 class=" display-1 or" style="padding: 10px;">حدد لنا</h3>
				<p class="hr3 caption" style="max-width:900px;"><span>&nbsp شارع موسى بن نصير ، الرياض ، المملكة العربية السعودية &nbsp</span></p>
			</v-layout>

		</v-card>

		<GmapMap
		  :center="center"
		  :zoom="15"
		  style="width: 100%; height: 300px"
		>
		  <GmapMarker
		  
		    :position="center"
		    :clickable="true"
		    :draggable="true"
		    @click="center=m.position"
		  />
		</GmapMap>

		<!-- <img src='/static/map.png' style="width: 100%;"> -->



	</div>


</template>

<script>
import axios from 'axios'

	export default{
		data(){
			return{
				aboutUsTxt:`أن تكون شركة من الشركات السعودية العالمية الرائدة في تنظيم المؤتمرات والمعارض وابتكار المبادرات الوطنية الشبابيةالتي تساهم في رؤية 2030`,
				visionTxt:`أن تكون شركة من الشركات السعودية العالمية الرائدة في تنظيم المؤتمرات والمعارض وابتكار المبادرات الوطنية الشبابيةالتي تساهم في رؤية 2030`,
				coreValues:`تبقى قيمنا الأساسية هي حجر الزاوية لشركتنا وهي ما نعتمد عليه في نظام أخلاقيات العمل لدينا`,
				LearningAndDev:`خلق أفضل الأفكار الإبداعية وتشجيع طرح المبادرات الوطنية`,
				initiativesTxt:`خلق أفضل الأفكار الإبداعية وتشجيع طرح المبادرات الوطنية`,
				techText:` استخدام أحدث التقنيات وابتكارالتطبيقات التي تساهم في رفع كفاءة العمل`,
				partnerTxt:`نتعاون مع الجهات المحلية والعالمية والمؤسسات ذات الصلة لتطوير مجال المعارض والمؤتمرات`,
				ourServices:`نحن متخصصون في توفير الخدمات التالية بفعالية عالية`,
				stayConnectedTxt:`يسعدنا التواصل معك في كل وقت للاجابة على كل تساؤلاتك وتزويدك بكل ما تحتاجه لإنشاء حدث ناجح`,
				ourServicesArray:[
					{icon:`Icon_tech_design.png`,title:'التصميم الفني'},
					{icon:`Icon_media_production.png`,title:'الإنتاج الإعلامي'},
					{icon:`Icon_media_campaigns.png`,title:'الحملات الإعلامية'},
					{icon:`icon_telecommunication.png`,title:'الإتصالات'},
					{icon:`Icon_support_services.png`,title:'الخدمات المساندة'},
					{icon:`icon_spcial_events_management.png`,title:'إدارة الفعاليات الخاصة'}
				],

		        center: {lat:24.704341, lng:46.683830},
		        markers: [{lat:24.704341, lng:46.683830}],
		        places: [],
		        currentPlace: null,
		        contact:{
		        	fullName:'',
		        	phone:'',
		        	email:'',
		        	subject:'',
		        	disc:''
		        },
		        rules: {
                  required: value => !!value || 'Required.',
                  counter: value => value.length <= 20 || 'Max 20 characters',
                  email: value => {
                    const pattern = /^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/
                    return pattern.test(value) || 'Invalid e-mail.'
		        }
		    	}
			}
		},
		methods:{
			send(){
				let data = {
					fullName:this.contact.fullName,
		        	phone:this.contact.phone,
		        	email:this.contact.email,
		        	subject:this.contact.subject,
		        	disc:this.contact.disc
				}

				const body = `${data.fullName}\n${data.disc}\n${data.phone}\n${data.email}`;

				// console.log(data);

				const email = 'info@gogleeco.com';

				const e = (uri)=>{
					return encodeURI(uri)
				}

				window.location = `mailto:${email}?subject=${e(data.subject)}&body=${e(body)}`;

			}
		}
	}	
</script>



<style>
.v-messages__message{
	font-size: 18px;
	color: white;
	opacity: 1 !important;
}
.v-input input , .v-textarea textarea {
	color: black;
}

.bgTitle{
	font-size: 62px!important;
}

.gr{
	margin: auto;
    width: 430px;
    position: absolute;
}

.bg2el{
	max-width: 300px;
}

.hr { width:100%; text-align:center; border-bottom: 1px solid #ef8000; line-height:0.1em; margin:10px 0 20px; } 

.hr span { background:#000; padding:0 0.5px; }

.hr2 { width:100%; text-align:center; border-bottom: 1px solid #ef8000; line-height:0.1em; margin:10px 0 20px; } 

.hr2 span { background:#fff; padding:0 0.5px; }

.our_vals{
	height: 500px !important;
	background:black;
}

.services{
	height: 300px !important;
}

.contact_us{
	height: 615px !important;
	background-color:black; 
}



@media screen and (max-width:600px){
	.bgTitle{
		font-size: 30px !important;
	}

	.our_vals{
		height:860px !important;
	}

	.services{
		height: 500px !important;
	}

	.contact_us{
		height: 100% !important;
	}

	.gr{
		width: 250px;
	}

	.bg2el{
		max-width: 100%;
	}

	.hr{
		line-height: normal;
		border-bottom: 1px solid #000;
	}

	.hr2{
		line-height: normal;
		border-bottom: 1px solid #fff;
	}
}

.Title{
	font-family: 'Passion One', cursive !important;
}

.or{
	color: #ef8000;
}

.defuse{
	background-color: white;
	opacity: 0.7;
}






.hr3 { width:100%; text-align:center; border-bottom: 1px solid #ef8000; line-height:0.1em; margin:10px 0 20px; } 

.hr3 span { background:#fff; padding:0 0.5px; }
</style>