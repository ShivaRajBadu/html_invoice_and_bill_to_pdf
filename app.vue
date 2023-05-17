<template>
  <div class="main-container">
    <Invoice />
    <button class="converter_btn" @click="generatePDF($event)">
      Convert To PDF
    </button>
  </div>
</template>

<script setup>
import { jsPDF } from "jspdf";
import html2canvas from "html2canvas";

const generatePDF = async (e) => {
  const canvas = await html2canvas(e.target.previousSibling);
  const imgData = canvas.toDataURL("image/png");
  const pdf = new jsPDF();
  const pdfWidth = pdf.internal.pageSize.getWidth();
  const pdfHeight = (canvas.height * pdfWidth) / canvas.width;

  pdf.addImage(imgData, "PNG", 0, 0, pdfWidth, pdfHeight);
  pdf.save("output.pdf");
};
</script>

<style scoped>
.main-container {
  max-width: 1440px;
  margin: 0 auto;
  background-color: #e4e4e4;
  padding: 5rem 0;
}
.converter_btn {
  margin-top: 3rem;
  font-size: 18px;
  padding: 0.5rem 0;
  border: none;
  background-color: #ffcccc;
  box-shadow: 1px 1px 10px rgb(153, 147, 147);
  font-weight: 600;
  text-align: center;
  width: 66%;
  margin-left: 13rem;
}
</style>
