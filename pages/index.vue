<template>
  <menubar>
    <li><nuxt-link to="/">หน้าหลัก</nuxt-link></li>
    <li><nuxt-link to="/">เกี่ยวกับเรา</nuxt-link></li>
    <li><nuxt-link to="/">บัตรเติมเงิน</nuxt-link></li>
    <li><nuxt-link to="/">เติมเกมออนไลน์</nuxt-link></li>
    <li><nuxt-link to="/">เติมเงินมือถือ</nuxt-link></li>
    <li><nuxt-link to="/">สุ่มของรางวัล</nuxt-link></li>
    <li><nuxt-link to="/">เติมบัตรเครดิต</nuxt-link></li>
    <li><nuxt-link to="/">คำถามที่พบบ่อย</nuxt-link></li>
  </menubar>
</template>

<script>
import menubar from '@/components/menubar';
import Dropdown from '@/components/dropdown';
export default {
  data() {
    return {
      options: [
        { text: "Option 1" },
        { text: "Option 2" },
        { text: "Option 3" }
      ]
    }
  },
  methods: {
    handleSelection(item) {
      console.log(item.text + " selected")
    }
  }
}
</script>

