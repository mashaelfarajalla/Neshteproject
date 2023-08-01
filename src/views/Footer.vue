<template>
  <footer class="">
    <div class="container">
      <div class="row text-start py-5">
        <div class="col-lg-3 text-start">
          <h5>عن الموقع</h5>
          <p class="mt-4">
            موقع نشتي، وجهتك المثالية لشراء وبيع الأغراض المستعملة ، تقدم تجربة
            سلسة وممتعة.
            <br />
            تلبي منصتنا مجموعة متنوعة من الفئات ، مما يضمن أنه يمكنك العثور على
            ما تبحث عنه بالضبط أو بيع أغراضك بسهولة.
          </p>
        </div>
        <div class="col-md-4 col-lg-3">
          <h5>الحساب والعضوية</h5>
          <ul class="list-unstyled mt-4 mb-0">
            <li class="mb-1">
              <a href="#!">تسجيل </a>
            </li>
            <li class="mb-1">
              <a href="#!">الإعلانات المميزة </a>
            </li>
            <li class="mb-1">
              <a href="#!">توثيق العضوية وإضافة التراخيص</a>
            </li>
            <li>
              <a href="#!">حساب و سداد عمولة الموقع</a>
            </li>
          </ul>
        </div>

        <div class="col-md-4 col-lg-3">
          <h5>روابط</h5>
          <ul class="list-unstyled mt-4 mb-0">
            <li class="mb-1">
              <a href="#!">اتصل بنا </a>
            </li>
            <li class="mb-1">
              <a href="#!">مركز الأمان </a>
            </li>
            <li class="mb-1">
              <a href="#!">اتفاقية الاستخدام</a>
            </li>
            <li class="mb-1">
              <a href="#!">الأسئلة الشائعة</a>
            </li>
            <li class="mb-1">
              <a href="#!">قائمة السلع والإعلانات الممنوعة </a>
            </li>
          </ul>
        </div>
        <div class="col-md-4 col-lg-3">
          <h5>حمل التطبيق</h5>

          <img src="../../public/images/googleplay.jpg" class="" />
          <img src="../../public/images/Appstor.jpg" class="" />
        </div>
      </div>
      <hr />
      <div class="row mt-5 justify-content-end">
        <div class="col-auto">
          <h6>تابعنا:</h6>
        </div>
        <div class="col-auto">
          <div class="row">
            <div
              class="col-auto"
              v-for="(x, index) in socialmedia"
              :key="index"
            >
              <span
                ><svg
                  width="20"
                  height="20"
                  viewBox="0 0 20 20"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <g clip-path="url(#clip0_95_1540)">
                    <path
                      d="M17.4998 0H2.49989C1.8371 0.000720903 1.20166 0.264333 0.732996 0.732996C0.264333 1.20166 0.000720903 1.8371 0 2.49989L0 17.4998C0.000720903 18.1626 0.264333 18.798 0.732996 19.2667C1.20166 19.7354 1.8371 19.999 2.49989 19.9997H17.4998C18.1626 19.999 18.798 19.7354 19.2667 19.2667C19.7354 18.798 19.999 18.1626 19.9997 17.4998V2.49989C19.999 1.8371 19.7354 1.20166 19.2667 0.732996C18.798 0.264333 18.1626 0.000720903 17.4998 0Z"
                      fill="#2B2B2B"
                    />
                    <path
                      d="M16.875 9.99987H13.7499V7.49998C13.7499 6.81002 14.31 6.87509 15 6.87509H16.2501V3.75H13.7502C13.2577 3.74996 12.7701 3.84693 12.3151 4.03537C11.8601 4.22381 11.4467 4.50003 11.0984 4.84826C10.7502 5.19648 10.474 5.60989 10.2856 6.06488C10.0971 6.51987 10.0001 7.00751 10.0002 7.49998V9.99987H7.5V13.125H9.99989V20.0003H13.7499V13.125H15.6261L16.875 9.99987Z"
                      fill="white"
                    />
                  </g>
                  <defs>
                    <clipPath id="clip0_95_1540">
                      <rect width="20" height="20" fill="white" />
                    </clipPath>
                  </defs>
                </svg>
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="footerbottom mt-4">
      <div class="container">
        <div class="row">
          <p>مؤسسة موقع للتسويق الإلكتروني2023</p>
        </div>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  data() {
    return {
      socialmedia: 5,
    };
  },
};
</script>
