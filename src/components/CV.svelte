<script>
  import {_} from "svelte-i18n";
</script>

<main class="hyphens-manual">

  <!-- Page -->
  <div
    class="p-6 mx-auto page max-w-a4 md:max-w-a4 h-a4 xsm:p-8 sm:p-9 md:p-16"
  >

    <!-- Header -->
    <header class="clearfix mb-8 md:mb-11 print:pt-16">
      <div class="float-left flex items-center">
        <div
          class="initials-container mr-5 text-base leading-none text-white
          bg-gray-700 font-medium px-3"
          style="padding-bottom: 0.6875rem; padding-top: 0.6875rem; /*11px*/"
        >
          <div
            class="initial text-center"
            style="padding-bottom: 0.1875rem; /*3px*/"
          >
            A
          </div>
          <div
            class="initial text-center"
            style="padding-bottom: 0.1875rem; /*3px*/"
          >
            E
          </div>
          <div class="text-center initial">D</div>
        </div>
        <div class="pb-px">
          <h1 class="text-3xl font-semibold text-gray-750">
            Ahmet Enes Duruer
          </h1>
          <h2 class="text-gray-700">{$_('profession')}</h2>
        </div>
      </div>
      <div class="float-right text-right text-gray-700">
        <ul class="text-right">
          <li class="flex items-center align-right">
            <span class="mr-4 flex-1">Sakarya, {$_('country')}, 54600</span>
            <svg
              class="h-4 w-4 pb-px stroke-current"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="none"
              stroke="#000000"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            >
              <circle cx="12" cy="10" r="3"></circle>
              <path
                d="M12 21.7C17.3 17 20 13 20 10a8 8 0 1 0-16 0c0 3 2.7 6.9 8
                11.7z"
              ></path>
            </svg>
          </li>
          <li class="flex items-center align-right">
            <span class="mr-4 flex-1"><a href="https://duruer.dev" target="_blank">https://duruer.dev</a></span>
            <svg
              class="h-4 w-4 pb-px stroke-current"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="none"
              stroke="#000000"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            >
              <rect x="2" y="3" width="20" height="14" rx="2" ry="2"></rect>
              <line x1="8" y1="21" x2="16" y2="21"></line>
              <line x1="12" y1="17" x2="12" y2="21"></line>
            </svg>
          </li>
          <li class="flex items-center">
            <span class="mr-4 flex-1"><a href="mailto:ahmet@duruer.dev">ahmet@duruer.dev</a></span>
            <svg
              class="h-4 w-4 pb-px stroke-current"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="none"
              stroke="#000000"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
            >
              <path
                d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1
                0-2-.9-2-2V6c0-1.1.9-2 2-2z"
              ></path>
              <polyline points="22,6 12,13 2,6"></polyline>
            </svg>
          </li>
          <li class="flex items-center">
            <span class="mr-4 flex-1"><a href="https://linkedin.com/in/ahmet-enes-duruer" target="_blank">linkedin.com/in/ahmet-enes-duruer</a></span>
            <svg
              class="h-4 w-4 pb-px fill-current"
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="#000"
            >
              <path
                d="M22.23 0H1.77C.8 0 0 .77 0 1.72v20.56C0 23.23.8 24 1.77
                24h20.46c.98 0 1.77-.77 1.77-1.72V1.72C24 .77 23.2 0 22.23
                0zM7.27 20.1H3.65V9.24h3.62V20.1zM5.47 7.76h-.03c-1.22
                0-2-.83-2-1.87 0-1.06.8-1.87 2.05-1.87 1.24 0 2 .8 2.02 1.87 0
                1.04-.78 1.87-2.05 1.87zM20.34
                20.1h-3.63v-5.8c0-1.45-.52-2.45-1.83-2.45-1 0-1.6.67-1.87
                1.32-.1.23-.11.55-.11.88v6.05H9.28s.05-9.82
                0-10.84h3.63v1.54a3.6 3.6 0 0 1 3.26-1.8c2.39 0 4.18 1.56 4.18
                4.89v6.21z"
              ></path>
            </svg>
          </li>
        </ul>
      </div>
    </header>

    <hr class="mb-8"/>
    <!-- end Name -->

    <!-- Column -->
    <div
      class="md:col-count-2 print:col-count-2 col-gap-md md:h-a4-col
      print:h-a4-col col-fill-auto"
    >

      <section class="mt-8 first:mt-0">
        <!-- To keep in the same column -->
        <div class="break-inside-avoid">

          <h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-800">
            {$_('title.about-me')}
          </h2>

          <section class="mb-4.5 break-inside-avoid">
            <p class="mt-2.1 text-md text-gray-700 leading-normal text-justify">
              {@html $_('about-me')}
            </p>
          </section>

        </div>
      </section>


      <hr class="mt-8"/>

      <section class="mt-8 first:mt-0">

        <!-- To keep in the same column -->
        <div class="break-inside-avoid">

          <h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-800">
            {$_('title.experience')}
          </h2>

          <section class="mb-4.5 break-inside-avoid">
            <header>
              <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
                {$_('work-experience.iconecwave.title')}
              </h3>
              <p class="leading-normal text-md text-gray-650">
                {$_('work-experience.iconecwave.date')} | {$_('work-experience.iconecwave.profession')}
              </p>
              <div class="text-gray-600 leading-loose">
                {$_('work-experience.iconecwave.technologies')}
              </div>
            </header>
          </section>

          <section class="mb-4.5 break-inside-avoid">
            <header>
              <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
                {$_('work-experience.kodgemisi.title')}
              </h3>
              <p class="leading-normal text-md text-gray-650">
                {$_('work-experience.kodgemisi.date')} | {$_('work-experience.kodgemisi.profession')}
              </p>
              <div class="text-gray-600 leading-loose">
                {$_('work-experience.kodgemisi.technologies')}
              </div>
            </header>
          </section>

          <section class="mb-4.5 break-inside-avoid">
            <header>
              <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
                {$_('work-experience.statu.title')}
              </h3>
              <p class="leading-normal text-md text-gray-650">
                {$_('work-experience.statu.date')} | {$_('work-experience.statu.profession')}
              </p>
              <div class="text-gray-600 leading-loose">
                {$_('work-experience.statu.technologies')}
              </div>
            </header>
          </section>

          <section class="mb-4.5 break-inside-avoid">
            <header>
              <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
                {$_('work-experience.general-mobile.title')}
              </h3>
              <p class="leading-normal text-md text-gray-650">
                {$_('work-experience.general-mobile.date')} | {$_('work-experience.general-mobile.profession')}
              </p>
              <div class="text-gray-600 leading-loose">
                {$_('work-experience.general-mobile.technologies')}
              </div>
            </header>
          </section>

        </div>
      </section>

      <br>

      <section class="mt-8 first:mt-0">

        <!-- To keep in the same column -->
        <div class="break-inside-avoid">
          <h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-800">
            {$_('title.references')}
          </h2>
        </div>

        <section class="mb-4.5 break-inside-avoid">
          <header>
            <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
              {$_("references.iconecwave.title")}
            </h3>
            <p class="leading-normal text-md text-gray-650">
              {$_("references.iconecwave.things")}
            </p>
          </header>
          <p class="mt-2.1 text-md text-gray-700 leading-normal text-justify">
            {@html $_("references.iconecwave.description")}
          </p>
        </section>

        <section class="mb-4.5 break-inside-avoid">
          <header>
            <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
              {$_("references.iconecwave-dxpathfinder.title")}
            </h3>
            <p class="leading-normal text-md text-gray-650">
              {$_("references.iconecwave-dxpathfinder.things")}
            </p>
          </header>
          <p class="mt-2.1 text-md text-gray-700 leading-normal text-justify">
            {@html $_("references.iconecwave-dxpathfinder.description")}
          </p>
        </section>

        <section class="mb-4.5 break-inside-avoid">
          <header>
            <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
              {@html $_("references.kodgemisi.title")}
            </h3>
            <p class="leading-normal text-md text-gray-650">
              {$_("references.kodgemisi.things")}
            </p>
          </header>
          <p class="mt-2.1 text-md text-gray-700 leading-normal text-justify">
            {@html $_("references.kodgemisi.description")}
          </p>
        </section>

        <section class="mb-4.5 break-inside-avoid">
          <header>
            <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
              {$_("references.general-mobile.title")}
            </h3>
            <p class="leading-normal text-md text-gray-650">
              {$_("references.general-mobile.things")}
            </p>
          </header>
          <p class="mt-2.1 text-md text-gray-700 leading-normal text-justify">
            {@html $_("references.general-mobile.description")}
          </p>
        </section>

        <section class="mb-4.5 break-inside-avoid">
          <header>
            <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
              {@html $_("references.portfolio.title")}
            </h3>
            <p class="leading-normal text-md text-gray-650">
              {$_("references.portfolio.date")} | {$_("references.portfolio.things")}
            </p>
          </header>
          <p class="mt-2.1 text-md text-gray-700 leading-normal text-justify">
            {$_("references.portfolio.description")}
          </p>
        </section>

        <section class="mb-4.5 break-inside-avoid">
          <header>
            <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
              {$_("references.routve.title")}
            </h3>
            <p class="leading-normal text-md text-gray-650">
              {$_("references.routve.date")} | {$_("references.routve.things")}
            </p>
          </header>
          <p class="mt-2.1 text-md text-gray-700 leading-normal text-justify">
            {$_("references.routve.description")}
          </p>
        </section>

        <section class="mb-4.5 break-inside-avoid">
          <header>
            <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
              {$_("references.pano.title")}
            </h3>
            <p class="leading-normal text-md text-gray-650">
              {$_("references.pano.date")} | {$_("references.pano.things")}
            </p>
          </header>
          <p class="mt-2.1 text-md text-gray-700 leading-normal text-justify">
            {$_("references.pano.description")}
          </p>
        </section>

        <hr class="mt-8"/>

        <section class="mt-8 first:mt-0">

          <!-- To keep in the same column -->
          <div class="break-inside-avoid">

            <h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-800">
              {$_('title.education')}
            </h2>

            <section class="mb-4.5 break-inside-avoid">
              <header>
                <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
                  {$_('education.pecs-uni.title')}
                </h3>
                <p class="leading-normal text-md text-gray-600">
                  {$_('education.pecs-uni.major')}
                </p>
              </header>
            </section>

          </div>
        </section>
      </section>
    </div>
  </div>

  <br>
  <br>
  <br>

  <!-- Page -->
  <div
    class="p-6 mx-auto page max-w-a4 md:max-w-a4 h-a4 xsm:p-8 sm:p-9 md:p-16"
  >

    <!-- Column -->
    <div
      class="md:col-count-2 print:col-count-2 col-gap-md md:h-a4-col
      print:h-a4-col col-fill-auto mt-16"
    >
      <!--    &lt;!&ndash; Column &ndash;&gt;-->
      <!--    <div-->
      <!--      class="md:col-count-2 print:col-count-2 col-gap-md md:h-a4-col-->
      <!--      print:h-a4-col col-fill-auto"-->
      <!--    >-->

      <section class="mt-8 first:mt-0">

        <!-- To keep in the same column -->
        <div class="break-inside-avoid">

          <h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-800">
            {$_('title.languages')}
          </h2>

          <section class="mb-4.5">
            <header>
              <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
                English
              </h3>
              <p class="leading-normal text-md text-gray-650">
                {$_('language.professional')}
              </p>
            </header>
          </section>
        </div>
      </section>

      <section class="mt-8 first:mt-0">

        <!-- To keep in the same column -->
        <div class="break-inside-avoid">

          <section class="mb-4.5 break-inside-avoid">
            <header>
              <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
                Turkish
              </h3>
              <p class="leading-normal text-md text-gray-650">
                {$_('language.native')}
              </p>
            </header>
          </section>

          <hr class="mt-8"/>

          <section class="mt-8 first:mt-0">

            <!-- To keep in the same column -->
            <div class="break-inside-avoid">

              <h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-800">
                {$_('title.certificates')}
              </h2>

              <section class="mb-4.5 break-inside-avoid">
                <header>
                  <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
                    {$_("certificates.efset.title")}
                  </h3>
                  <p class="leading-normal text-md text-gray-600">
                    {$_("certificates.efset.description")}
                  </p>
                </header>
              </section>

            </div>

          </section>

          <hr class="mt-8"/>

          <section class="mt-8 first:mt-0">

            <!-- To keep in the same column -->
            <div class="break-inside-avoid">

              <h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-800">
                {$_('title.skills')}
              </h2>

              <section class="mb-4.5">
                <header>
                  <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
                    Kotlin
                  </h3>
                  <p class="leading-normal text-md text-gray-650">
                    {$_('skills.high-level')}
                  </p>
                </header>
                <div class="my-3.2 last:pb-1.5">
                  <ul
                    class="flex flex-wrap text-md leading-relaxed -mr-1.6 -mb-1.6"
                  >
                    <li
                      class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                    >
                      Vert.x
                    </li>
                    <li
                      class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                    >
                      Back-end
                    </li>
                    <li
                      class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                    >
                      OOP
                    </li>
                    <li
                      class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                    >
                      Android
                    </li>
                    <li
                      class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                    >
                      Web
                    </li>
                    <li
                      class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                    >
                      Server
                    </li>
                  </ul>
                </div>
              </section>
            </div>
          </section>

          <section class="mb-4.5 break-inside-avoid">
            <header>
              <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
                Java
              </h3>
              <p class="leading-normal text-md text-gray-650">
                {$_('skills.high-level')}
              </p>
            </header>
            <div class="my-3.2 last:pb-1.5">
              <ul
                class="flex flex-wrap text-md leading-relaxed -mr-1.6 -mb-1.6"
              >
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  Spring
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  Micronaut
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  Hibernate
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  Lombok
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  MapStruct
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  AWS SDK
                </li>
              </ul>
            </div>
          </section>

          <section class="mb-4.5 break-inside-avoid">
            <header>
              <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
                Javascript
              </h3>
              <p class="leading-normal text-md text-gray-650">
                {$_('skills.high-level')}
              </p>
            </header>
            <div class="my-3.2 last:pb-1.5">
              <ul
                class="flex flex-wrap text-md leading-relaxed -mr-1.6 -mb-1.6"
              >
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  Vue.js
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  Svelte 3
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  ReactJS
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  SvelteKit
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  REST API
                </li>
              </ul>
            </div>
          </section>

          <section class="mb-4.5 break-inside-avoid">
            <header>
              <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
                Database
              </h3>
              <p class="leading-normal text-md text-gray-650">
                {$_('skills.middle-level')}
              </p>
            </header>
            <div class="my-3.2 last:pb-1.5">
              <ul
                class="flex flex-wrap text-md leading-relaxed -mr-1.6 -mb-1.6"
              >
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  MySQL
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  SQLite
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  MariaDB
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  MongoDB
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  MSSQL
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  DynamoDB
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  PostgreSQL
                </li>
              </ul>
            </div>
          </section>

          <section class="mb-4.5 break-inside-avoid">
            <header>
              <h3 class="text-lg font-semibold text-gray-650 leading-snugish">
                Linux
              </h3>
              <p class="leading-normal text-md text-gray-650">
                {$_('skills.high-level')}
              </p>
            </header>
            <div class="my-3.2 last:pb-1.5">
              <ul
                class="flex flex-wrap text-md leading-relaxed -mr-1.6 -mb-1.6"
              >
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  Arch Linux
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  Linux Mint
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  Debian
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  Server
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  DevOps
                </li>
                <li
                  class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750
                  bg-gray-200"
                >
                  Docker
                </li>
              </ul>
            </div>
          </section>

        </div>

      </section>

      <section class="mt-8 first:mt-0">

        <!-- To keep in the same column -->
        <div class="break-inside-avoid">

          <h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-800">
            {$_('title.hobbies')}
          </h2>

        </div>

        <section class="mb-4.5 break-inside-avoid">
          <div class="my-3.2 last:pb-1.5">
            <ul class="flex flex-wrap text-md leading-relaxed -mr-1.6 -mb-1.6">
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                {$_("hobbies.table-tennis")}
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                {$_("hobbies.swimming")}
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                {$_("hobbies.cycling")}
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                {$_("hobbies.billiard")}
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                {$_("hobbies.researching")}
              </li>
            </ul>
          </div>
        </section>

      </section>

      <section class="mt-8 first:mt-0">

        <!-- To keep in the same column -->
        <div class="break-inside-avoid">

          <h2 class="mb-4 font-bold tracking-widest text-sm2 text-gray-800">
            {$_('title.other')}
          </h2>

        </div>

        <section class="mb-4.5 break-inside-avoid">
          <div class="my-3.2 last:pb-1.5">
            <ul class="flex flex-wrap text-md leading-relaxed -mr-1.6 -mb-1.6">
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                GitHub
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                IDE
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                Git
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                Python
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                BitBucket
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                GitLab
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                Trello
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                Slack
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                CI / CD
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                GitHub Actions
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                Travis CI
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                Back-End
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                JavaScript Developer
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                Maven
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                Gradle
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                JIRA
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                Jenkins
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                Agile Sprint / Kanban
              </li>
              <li
                class="px-2.5 mr-1.6 mb-1.6 text-base text-gray-750 bg-gray-200"
              >
                Googling :)
              </li>
            </ul>
          </div>
        </section>

      </section>
    </div>

    <!--    </div>-->
    <!-- end Column -->

  </div>
  <!-- end Page -->

</main>
