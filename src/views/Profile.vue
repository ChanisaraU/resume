<template>
  <div class="profile-page">
    <section class="section-profile-cover section-shaped my-0">
      <div class="shape shape-style-1 shape-primary shape-skew alpha-4">
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
        <span></span>
      </div>
    </section>

    <modal :show.sync="modals.modal1">
      <h6 slot="header" class="modal-title" id="modal-title-default">About Us</h6>

      <p>สวัสดีค่ะ ฉันชื่อชนิสรา อุตตมะเวทิน ชื่อเล่นว่ามิ้น  ตอนนี้ฉันกำลังหางานในด้านการเขียนโปรแกรมอยู่ </p>
      <p>ฉันจบการศึกษาจาก สาขาวิทยาการคอมพิวเตอร์ คณะวิทยาศาสตร์ มหาวิทยาลัยนเรศวร ค่ะ ในรั้วมหาวิทยาลัยฉันได้มีโอกาสได้เข้าร่วมกิจกรรมนอกเวลาเรียนเป็นพวกค่ายอาสาสอนเด็ก 
อบรมการเขียนโปรแกรมจากชมรม YoungSoft เคยเข้าร่วมสโมสรนิสิตคณะวิทยาศาสตร์  และทำงานระหว่างเรียนกับบริษัท Tesco Lotus  จากทุกอย่างที่กล่าวมาทำให้ฉันอดทน เข้ากับคนอื่นได้ดี  ได้พัฒนาด้านการสื่อสาร ทำงานได้อย่างหลากหลายค่ะ
นอกจากนี้ฉันยังได้มีโอกาสไปฝึกงานกับบริษัท Infonet (Thailand) Limited 
ได้รับผิดชอบหน้าที่เกี่ยวกับ it helpdesk และ tester และมีพี่เลี้ยงคอยดูแลและให้ความรู้ฉันค่ะ จากนั้นฉันได้เข้าร่วมบริษัท MFEC Public Company Limited ในตำแหน่ง Progremmer
จากทุกอย่างที่กล่าวมาข้างต้นทำให้ฉันมั่นใจค่ะว่าสามารถร่วมงานกับคุณได้</p>

      <template slot="footer">
        <base-button type="primary" class="ml-auto" @click="modals.modal1 = false">Close</base-button>
      </template>
    </modal>
    <section class="section section-skew">
      <div class="container">
        <card shadow class="card-profile mt--300" no-body>
          <div class="px-4">
            <div class="row justify-content-center">
              <div class="col-lg-3 order-lg-2">
                <div class="card-profile-image">
                  <a href="#">
                    <img v-lazy="'img/theme/team-4-800x800.jpg'" class="rounded-circle" />
                  </a>
                </div>
              </div>
              <div class="col-lg-4 order-lg-3 text-lg-right align-self-lg-center">
                <div class="card-profile-actions py-4 mt-lg-0">
                  <base-button
                    tag="a"
                    type="info"
                    size="sm"
                    href="https://drive.google.com/file/d/1tCWiCoFnCZ6pLZiX9owA1LNxciITfZES/view?usp=sharing"
                    role="button"
                    aria-pressed="true"
                  >Download Resume</base-button>
                  <base-button
                    tag="a"
                    type="default"
                    size="sm"
                    class="float-right"
                    href="https://drive.google.com/file/d/18-i-RTTImxCoVrllNF9vcD3vC5pcOaC_/view?usp=sharing"
                    role="button"
                    aria-pressed="true"
                  >Thesis</base-button>
                </div>
              </div>
              <div class="col-lg-4 order-lg-1">
                <div class="card-profile-stats d-flex justify-content-center">
                  
                </div>
              </div>
            </div>
            <div class="text-center mt-5">
              <h3>
                Chanisara Uttamawetin
                <span class="font-weight-light">, 23</span>
              </h3>
              <div class="h6 font-weight-300">
                <i class="ni location_pin mr-2"></i>Bangkok, Thailand
              </div>
              <div class="h6 mt-4">
                <i class="ni business_briefcase-24 mr-2"></i>programmer
              </div>
              <div>
                <p
                  class="font-weight-bold text-success"
                >Skill (Python, JavaScript, Vue.js, NodeJs, PHP, SQL, UiPath, LineAPI)</p>
              </div>
              <div>
              <p class="text-warning mb-0"> contact : 0923144886 , 0881743803</p>
              <p class="text-warning mb-0"> email : chanisaramint@gmail.com </p>
              <p class="text-warning mb-0"> line ID : chanisaramint</p>
              
              </div>
            </div>
            <div class="mt-5 py-5 border-top text-center">
              <div class="row justify-content-center">
                <div class="col-lg-9">
                  <p>สวัสดีค่ะ เราชื่อ มิ้นนะคะ ปัจจุบันทำงานเป็นโปรแกรมเมอร์ค่ะ อยู่ที่กรุงเทพมหานคร....</p>
                  <a href="#"></a>
                  <button class="btn btn-link text-info" @click="modals.modal1 = true">Show more</button>
                </div>
              </div>
            </div>
          </div>
        </card>
      </div>
    </section>
    <section class="section section-components">
      <div class="container">
        <h3 class="h4 text-success font-weight-bold mb-4">Experience</h3>
        <tabs-section></tabs-section>
        <progress-section></progress-section>
        <div class="row row-grid justify-content-between">
          <tabs fill class="flex-column flex-md-row">
            <card shadow>
            <tab-pane title="My Work">
                <p class="description"></p>
                <div class="row py-3 align-items-center">
                <div class="col-sm-3">
                    <small class="text-uppercase text-muted font-weight-bold">Intern</small><br>
                    <small class="text-uppercase text-muted font-weight-bold">November 2018  -  March 2019</small>
                  </div>
                  <div class="col-sm-9">
                    <p class="text-info mb-0">
                      <li class="text-info mb-0">
                        test system website and Application
                      </li>
                      <li class="text-info mb-0">
                        Fill in the EDC device.
                      </li><br>
                
                  </div>
                  <div class="col-sm-3">
                    <small class="text-uppercase text-muted font-weight-bold">Programmer</small><br>
                    <small class="text-uppercase text-muted font-weight-bold">May 2019 - Present</small>
                  </div>
                  <div class="col-sm-9">
                    <p class="text-primary mb-0">
                      <li class="text-primary mb-0">
                        Develop Line API + Queue system 
                      </li>
                      <li class="text-primary mb-0">
                        Develop Line API + dialogflow + Google sheet (google script)
                      </li>
                      <li class="text-primary mb-0">
                        Develop UI Path +  Internal system
                      </li>
                      <li class="text-primary mb-0">
                      Contest cisco innovation challenoe 2019 Develop ( นวัตกรรมบ้าน iot เพื่อผู้สูงอายุ )
                      </li>
                      <li class="text-primary mb-0">
                      Develop Learning Management System (LMS)  of Moodle with cisco webex
                      </li>
                      <li class="text-primary mb-0">
                      admin page facebook + Create infographic
                      </li>
                      <li class="text-primary mb-0">
                      Develop Website + Vue.js
                      </li>
                      <li class="text-primary mb-0">
                      Develop line notify  +  Learning Management System (LMS) moodle 
                      </li>
                      <li class="text-primary mb-0">
                      Create UX UI website + adobe XD
                      </li>
                  </div>
                </div>
              </tab-pane>
            
              <tab-pane title="education">
                <p class="description">
                  <div class="row py-3 align-items-center">
                  <div class="col-sm-3">
                    <small class="text-uppercase text-muted font-weight-bold">Bachelor degree</small><br>
                    <small class="text-uppercase text-muted font-weight-bold">2015 - 2019</small>
                  </div>
                  <div class="col-sm-9">
                    <p class="text-primary mb-0">
                      <li class="text-primary mb-0">
                        Major Computer Science, Faculty of Science, Bachelor of Science, Naresuan University , GPA:2.24
                      </li>
                    </div>
                  </div>
              </tab-pane>

              <tab-pane title="Training">
                <p class="description"></p>
                <div class="row py-3 align-items-center">
                  <div class="col-sm-3">
                    <small class="text-uppercase text-muted font-weight-bold">2019</small>
                  </div>
                  <div class="col-sm-9">
                    <p class="text-primary mb-0">
                      <li class="text-primary mb-0">
                        THE 5th CONFERENCE ON RESEARCH AND
                        CREATIVE INNOVATIONS : CRCI-2018
                      </li>
                      <li class="text-primary mb-0">
                        The 2nd academic service program on health
                        promotion and sports skill development :
                        Banrongluke school
                      </li><br>
                    
                  </div>
                  <div class="col-sm-3">
                    <small class="text-uppercase text-muted font-weight-bold">2018</small>
                  </div>
                  <div class="col-sm-9">
                    <p class="text-info mb-0">
                      <li class="text-warning mb-0">
                        Faculty of Science Students' Club
                      </li>
                      <br>
                  </div>
                  <div class="col-sm-3">
                    <small class="text-uppercase text-muted font-weight-bold">2017</small>
                  </div>
                  <div class="col-sm-9">
                    <p class="text-info mb-0">
                      <li class="text-info mb-0">
                        YoungSoft, Naresuan University Training
                        Programming with PHP language(laravel)
                      </li>
                      <li class="text-info mb-0">
                        YoungSoft, Naresuan University Android firebase
                        application development workshop
                      </li><br>
                
                  </div>
                  <div class="col-sm-3">
                    <small class="text-uppercase text-muted font-weight-bold">2016</small>
                  </div>
                  <div class="col-sm-9">
                    <p class="text-success mb-0">
                      <li class="text-success mb-0">
                        YoungSoft, Naresuan University wordpress
                        template workshop
                      </li>

                  </div>
                </div>
              </tab-pane>
            </card>
          </tabs>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
import Modal from "@/components/Modal.vue";
import Tabs from "@/components/Tabs/Tabs.vue";
import TabPane from "@/components/Tabs/TabPane.vue";
export default {
  components: {
    Modal,
    Tabs,
    TabPane
  },
  data() {
    return {
      modals: {
        modal1: false,
        modal2: false,
        modal3: false
      }
    };
  }
};
</script>
<style>
</style>
