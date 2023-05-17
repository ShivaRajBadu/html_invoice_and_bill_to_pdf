<template>
  <div ref="content" class="wrapper">
    <h1 class="supplier_name">COMPANY NAME LIMITED</h1>
    <p class="supplier_address">Kathmandu, Nepal</p>
    <div class="bill_info">
      <div class="bill_left_info">
        <p>Bill To: <span>Turaj Furaj</span></p>
        <p>Address: <span>Dharan-15</span></p>
        <p>PAN: <span>232312442</span></p>
      </div>
      <div class="bill_right_info">
        <p>Bill Date: <span>2080/01/05</span></p>
        <p>Bill No: <span>32342</span></p>
        <p style="max-width: 200px; width: 100%; text-align: center">
          Remarks:
          <span class="remarks">Lorem ipsum dolor sit amej </span>
        </p>
      </div>
    </div>
    <div class="table_section">
      <table class="table">
        <thead class="thead">
          <tr>
            <th>S.N</th>
            <th>Product Name</th>
            <th>Batch</th>
            <th>Exp.Date</th>
            <th>Rate</th>
            <th>PTR</th>
            <th>MRP</th>
            <th>Qty</th>
            <th>Amt</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>1.</td>
            <td>badu company private limited</td>
            <td>12</td>
            <td>2024/08/23</td>
            <td>100.5</td>
            <td>110.55</td>
            <td>137</td>
            <td>1000</td>
            <td>100,50000.00</td>
          </tr>
          <tr>
            <td>2.</td>
            <td>shiva company private limited</td>
            <td>12</td>
            <td>2024/08/23</td>
            <td>100.5</td>
            <td>110.55</td>
            <td>137</td>
            <td>1000</td>
            <td>100,50000.00</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script setup>
const content = ref(null);
</script>

<style scoped>
*,
::before,
::after {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.wrapper {
  background-color: white;
  max-width: 820px;
  width: 100%;
  margin: 0 auto;
  padding: 3.5rem 1rem;
}

.supplier_name {
  text-transform: uppercase;
  text-align: center;
  font-size: 18px;
  font-weight: bold;
}

.supplier_address {
  text-align: center;
  font-size: 14px;
  padding: 0.3rem 0;
}

.bill_info {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-block: 1rem;
}

.bill_left_info > p,
.bill_right_info > p {
  padding: 0.2rem 0;
  font-size: 12px;
  font-weight: bold;
}

.bill_left_info span,
.bill_right_info span {
  font-weight: 400 !important;
}

.remarks {
  width: 100px;
}

.table_section {
  margin-top: 2rem;
}

.table {
  width: 100%;
  border-collapse: collapse;
  border-spacing: 8px;
  border: 1px solid rgb(75, 73, 73);
}

th {
  text-align: start;
  font-size: 14px;
  width: min-content;
  border-bottom: 1px solid black;
  box-sizing: border-box;
  position: relative;
  padding: 0.1rem 0.2rem;
}

td {
  text-align: start;
  font-size: 12px;
  padding-block: 0.2rem;
  padding-left: 0.3rem;
  padding-right: 0.4rem;
  box-sizing: border-box;
  position: relative;
}

th:nth-child(2) {
  width: 30%;
}

th::after,
td::after {
  content: "";
  position: absolute;
  top: 0;
  right: 7px;

  height: 100%;
  border-right: 1px solid black;
}

th:last-child::after,
td:last-child::after {
  border-right: none;
}
</style>
