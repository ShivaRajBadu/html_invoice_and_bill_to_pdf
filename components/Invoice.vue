<template>
  <div ref="content" class="wrapper">
    <h1 class="supplier_name">COMPANY NAME LIMITED</h1>

    <div class="invoice_info">
      <div class="invoice_left_info">
        <div>
          <p>PAN NO:</p>
          <p>232312442</p>
        </div>
        <p>Dharan-15, Sunsari</p>
      </div>
      <div class="invoice_right_info">
        <div>
          <p>Invoice No:</p>
          <p>32342</p>
        </div>
        <div>
          <p>Transaction Date:</p>
          <p>2080/01/05</p>
        </div>
        <div>
          <p>Invoice Issue Date:</p>
          <p>2080/01/05</p>
        </div>
      </div>
    </div>
    <div class="email_section">
      <p class="email">E-MAIL <span>companyName5@hotmail.com</span></p>
      <div>
        <p>2078/02/22</p>
        <p>12:02:33 PM</p>
      </div>
    </div>
    <h2 class="invoice-title">INVOICE</h2>
    <div class="table_section">
      <p class="dashed-line"></p>

      <table class="table">
        <thead class="thead">
          <tr>
            <th>S.N</th>
            <th>CODE:</th>
            <th>ITEM DESCRIPTION:</th>
            <th>PACK:</th>
            <th>BATCH:</th>
            <th>EXP.DATE</th>
            <th>QTY:</th>
            <th>CC/RATE:</th>
            <th>AMOUNT:</th>
            <th>M.R.P</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>1.</td>
            <td>NN10093</td>
            <td>HEDUDUD 50ML WERIE</td>
            <td>1PH</td>
            <td>GE0361</td>
            <td>Oct 2022</td>
            <td>5</td>
            <td>126.43</td>
            <td>633.00</td>
            <td>93.00</td>
          </tr>
          <tr>
            <td>2.</td>
            <td>RY10093</td>
            <td>HEDUDUD 50ML WERIE</td>
            <td>1PH</td>
            <td>GE0361</td>
            <td>Oct 2022</td>
            <td>5</td>
            <td>126.43</td>
            <td>633.00</td>
            <td>93.00</td>
          </tr>
          <tr>
            <td colspan="3" style="text-align: center">- do -</td>
            <td>1PH</td>
            <td>GE0361</td>
            <td>Oct 2022</td>
            <td>7 FREE</td>
            <td>126.43</td>
            <td>633.00</td>
            <td>93.00</td>
          </tr>
          <tr>
            <td>3.</td>
            <td>WY10029</td>
            <td>param 50ml petya</td>
            <td>1PH</td>
            <td>GE0361</td>
            <td>Oct 2022</td>
            <td>5</td>
            <td>126.43</td>
            <td>633.00</td>
            <td>93.00</td>
          </tr>
        </tbody>
      </table>
      <!-- total table  -->
      <table class="total_table">
        <tbody class="total_t_body">
          <tr>
            <td>CUSTOMER COPY</td>
            <td>TOTAL</td>
            <td>:</td>
            <td>3,954.10</td>
          </tr>
          <tr>
            <td></td>
            <td>LESS DISCOUNT</td>
            <td>:</td>

            <td>3,954.10</td>
          </tr>
          <tr>
            <td></td>
            <td>ROUNDING</td>
            <td>:</td>
            <td>3,954.10</td>
          </tr>
        </tbody>
      </table>
      <!-- net total -->
      <table class="net_total">
        <tbody class="net_total_tbody">
          <tr>
            <td></td>
            <td>NET TOTAL</td>
            <td>:</td>
            <td>3,954.10</td>
          </tr>
        </tbody>
      </table>
      <p class="inwords">
        Inwords Rs: <span>Three Thousands Five Hundreds Ninty Nine Only</span>
      </p>
      <div class="note">
        <p>Note:</p>
        <p>Due Date: 2078/03/23</p>
      </div>
    </div>
    <div class="signatures">
      <div>
        <p>(Checked By)</p>
        <p>(Received By)</p>
      </div>
      <div class="for">
        <p>For: <span>SARTHAK MEDI DISTRIBUTOR</span></p>
        <p>RAMESH</p>
      </div>
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

.invoice_info {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  margin-top: 1rem;
}
.invoice_left_info > div,
.invoice_right_info > div {
  display: flex;
  gap: 1.2rem;
  padding-block: 0.09rem;
}

.invoice_left_info > div > p:first-child,
.invoice_right_info > div > p:first-child {
  font-weight: 500;
  font-size: 14px;
  margin-right: 0;
  margin-left: auto;
}
.invoice_left_info > div > p:last-child,
.invoice_right_info > div > p:last-child {
  font-size: 14px;
  font-weight: 600;
  text-align: end;
  margin-right: 0;
  margin-left: auto;
}

.email_section {
  display: flex;
  justify-content: space-between;
  font-size: 14px;
  font-weight: 600;
}
.email > span {
  font-weight: 500;
  margin-left: 1rem;
}
.email_section > div {
  text-align: end;
}
.email_section > div > p:last-child {
  font-weight: 500;
}
.invoice-title {
  text-align: center;
  margin-block: 0.4rem;
  font-size: 18px;
}
.table_section {
  margin-top: 2rem;
}
.dashed-line {
  border-bottom: 1px dashed rgb(75, 73, 73);
  margin-bottom: 0.25rem;
}

.table {
  width: 100%;
  border-collapse: collapse;
  border-spacing: 8px;
  position: relative;
  margin-bottom: 1rem;
}
.table::after {
  position: absolute;
  content: " ";
  bottom: -8px;

  width: 100%;
  border-bottom: 1px dashed black;
}

th {
  text-align: start;
  font-size: 14px;
  width: max-content;
  max-width: 15%;
  padding-top: 0.5rem;
  padding-bottom: 0.4rem;

  border-block: 1px dashed rgb(75, 73, 73);
  box-sizing: border-box;
  position: relative;
}

th:nth-child(3) {
  max-width: 25%;
  width: 100%;
}
td {
  text-align: start;
  font-size: 12px;
  padding-top: 0.1rem;
  padding-left: 0.2rem;
  padding-right: 0.4rem;
  box-sizing: border-box;
  position: relative;
}

th:last-child::after,
td:last-child::after {
  border-right: none;
}
.total_table {
  width: 100%;
}
/* .total_table > tbody > tr > td {
  border: 1px solid green;
} */
.total_table > tbody > tr > td:nth-child(2) {
  width: 20%;
}
.total_table > tbody > tr > td:first-child {
  width: 57%;
}
.total_t_body {
  position: relative;
}
.total_t_body::after {
  content: "";
  position: absolute;
  bottom: -6px;
  right: 100px;
  width: 75px;
  border-bottom: 1px dashed rgb(75, 73, 73);
}
.net_total {
  width: 100%;
  margin-top: 0.6rem;
  margin-bottom: 2rem;
}

.net_total > tbody > tr > td:nth-child(2) {
  width: 20%;
}
.net_total > tbody > tr > td:first-child {
  width: 56.5%;
}
.net_total_tbody {
  position: relative;
}
.net_total_tbody::after {
  content: "";
  position: absolute;
  width: 75px;
  bottom: -10px;
  right: 100px;
  height: 6px;
  border-bottom: 1px dashed rgb(75, 73, 73);
  border-top: 1px dashed rgb(75, 73, 73);
}
.inwords {
  font-size: 15px;
  font-weight: 500;
  border-bottom: 1px dashed rgb(75, 73, 73);
  padding-block: 0.5rem;
}
.inwords > span {
  font-weight: 500;
  font-size: 14px;
}
.note {
  margin-block: 0.6rem;
}
.note > p:first-child {
  font-weight: 600;
  font-size: 14px;
}
.note > p:last-child {
  font-size: 14px;
  font-weight: 600;
  padding-left: 0.4rem;
}
.signatures {
  margin-top: 10rem;
  display: flex;
  justify-content: space-between;
}
.signatures p {
  font-size: 14px;
}
.signatures > div:first-child {
  display: flex;
  gap: 5rem;
}
.for {
  font-size: 14px;
  text-align: end;
}
.for > p:last-child {
  padding-block: 0.2rem;
}
</style>
