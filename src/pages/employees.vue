<template>
  <main class="space-y-16 py-8">
    <Navbar />
    <section id="heading">
      <div class="flex w-[48rem] flex-col gap-y-4 px-8 md:px-0">
        <h1 class="text-4xl font-semibold">Employees</h1>
        <p class="text-neutral-500 dark:text-neutral-400">
          Our valuable, professionally-trained employees of Fang Industries,
          inc.
        </p>
      </div>
    </section>
    <section id="members">
      <div class="flex w-[48rem] flex-col gap-y-6 px-8 md:px-0">
        <EmployeeCard
          :img="Jayden"
          quote="It's sad when someone you know becomes someone you knew"
          name="Joydon Rich Loui III"
          :timestamp="1671559320"
        />
        <EmployeeCard
          :img="Nadine"
          quote="I’m sorry, I’m uncomfortable with emotions."
          name="Nichodine Staphylococcus Sus"
          :timestamp="1665384948"
        />
        <EmployeeCard
          :img="Albert"
          quote="L"
          name="Angry Birt"
          :timestamp="1664344117"
        />
        <EmployeeCard
          :img="Brigitta"
          quote="mental = gone 👍"
          name="Brigitata Ingitta Laur Widjstrich"
          :timestamp="1664009853"
        />
        <EmployeeCard
          :img="Tristan"
          quote="the best way to cook egg is for it to explode like my nuts"
          name="Tristano Litano Milano The Minato Karim Gupta"
          :timestamp="1660783111"
        />
        <EmployeeCard
          :img="Jovan"
          quote="sometimes i just wanna bomb the school because i keep on seeing ms ririn's face"
          name="Muhammad Jovannes Aditya Gunawan Surya Jonathan William Ahmad Agung Budi Gunadi Hartono Setiawan Putra Immanuel Wijaya"
          :timestamp="1657468496"
        />
        <EmployeeCard
          :img="Antonio"
          quote="i don't know what the fuck i'm doing here"
          name="Antonius Kausarius III, Jr."
          :timestamp="1650507835"
        />
        <EmployeeCard
          :img="Nicholas"
          quote="i love clicking on lolies"
          name="Nikky Nikky Daninisawawaera Susprapto"
          :timestamp="1649574237"
        />
        <EmployeeCard
          :img="Jason"
          quote="im disappointed by the fact that i made this"
          name="Jaosn Fanansg"
          :timestamp="1644972908"
        />
        <EmployeeCard
          :img="Evan"
          quote="i love loling"
          name="Evannes Bohannes Gohannes Cornary Monarchy Karawachi Wangsa Bangsa"
          :timestamp="1644972908"
        />
      </div>
    </section>
    <Footer />
  </main>
</template>

<script setup lang="ts">
import Navbar from "@/components/Navbar.vue";
import Footer from "@/components/Footer.vue";
import EmployeeCard from "@/components/EmployeeCard.vue";

import Evan from "@/assets/media/evan.png";
import Jason from "@/assets/media/jason.png";
import Nicholas from "@/assets/media/nicholas.png";
import Antonio from "@/assets/media/anto.png";
import Jovan from "@/assets/media/jovan.jpg";
import Tristan from "@/assets/media/tristan.png";
import Brigitta from "@/assets/media/bri.png";
import Albert from "@/assets/media/albert.png";
import Nadine from "@/assets/media/nadine.png";
import Jayden from "@/assets/media/jayden.png";
</script>
