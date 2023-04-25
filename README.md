<style>
  * {
    box-sizing: border-box;
  }

  .log__container {
    margin-right: auto;
    margin-left: auto;
    padding-left: 15px;
    padding-right: 15px;
    max-width: 1180px;
  }

  @media (max-width: 375px) {
    .log__container {
      padding-left: 0px;
      padding-right: 0px;
    }
  }

  .log__block {
    padding-top: 32px;
  }

  .log__header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 10px;
  }

  @media (max-width: 768px) {
    .log__header {
      flex-direction: column;
      margin-bottom: 20px;
    }
  }

  .log__title {
    letter-spacing: -0.75px;
    line-height: 110%;
    font-style: normal;
    font-weight: 700;
    font-size: 24px;
    margin-top: 24px;
    margin-bottom: 24px;
    color: #282827;
  }

  .log__sartime {
    display: flex;
    align-items: center;
    font-size: 20px;
    text-align: center;
    color: #282827;
  }

  .log__sartime label {
    font-weight: 600;
    text-transform: uppercase;
    border: 2px solid #000;
    width: 200px;
    height: 35px;
    padding: 5px 0;
    border-right: none;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  @media (max-width: 480px) {
    .log__sartime label {
      width: 150px;
    }
  }

  .log__sartime input {
    border: 2px solid #000;
    width: 200px;
    height: 35px;
    padding: 5px 0;
    text-align: center;
    outline: none;
    font-size: 20px;
    border-radius: 0;
  }

  @media (max-width: 480px) {
    .log__sartime input {
      width: 150px;
    }
  }

  .log__table table {
    border-collapse: collapse;
    font-size: 18px;
    margin-bottom: 16px;
  }

  .log__table tr {}

  .log__table table tr:nth-child(even) {
    background-color: #e6e6e6; 
  }

  @media (max-width: 768px) {
    .log__table table {
      width: 100%;
    }
  }

  .log__table td,
  .log__table th {
    text-align: center;
    padding: 5px;

  }

  @media (max-width: 991px) {

    .log__table td,
    .log__table th {
      padding: 5px 0;
    }
  }

  .log__table th {
    background-color: #3a4c7e;
    color: #fff;
    border: 1px solid #fff;
  }

  @media (max-width: 768px) {
    .log__table th {
      width: 25%;
    }
  }

  .log__table td {
    border: 1px solid #95999f;
    width: 9%;
  }

  .log__table input {
    width: 100%;
    box-sizing: border-box;
    border: none;
    padding: 5px;
    background-color: transparent;
  }

  .log__table input {
    text-align: center;
    font-size: 20px;
  }

  @media (max-width: 991px) {
    .log__table input {
      font-size: 18px;
    }
  }

  @media (max-width: 850px) {
    .log__table input {
      font-size: 16px;
    }
  }

  @media (max-width: 768px) {
    .log__table input {
      font-size: 20px;
    }
  }

  @media (max-width: 430px) {
    .log__table input {
      font-size: 18px;
    }
  }

  .log__table input:focus {
    outline: none;
  }

  .log__table input::-webkit-outer-spin-button,
  .log__table input::-webkit-inner-spin-button {
    -webkit-appearance: none;
    margin: 0;
  }

  .log__table-bottom {
    display: flex;
    justify-content: space-between;
    gap: 20px;
  }

  .log__table-bottom table:first-child {
    width: 300px;
  }

  .log__table-bottom table:last-child {
    width: 100%;
  }

  .log__table th {
    height: 84px;
  }

  .log__table-half {
    height: 42px !important;
  }

  .log__buttons {
    margin-top: 20px;
    display: flex;
    justify-content: center;
    gap: 40px;
  }

  @media (max-width: 991px) {
    .log__buttons {
      justify-content: space-around;
    }
  }

  @media (max-width: 480px) {
    .log__buttons {
      gap: 20px;
      justify-content: space-between;
    }
  }

  .log__button-add {
    background-color: #000000;
    border: none;
    font-size: 24px;
    color: #fff;
    padding: 10px 30px;
    cursor: pointer;
  }

  @media (any-hover: hover) {
    .log__button-add:hover {
      background-color: #41aa21;
      transition: all 0.3s ease 0s;
    }
  }

  @media (max-width: 480px) {
    .log__button-add {
      padding: 10px 10px;
    }
  }

  .log__button-clear {
    background-color: #fe0000;
    border: none;
    font-size: 24px;
    color: #fff;
    padding: 10px 30px;
    cursor: pointer;
  }

  @media (any-hover: hover) {
    .log__button-clear:hover {
      background-color: #f71a1a;
      transition: all 0.3s ease 0s;
    }
  }

  @media (max-width: 480px) {
    .log__button-clear {
      padding: 10px 10px;
    }
  }

  .log__table-mobile-2 {
    display: none;
  }

  .log__table-mobile-3 {
    display: none;
  }

  .log__table-mobile-4 {
    display: none;
  }

  .log__nav {
    margin-top: 40px;
    display: flex;
    align-items: center;
    justify-content: space-around;
    font-size: 24px;
  }

  .log__nav-button {
    padding: 10px 30px;
    border: 2px solid #000;
    border-radius: 10px;
    display: flex;
    gap: 20px;
    align-items: center;
    cursor: pointer;
  }

  .log__nav-button span {
    border-right: 1px solid #000;
    height: 24px;
  }

  @media (any-hover: hover) {
    .log__nav-button:hover {
      background-color: #000;
      color: #fff;
      transition: all 0.3s ease 0s;
    }

    .log__nav-button:hover span {
      border-right: 1px solid #fff;
      transition: all 0.3s ease 0s;
    }
  }

  @media (max-width: 480px) {
    .log__nav-button {
      padding: 10px 10px;
    }
  }

  .log__readonly {
    background-color: #377d22 !important;
  }

  .desktop {
    display: block;
  }

  @media (max-width: 768px) {
    .desktop {
      display: none;
    }
  }

  .mobile {
    display: none;
  }

  @media (max-width: 768px) {
    .mobile {
      display: block;
    }
  }

  .row-4,
  .row-5,
  .row-6,
  .row-7,
  .row-8,
  .row-9,
  .row-10,
  .row-11,
  .row-12 {
    display: none;
  }

  .show {
    display: table-row;
  }
</style>

<body class="log">
  <div class="log__container">
    <div class="log__block">
      <div class="log__header">
        <h2 class="log__title">VFR Flight Planner</h2>
        <div class="log__sartime">
          <label>Sartime</label>
          <input type="text" id="sartime">
        </div>
      </div>
      <div class="log__table desktop">
        <table id="table1" class="table1">
          <tr>
            <th rowspan="2">FROM</th>
            <th rowspan="2">TO</th>
            <th rowspan="2">MSA</th>
            <th rowspan="2">CAS</th>
            <th class="log__table-half" colspan="2">ALTITUDE</th>
            <th rowspan="2" class="log__readonly">TAS <br>
              kts</th>
            <th rowspan="2">TRK <br>
              °T
            </th>
            <th class="log__table-half" colspan="2">WIND</th>
            <th rowspan="2">VAR <br>(-E &nbsp; +W)</th>
          </tr>
          <tr>
            <th class="log__table-half">FEET</th>
            <th class="log__table-half">TEMP</th>
            <th class="log__table-half">°T</th>
            <th class="log__table-half">kts</th>
          </tr>
          <tr>
            <td><input class="from1" type="text"></td>
            <td><input class="to1" type="text"></td>
            <td><input class="msa1" type="number"></td>
            <td><input class="cas1" type="number"></td>
            <td><input class="feet1" type="number"></td>
            <td><input class="temp1" type="number"></td>
            <td><input class="tas_kts1" readonly type="text"></td>
            <td><input class="trk_t1" type="number"></td>
            <td><input class="wind_t1" type="number"></td>
            <td><input class="wind_kts1" type="number"></td>
            <td><input class="var_e_w1" type="number"></td>
          </tr>
          <tr>
            <td><input class="from2" type="text"></td>
            <td><input class="to2" type="text"></td>
            <td><input class="msa2" type="number"></td>
            <td><input class="cas2" type="number"></td>
            <td><input class="feet2" type="number"></td>
            <td><input class="temp2" type="number"></td>
            <td><input class="tas_kts2" readonly type="text"></td>
            <td><input class="trk_t2" type="number"></td>
            <td><input class="wind_t2" type="number"></td>
            <td><input class="wind_kts2" type="number"></td>
            <td><input class="var_e_w2" type="number"></td>
          </tr>
          <tr>
            <td><input class="from3" type="text"></td>
            <td><input class="to3" type="text"></td>
            <td><input class="msa3" type="number"></td>
            <td><input class="cas3" type="number"></td>
            <td><input class="feet3" type="number"></td>
            <td><input class="temp3" type="number"></td>
            <td><input class="tas_kts3" readonly type="text"></td>
            <td><input class="trk_t3" type="number"></td>
            <td><input class="wind_t3" type="number"></td>
            <td><input class="wind_kts3" type="number"></td>
            <td><input class="var_e_w3" type="number"></td>
          </tr>
          <tr class="row-4">
            <td><input class="from4" type="text"></td>
            <td><input class="to4" type="text"></td>
            <td><input class="msa4" type="number"></td>
            <td><input class="cas4" type="number"></td>
            <td><input class="feet4" type="number"></td>
            <td><input class="temp4" type="number"></td>
            <td><input class="tas_kts4" readonly type="text"></td>
            <td><input class="trk_t4" type="number"></td>
            <td><input class="wind_t4" type="number"></td>
            <td><input class="wind_kts4" type="number"></td>
            <td><input class="var_e_w4" type="number"></td>
          </tr>
          <tr class="row-5">
            <td><input class="from5" type="text"></td>
            <td><input class="to5" type="text"></td>
            <td><input class="msa5" type="number"></td>
            <td><input class="cas5" type="number"></td>
            <td><input class="feet5" type="number"></td>
            <td><input class="temp5" type="number"></td>
            <td><input class="tas_kts5" readonly type="text"></td>
            <td><input class="trk_t5" type="number"></td>
            <td><input class="wind_t5" type="number"></td>
            <td><input class="wind_kts5" type="number"></td>
            <td><input class="var_e_w5" type="number"></td>
          </tr>
          <tr class="row-6">
            <td><input class="from6" type="text"></td>
            <td><input class="to6" type="text"></td>
            <td><input class="msa6" type="number"></td>
            <td><input class="cas6" type="number"></td>
            <td><input class="feet6" type="number"></td>
            <td><input class="temp6" type="number"></td>
            <td><input class="tas_kts6" readonly type="text"></td>
            <td><input class="trk_t6" type="number"></td>
            <td><input class="wind_t6" type="number"></td>
            <td><input class="wind_kts6" type="number"></td>
            <td><input class="var_e_w6" type="number"></td>
          </tr>
          <tr class="row-7">
            <td><input class="from7" type="text"></td>
            <td><input class="to7" type="text"></td>
            <td><input class="msa7" type="number"></td>
            <td><input class="cas7" type="number"></td>
            <td><input class="feet7" type="number"></td>
            <td><input class="temp7" type="number"></td>
            <td><input class="tas_kts7" readonly type="text"></td>
            <td><input class="trk_t7" type="number"></td>
            <td><input class="wind_t7" type="number"></td>
            <td><input class="wind_kts7" type="number"></td>
            <td><input class="var_e_w7" type="number"></td>
          </tr>
          <tr class="row-8">
            <td><input class="from8" type="text"></td>
            <td><input class="to8" type="text"></td>
            <td><input class="msa8" type="number"></td>
            <td><input class="cas8" type="number"></td>
            <td><input class="feet8" type="number"></td>
            <td><input class="temp8" type="number"></td>
            <td><input class="tas_kts8" readonly type="text"></td>
            <td><input class="trk_t8" type="number"></td>
            <td><input class="wind_t8" type="number"></td>
            <td><input class="wind_kts8" type="number"></td>
            <td><input class="var_e_w8" type="number"></td>
          </tr>
          <tr class="row-9">
            <td><input class="from9" type="text"></td>
            <td><input class="to9" type="text"></td>
            <td><input class="msa9" type="number"></td>
            <td><input class="cas9" type="number"></td>
            <td><input class="feet9" type="number"></td>
            <td><input class="temp9" type="number"></td>
            <td><input class="tas_kts9" readonly type="text"></td>
            <td><input class="trk_t9" type="number"></td>
            <td><input class="wind_t9" type="number"></td>
            <td><input class="wind_kts9" type="number"></td>
            <td><input class="var_e_w9" type="number"></td>
          </tr>
          <tr class="row-10">
            <td><input class="from10" type="text"></td>
            <td><input class="to10" type="text"></td>
            <td><input class="msa10" type="number"></td>
            <td><input class="cas10" type="number"></td>
            <td><input class="feet10" type="number"></td>
            <td><input class="temp10" type="number"></td>
            <td><input class="tas_kts10" readonly type="text"></td>
            <td><input class="trk_t10" type="number"></td>
            <td><input class="wind_t10" type="number"></td>
            <td><input class="wind_kts10" type="number"></td>
            <td><input class="var_e_w10" type="number"></td>
          </tr>

          <tr class="row-11">
            <td><input class="from11" type="text"></td>
            <td><input class="to11" type="text"></td>
            <td><input class="msa11" type="number"></td>
            <td><input class="cas11" type="number"></td>
            <td><input class="feet11" type="number"></td>
            <td><input class="temp11" type="number"></td>
            <td><input class="tas_kts11" readonly type="text"></td>
            <td><input class="trk_t11" type="number"></td>
            <td><input class="wind_t11" type="number"></td>
            <td><input class="wind_kts11" type="number"></td>
            <td><input class="var_e_w11" type="number"></td>
          </tr>

          <tr class="row-12">
            <td><input class="from12" type="text"></td>
            <td><input class="to12" type="text"></td>
            <td><input class="msa12" type="number"></td>
            <td><input class="cas12" type="number"></td>
            <td><input class="feet12" type="number"></td>
            <td><input class="temp12" type="number"></td>
            <td><input class="tas_kts12" readonly type="text"></td>
            <td><input class="trk_t12" type="number"></td>
            <td><input class="wind_t12" type="number"></td>
            <td><input class="wind_kts12" type="number"></td>
            <td><input class="var_e_w12" type="number"></td>
          </tr>
        </table>
        <table id="table2" class="table2">
          <tr>
            <th rowspan="2" class="log__readonly">HDG <br> °M</th>
            <th rowspan="2">DIST <br> nm</th>
            <th rowspan="2" class="log__readonly">G/S <br> kts</th>
            <th rowspan="2" class="log__readonly">EET</th>
            <th rowspan="2">ETA</th>
            <th rowspan="2">REVISED <br> ETA</th>
            <th rowspan="2">ATA</th>
            <th rowspan="2" class="log__readonly">LEG <br> FUEL</th>
            <th rowspan="2">Fuel <br> Burn</th>
            <th rowspan="2" class="log__readonly">FUEL <br> REMAIN</th>
            <th rowspan="2">Fuel on <br> Board</th>
          </tr>
          <tr>
          </tr>
          <tr>
            <td><input class="hdg1" readonly type="text"></td>
            <td><input class="distance_nm1" type="number"></td>
            <td><input class="gs_kts1" readonly type="text"></td>
            <td><input class="eet1" readonly type="text"></td>
            <td><input class="eta1" type="number"></td>
            <td><input class="revised_eta1" type="number"></td>
            <td><input class="ata1" type="number"></td>
            <td><input class="leg_fuel1" readonly type="text"></td>
            <td><input class="fuel_burn1" type="number"></td>
            <td><input class="fuel_remain1" readonly type="text"></td>
            <td><input class="fuel_on_board1" type="number"></td>
          </tr>
          <tr>
            <td><input class="hdg2" readonly type="text"></td>
            <td><input class="distance_nm2" type="number"></td>
            <td><input class="gs_kts2" readonly type="text"></td>
            <td><input class="eet2" readonly type="text"></td>
            <td><input class="eta2" type="number"></td>
            <td><input class="revised_eta2" type="number"></td>
            <td><input class="ata2" type="number"></td>
            <td><input class="leg_fuel2" readonly type="text"></td>
            <td><input class="fuel_burn2" type="number"></td>
            <td><input class="fuel_remain2" readonly type="text"></td>
            <td><input class="fuel_on_board2" type="number"></td>
          </tr>
          <tr>
            <td><input class="hdg3" readonly type="text"></td>
            <td><input class="distance_nm3" type="number"></td>
            <td><input class="gs_kts3" readonly type="text"></td>
            <td><input class="eet3" readonly type="text"></td>
            <td><input class="eta3" type="number"></td>
            <td><input class="revised_eta3" type="number"></td>
            <td><input class="ata3" type="number"></td>
            <td><input class="leg_fuel3" readonly type="text"></td>
            <td><input class="fuel_burn3" type="number"></td>
            <td><input class="fuel_remain3" readonly type="text"></td>
            <td><input class="fuel_on_board3" type="number"></td>
          </tr>
          <tr class="row-4">
            <td><input class="hdg4" readonly type="text"></td>
            <td><input class="distance_nm4" type="number"></td>
            <td><input class="gs_kts4" readonly type="text"></td>
            <td><input class="eet4" readonly type="text"></td>
            <td><input class="eta4" type="number"></td>
            <td><input class="revised_eta4" type="number"></td>
            <td><input class="ata4" type="number"></td>
            <td><input class="leg_fuel4" readonly type="text"></td>
            <td><input class="fuel_burn4" type="number"></td>
            <td><input class="fuel_remain4" readonly type="text"></td>
            <td><input class="fuel_on_board4" type="number"></td>
          </tr>
          <tr class="row-5">
            <td><input class="hdg5" readonly type="text"></td>
            <td><input class="distance_nm5" type="number"></td>
            <td><input class="gs_kts5" readonly type="text"></td>
            <td><input class="eet5" readonly type="text"></td>
            <td><input class="eta5" type="number"></td>
            <td><input class="revised_eta5" type="number"></td>
            <td><input class="ata5" type="number"></td>
            <td><input class="leg_fuel5" readonly type="text"></td>
            <td><input class="fuel_burn5" type="number"></td>
            <td><input class="fuel_remain5" readonly type="text"></td>
            <td><input class="fuel_on_board5" type="number"></td>
          </tr>
          <tr class="row-6">
            <td><input class="hdg6" readonly type="text"></td>
            <td><input class="distance_nm6" type="number"></td>
            <td><input class="gs_kts6" readonly type="text"></td>
            <td><input class="eet6" readonly type="text"></td>
            <td><input class="eta6" type="number"></td>
            <td><input class="revised_eta6" type="number"></td>
            <td><input class="ata6" type="number"></td>
            <td><input class="leg_fuel6" readonly type="text"></td>
            <td><input class="fuel_burn6" type="number"></td>
            <td><input class="fuel_remain6" readonly type="text"></td>
            <td><input class="fuel_on_board6" type="number"></td>
          </tr>

          <tr class="row-7">
            <td><input class="hdg7" readonly type="text"></td>
            <td><input class="distance_nm7" type="number"></td>
            <td><input class="gs_kts7" readonly type="text"></td>
            <td><input class="eet7" readonly type="text"></td>
            <td><input class="eta7" type="number"></td>
            <td><input class="revised_eta7" type="number"></td>
            <td><input class="ata7" type="number"></td>
            <td><input class="leg_fuel7" readonly type="text"></td>
            <td><input class="fuel_burn7" type="number"></td>
            <td><input class="fuel_remain7" readonly type="text"></td>
            <td><input class="fuel_on_board7" type="number"></td>
          </tr>
          <tr class="row-8">
            <td><input class="hdg8" readonly type="text"></td>
            <td><input class="distance_nm8" type="number"></td>
            <td><input class="gs_kts8" readonly type="text"></td>
            <td><input class="eet8" readonly type="text"></td>
            <td><input class="eta8" type="number"></td>
            <td><input class="revised_eta8" type="number"></td>
            <td><input class="ata8" type="number"></td>
            <td><input class="leg_fuel8" readonly type="text"></td>
            <td><input class="fuel_burn8" type="number"></td>
            <td><input class="fuel_remain8" readonly type="text"></td>
            <td><input class="fuel_on_board8" type="number"></td>
          </tr>
          <tr class="row-9">
            <td><input class="hdg9" readonly type="text"></td>
            <td><input class="distance_nm9" type="number"></td>
            <td><input class="gs_kts9" readonly type="text"></td>
            <td><input class="eet9" readonly type="text"></td>
            <td><input class="eta9" type="number"></td>
            <td><input class="revised_eta9" type="number"></td>
            <td><input class="ata9" type="number"></td>
            <td><input class="leg_fuel9" readonly type="text"></td>
            <td><input class="fuel_burn9" type="number"></td>
            <td><input class="fuel_remain9" readonly type="text"></td>
            <td><input class="fuel_on_board9" type="number"></td>
          </tr>
          <tr class="row-10">
            <td><input class="hdg10" readonly type="text"></td>
            <td><input class="distance_nm10" type="number"></td>
            <td><input class="gs_kts10" readonly type="text"></td>
            <td><input class="eet10" readonly type="text"></td>
            <td><input class="eta10" type="number"></td>
            <td><input class="revised_eta10" type="number"></td>
            <td><input class="ata10" type="number"></td>
            <td><input class="leg_fuel10" readonly type="text"></td>
            <td><input class="fuel_burn10" type="number"></td>
            <td><input class="fuel_remain10" readonly type="text"></td>
            <td><input class="fuel_on_board10" type="number"></td>
          </tr>

          <tr class="row-11">
            <td><input class="hdg11" readonly type="text"></td>
            <td><input class="distance_nm11" type="number"></td>
            <td><input class="gs_kts11" readonly type="text"></td>
            <td><input class="eet11" readonly type="text"></td>
            <td><input class="eta11" type="number"></td>
            <td><input class="revised_eta11" type="number"></td>
            <td><input class="ata11" type="number"></td>
            <td><input class="leg_fuel11" readonly type="text"></td>
            <td><input class="fuel_burn11" type="number"></td>
            <td><input class="fuel_remain11" readonly type="text"></td>
            <td><input class="fuel_on_board11" type="number"></td>
          </tr>

          <tr class="row-12">
            <td><input class="hdg12" readonly type="text"></td>
            <td><input class="distance_nm12" type="number"></td>
            <td><input class="gs_kts12" readonly type="text"></td>
            <td><input class="eet12" readonly type="text"></td>
            <td><input class="eta12" type="number"></td>
            <td><input class="revised_eta12" type="number"></td>
            <td><input class="ata12" type="number"></td>
            <td><input class="leg_fuel12" readonly type="text"></td>
            <td><input class="fuel_burn12" type="number"></td>
            <td><input class="fuel_remain12" readonly type="text"></td>
            <td><input class="fuel_on_board12" type="number"></td>
          </tr>
        </table>
        <div class="log__table-bottom">
          <table id="table3" class="table3">
            <tr>
              <th rowspan="2">Start,<br> Taxi</th>
              <th rowspan="2">Reserve <br> Fuel</th>
            </tr>
            <tr>
            </tr>
            <tr>
              <td><input class="start_taxi1" type="number"></td>
              <td><input class="reserve_fuel1" type="number"></td>
            </tr>
            <tr>
              <td><input class="start_taxi2" type="number"></td>
              <td><input class="reserve_fuel2" type="number"></td>
            </tr>
            <tr>
              <td><input class="start_taxi3" type="number"></td>
              <td><input class="reserve_fuel3" type="number"></td>
            </tr>
            <tr class="row-4">
              <td><input class="start_taxi4" type="number"></td>
              <td><input class="reserve_fuel4" type="number"></td>
            </tr>
            <tr class="row-5">
              <td><input class="start_taxi5" type="number"></td>
              <td><input class="reserve_fuel5" type="number"></td>
            </tr>
            <tr class="row-6">
              <td><input class="start_taxi6" type="number"></td>
              <td><input class="reserve_fuel6" type="number"></td>
            </tr>
            <tr class="row-7">
              <td><input class="start_taxi7" type="number"></td>
              <td><input class="reserve_fuel7" type="number"></td>
            </tr>
            <tr class="row-8">
              <td><input class="start_taxi8" type="number"></td>
              <td><input class="reserve_fuel8" type="number"></td>
            </tr>
            <tr class="row-9">
              <td><input class="start_taxi9" type="number"></td>
              <td><input class="reserve_fuel9" type="number"></td>
            </tr>
            <tr class="row-10">
              <td><input class="start_taxi10" type="number"></td>
              <td><input class="reserve_fuel10" type="number"></td>
            </tr>
            <tr class="row-11">
              <td><input class="start_taxi11" type="number"></td>
              <td><input class="reserve_fuel11" type="number"></td>
            </tr>
            <tr class="row-12">
              <td><input class="start_taxi12" type="number"></td>
              <td><input class="reserve_fuel12" type="number"></td>
            </tr>
          </table>
          <table id="table4" class="table4">
            <tr>
              <th rowspan="2">NOTES</th>
            </tr>
            <tr>
            </tr>
            <tr>
              <td><input class="notes1" type="text"></td>
            </tr>
            <tr>
              <td><input class="notes2" type="text"></td>
            </tr>
            <tr>
              <td><input class="notes3" type="text"></td>
            </tr>
            <tr class="row-4">
              <td><input class="notes4" type="text"></td>
            </tr>
            <tr class="row-5">
              <td><input class="notes5" type="text"></td>
            </tr>

            <tr class="row-6">
              <td><input class="notes6" type="text"></td>
            </tr>

            <tr class="row-7">
              <td><input class="notes7" type="text"></td>
            </tr>

            <tr class="row-8">
              <td><input class="notes8" type="text"></td>
            </tr>

            <tr class="row-9">
              <td><input class="notes9" type="text"></td>
            </tr>
            <tr class="row-10">
              <td><input class="notes10" type="text"></td>
            </tr>

            <tr class="row-11">
              <td><input class="notes11" type="text"></td>
            </tr>

            <tr class="row-12">
              <td><input class="notes12" type="text"></td>
            </tr>
          </table>
        </div>
        <div class="log__buttons">
          <button class="log__button-add" onclick="addRows()" type="submit">Add New Line</button>
          <button class="log__button-clear" onclick="clearRows()" type="reset">CLEAR</button>
        </div>
      </div>
      <div class="log__table mobile">
        <div class="log__table-mobile">
          <table id="mobile1" class="mobile1">
            <tr>
              <th rowspan="2">FROM</th>
              <th rowspan="2">TO</th>
              <th rowspan="2">MSA</th>
              <th rowspan="2">CAS</th>
            </tr>
            <tr>
            </tr>
            <tr>
              <td><input class="from13" type="text"></td>
              <td><input class="to13" type="text"></td>
              <td><input class="msa13" type="number"></td>
              <td><input class="cas13 " type="number"></td>
            </tr>
            <tr>
              <td><input class="from14" type="text"></td>
              <td><input class="to14" type="text"></td>
              <td><input class="msa14" type="number"></td>
              <td><input class="cas14" type="number"></td>
            </tr>
            <tr>
              <td><input class="from15" type="text"></td>
              <td><input class="to15" type="text"></td>
              <td><input class="msa15" type="number"></td>
              <td><input class="cas15" type="number"></td>
            </tr>
            <tr class="row-4">
              <td><input class="from16" type="text"></td>
              <td><input class="to16" type="text"></td>
              <td><input class="msa16" type="number"></td>
              <td><input class="cas16" type="number"></td>
            </tr>
            <tr class="row-5">
              <td><input class="from17" type="text"></td>
              <td><input class="to17" type="text"></td>
              <td><input class="msa17" type="number"></td>
              <td><input class="cas17" type="number"></td>
            </tr>
            <tr class="row-6">
              <td><input class="from18" type="text"></td>
              <td><input class="to18" type="text"></td>
              <td><input class="msa18" type="number"></td>
              <td><input class="cas18" type="number"></td>
            </tr>
            <tr class="row-7">
              <td><input class="from19" type="text"></td>
              <td><input class="to19" type="text"></td>
              <td><input class="msa19" type="number"></td>
              <td><input class="cas19" type="number"></td>
            </tr>
            <tr class="row-8">
              <td><input class="from20" type="text"></td>
              <td><input class="to20" type="text"></td>
              <td><input class="msa20" type="number"></td>
              <td><input class="cas20" type="number"></td>
            </tr>
            <tr class="row-9">
              <td><input class="from21" type="text"></td>
              <td><input class="to21" type="text"></td>
              <td><input class="msa21" type="number"></td>
              <td><input class="cas21" type="number"></td>
            </tr>
            <tr class="row-10">
              <td><input class="from22" type="text"></td>
              <td><input class="to22" type="text"></td>
              <td><input class="msa22" type="number"></td>
              <td><input class="cas22" type="number"></td>
            </tr>
            <tr class="row-11">
              <td><input class="from23" type="text"></td>
              <td><input class="to23" type="text"></td>
              <td><input class="msa23" type="number"></td>
              <td><input class="cas23" type="number"></td>
            </tr>
            <tr class="row-12">
              <td><input class="from24" type="text"></td>
              <td><input class="to24" type="text"></td>
              <td><input class="msa24" type="number"></td>
              <td><input class="cas24" type="number"></td>
            </tr>

          </table>
          <table id="mobile2" class="mobile2">
            <tr>
              <th class="log__table-half" colspan="2">ALTITUDE</th>
              <th rowspan="2" class="log__readonly">TAS <br>kts</th>
              <th rowspan="2">TRK <br>°T</th>
            </tr>
            <tr>
              <th class="log__table-half">FEET</th>
              <th class="log__table-half">TEMP</th>
            </tr>
            <tr>
              <td><input class="feet13" type="number"></td>
              <td><input class="temp13" type="number"></td>
              <td><input class="tas_kts13" readonly type="text"></td>
              <td><input class="trk_t13" type="number"></td>
            </tr>
            <tr>
              <td><input class="feet14" type="number"></td>
              <td><input class="temp14" type="number"></td>
              <td><input class="tas_kts14" readonly type="text"></td>
              <td><input class="trk_t14" type="number"></td>
            </tr>
            <tr>
              <td><input class="feet15" type="number"></td>
              <td><input class="temp15" type="number"></td>
              <td><input class="tas_kts15" readonly type="text"></td>
              <td><input class="trk_t15" type="number"></td>
            </tr>
            <tr class="row-4">
              <td><input class="feet16" type="number"></td>
              <td><input class="temp16" type="number"></td>
              <td><input class="tas_kts16" readonly type="text"></td>
              <td><input class="trk_t16" type="number"></td>
            </tr>
            <tr class="row-5">
              <td><input class="feet17" type="number"></td>
              <td><input class="temp17" type="number"></td>
              <td><input class="tas_kts17" readonly type="text"></td>
              <td><input class="trk_t17" type="number"></td>
            </tr>
            <tr class="row-6">
              <td><input class="feet18" type="number"></td>
              <td><input class="temp18" type="number"></td>
              <td><input class="tas_kts18" readonly type="text"></td>
              <td><input class="trk_t18" type="number"></td>
            </tr>
            <tr class="row-7">
              <td><input class="feet19" type="number"></td>
              <td><input class="temp19" type="number"></td>
              <td><input class="tas_kts19" readonly type="text"></td>
              <td><input class="trk_t19" type="number"></td>
            </tr>
            <tr class="row-8">
              <td><input class="feet20" type="number"></td>
              <td><input class="temp20" type="number"></td>
              <td><input class="tas_kts20" readonly type="text"></td>
              <td><input class="trk_t20" type="number"></td>
            </tr>
            <tr class="row-9">
              <td><input class="feet21" type="number"></td>
              <td><input class="temp21" type="number"></td>
              <td><input class="tas_kts21" readonly type="text"></td>
              <td><input class="trk_t21" type="number"></td>
            </tr>
            <tr class="row-10">
              <td><input class="feet22" type="number"></td>
              <td><input class="temp22" type="number"></td>
              <td><input class="tas_kts22" readonly type="text"></td>
              <td><input class="trk_t22" type="number"></td>
            </tr>
            <tr class="row-11">
              <td><input class="feet23" type="number"></td>
              <td><input class="temp23" type="number"></td>
              <td><input class="tas_kts23" readonly type="text"></td>
              <td><input class="trk_t23" type="number"></td>
            </tr>
            <tr class="row-12">
              <td><input class="feet24" type="number"></td>
              <td><input class="temp24" type="number"></td>
              <td><input class="tas_kts24" readonly type="text"></td>
              <td><input class="trk_t24" type="number"></td>
            </tr>

          </table>
          <div class="log__buttons">
            <button class="log__button-add" onclick="addRows()" type="submit">Add New Line</button>
            <button class="log__button-clear" onclick="clearRows()" type="reset">CLEAR</button>
          </div>
          <div class="log__nav" style="justify-content: flex-end;">
            <a onclick="nextBlocks()" class="log__nav-button">NEXT <span></span> <svg width="24" height="24"
                fill="#8edab5" xmlns="http://www.w3.org/2000/svg" fill-rule="evenodd" clip-rule="evenodd">
                <path d="M21.883 12l-7.527 6.235.644.765 9-7.521-9-7.479-.645.764 7.529 6.236h-21.884v1h21.883z" />
              </svg></a>
          </div>
        </div>
        <div class="log__table-mobile" style="display: none;">
          <table id="mobile3" class="mobile3">
            <tr>
              <th class="log__table-half" colspan="2">WIND</th>
              <th rowspan="2">VAR <br>(-E &nbsp; +W)</th>
              <th rowspan="2" class="log__readonly">HDG <br> °M</th>
            </tr>
            <tr>
              <th class="log__table-half">°T</th>
              <th class="log__table-half">kts</th>
            </tr>
            <tr>
              <td><input class="wind_t13" type="number"></td>
              <td><input class="wind_kts13" type="number"></td>
              <td><input class="var_e_w13" type="number"></td>
              <td><input class="hdg13" readonly type="text"></td>
            </tr>

            <tr>
              <td><input class="wind_t14" type="number"></td>
              <td><input class="wind_kts14" type="number"></td>
              <td><input class="var_e_w14" type="number"></td>
              <td><input class="hdg14" readonly type="text"></td>
            </tr>

            <tr>
              <td><input class="wind_t15" type="number"></td>
              <td><input class="wind_kts15" type="number"></td>
              <td><input class="var_e_w15" type="number"></td>
              <td><input class="hdg15" readonly type="text"></td>
            </tr>
            <tr class="row-4">
              <td><input class="wind_t16" type="number"></td>
              <td><input class="wind_kts16" type="number"></td>
              <td><input class="var_e_w16" type="number"></td>
              <td><input class="hdg16" readonly type="text"></td>
            </tr>

            <tr class="row-5">
              <td><input class="wind_t17" type="number"></td>
              <td><input class="wind_kts17" type="number"></td>
              <td><input class="var_e_w17" type="number"></td>
              <td><input class="hdg17" readonly type="text"></td>
            </tr>

            <tr class="row-6">
              <td><input class="wind_t18" type="number"></td>
              <td><input class="wind_kts18" type="number"></td>
              <td><input class="var_e_w18" type="number"></td>
              <td><input class="hdg18" readonly type="text"></td>
            </tr>

            <tr class="row-7">
              <td><input class="wind_t19" type="number"></td>
              <td><input class="wind_kts19" type="number"></td>
              <td><input class="var_e_w19" type="number"></td>
              <td><input class="hdg19" readonly type="text"></td>
            </tr>

            <tr class="row-8">
              <td><input class="wind_t20" type="number"></td>
              <td><input class="wind_kts20" type="number"></td>
              <td><input class="var_e_w20" type="number"></td>
              <td><input class="hdg20" readonly type="text"></td>
            </tr>

            <tr class="row-9">
              <td><input class="wind_t21" type="number"></td>
              <td><input class="wind_kts21" type="number"></td>
              <td><input class="var_e_w21" type="number"></td>
              <td><input class="hdg21" readonly type="text"></td>
            </tr>
            <tr class="row-10">
              <td><input class="wind_t22" type="number"></td>
              <td><input class="wind_kts22" type="number"></td>
              <td><input class="var_e_w22" type="number"></td>
              <td><input class="hdg22" readonly type="text"></td>
            </tr>
            <tr class="row-11">
              <td><input class="wind_t23" type="number"></td>
              <td><input class="wind_kts23" type="number"></td>
              <td><input class="var_e_w23" type="number"></td>
              <td><input class="hdg23" readonly type="text"></td>
            </tr>
            <tr class="row-12">
              <td><input class="wind_t24" type="number"></td>
              <td><input class="wind_kts24" type="number"></td>
              <td><input class="var_e_w24" type="number"></td>
              <td><input class="hdg24" readonly type="text"></td>
            </tr>

          </table>
          <table id="mobile4" class="mobile4">
            <tr>
              <th rowspan="2">DIST <br> nm</th>
              <th rowspan="2" class="log__readonly">G/S <br> kts</th>
              <th rowspan="2" class="log__readonly">EET</th>
              <th rowspan="2">ETA</th>
            </tr>
            <tr>
            </tr>
            <tr>
              <td><input class="distance_nm13" type="number"></td>
              <td><input class="gs_kts13" readonly type="text"></td>
              <td><input class="eet13" readonly type="text"></td>
              <td><input class="eta13" type="number"></td>
            </tr>

            <tr>
              <td><input class="distance_nm14" type="number"></td>
              <td><input class="gs_kts14" readonly type="text"></td>
              <td><input class="eet14" readonly type="text"></td>
              <td><input class="eta14" type="number"></td>
            </tr>

            <tr>
              <td><input class="distance_nm15" type="number"></td>
              <td><input class="gs_kts15" readonly type="text"></td>
              <td><input class="eet15" readonly type="text"></td>
              <td><input class="eta15" type="number"></td>
            </tr>

            <tr class="row-4">
              <td><input class="distance_nm16" type="number"></td>
              <td><input class="gs_kts16" readonly type="text"></td>
              <td><input class="eet16" readonly type="text"></td>
              <td><input class="eta16" type="number"></td>
            </tr>

            <tr class="row-5">
              <td><input class="distance_nm17" type="number"></td>
              <td><input class="gs_kts17" readonly type="text"></td>
              <td><input class="eet17" readonly type="text"></td>
              <td><input class="eta17" type="number"></td>
            </tr>

            <tr class="row-6">
              <td><input class="distance_nm18" type="number"></td>
              <td><input class="gs_kts18" readonly type="text"></td>
              <td><input class="eet18" readonly type="text"></td>
              <td><input class="eta18" type="number"></td>
            </tr>

            <tr class="row-7">
              <td><input class="distance_nm19" type="number"></td>
              <td><input class="gs_kts19" readonly type="text"></td>
              <td><input class="eet19" readonly type="text"></td>
              <td><input class="eta19" type="number"></td>
            </tr>

            <tr class="row-8">
              <td><input class="distance_nm20" type="number"></td>
              <td><input class="gs_kts20" readonly type="text"></td>
              <td><input class="eet20" readonly type="text"></td>
              <td><input class="eta20" type="number"></td>
            </tr>
            <tr class="row-9">
              <td><input class="distance_nm21" type="number"></td>
              <td><input class="gs_kts21" readonly type="text"></td>
              <td><input class="eet21" readonly type="text"></td>
              <td><input class="eta21" type="number"></td>
            </tr>
            <tr class="row-10">
              <td><input class="distance_nm22" type="number"></td>
              <td><input class="gs_kts22" readonly type="text"></td>
              <td><input class="eet22" readonly type="text"></td>
              <td><input class="eta22" type="number"></td>
            </tr>
            <tr class="row-11">
              <td><input class="distance_nm23" type="number"></td>
              <td><input class="gs_kts23" readonly type="text"></td>
              <td><input class="eet23" readonly type="text"></td>
              <td><input class="eta23" type="number"></td>
            </tr>
            <tr class="row-12">
              <td><input class="distance_nm24" type="number"></td>
              <td><input class="gs_kts24" readonly type="text"></td>
              <td><input class="eet24" readonly type="text"></td>
              <td><input class="eta24" type="number"></td>
            </tr>
          </table>
          <div class="log__nav">
            <a onclick="previousBlock()" class="log__nav-button"> <svg width="24" height="24" fill="#377d22"
                xmlns="http://www.w3.org/2000/svg" fill-rule="evenodd" clip-rule="evenodd">
                <path d="M2.117 12l7.527 6.235-.644.765-9-7.521 9-7.479.645.764-7.529 6.236h21.884v1h-21.883z" />
              </svg><span></span>BACK</a>
            <a onclick="nextBlocks()" class="log__nav-button">NEXT <span></span> <svg width="24" height="24"
                fill="#8edab5" xmlns="http://www.w3.org/2000/svg" fill-rule="evenodd" clip-rule="evenodd">
                <path d="M21.883 12l-7.527 6.235.644.765 9-7.521-9-7.479-.645.764 7.529 6.236h-21.884v1h21.883z" />
              </svg></a>

          </div>
        </div>
        <div class="log__table-mobile" style="display: none;">
          <table id="mobile5" class="mobile5">
            <tr>
              <th rowspan="2">REVISED <br> ETA</th>
              <th rowspan="2">ATA</th>
              <th rowspan="2" class="log__readonly">LEG <br> FUEL</th>
              <th rowspan="2">Fuel <br> Burn</th>
            </tr>
            <tr>
            </tr>
            <tr>
              <td><input class="revised_eta13" type="number"></td>
              <td><input class="ata13" type="number"></td>
              <td><input class="leg_fuel13" readonly type="text"></td>
              <td><input class="fuel_burn13" type="number"></td>
            </tr>
            <tr>
              <td><input class="revised_eta14" type="number"></td>
              <td><input class="ata14" type="number"></td>
              <td><input class="leg_fuel14" readonly type="text"></td>
              <td><input class="fuel_burn14" type="number"></td>
            </tr>
            <tr>
              <td><input class="revised_eta15" type="number"></td>
              <td><input class="ata15" type="number"></td>
              <td><input class="leg_fuel15" readonly type="text"></td>
              <td><input class="fuel_burn15" type="number"></td>
            </tr>
            <tr class="row-4">
              <td><input class="revised_eta16" type="number"></td>
              <td><input class="ata16" type="number"></td>
              <td><input class="leg_fuel16" readonly type="text"></td>
              <td><input class="fuel_burn16" type="number"></td>
            </tr>
            <tr class="row-5">
              <td><input class="revised_eta17" type="number"></td>
              <td><input class="ata17" type="number"></td>
              <td><input class="leg_fuel17" readonly type="text"></td>
              <td><input class="fuel_burn17" type="number"></td>
            </tr>
            <tr class="row-6">
              <td><input class="revised_eta18" type="number"></td>
              <td><input class="ata18" type="number"></td>
              <td><input class="leg_fuel18" readonly type="text"></td>
              <td><input class="fuel_burn18" type="number"></td>
            </tr>
            <tr class="row-7">
              <td><input class="revised_eta19" type="number"></td>
              <td><input class="ata19" type="number"></td>
              <td><input class="leg_fuel19" readonly type="text"></td>
              <td><input class="fuel_burn19" type="number"></td>
            </tr>
            <tr class="row-8">
              <td><input class="revised_eta20" type="number"></td>
              <td><input class="ata20" type="number"></td>
              <td><input class="leg_fuel20" readonly type="text"></td>
              <td><input class="fuel_burn20" type="number"></td>
            </tr>
            <tr class="row-9">
              <td><input class="revised_eta21" type="number"></td>
              <td><input class="ata21" type="number"></td>
              <td><input class="leg_fuel21" readonly type="text"></td>
              <td><input class="fuel_burn21" type="number"></td>
            </tr>
            <tr class="row-10">
              <td><input class="revised_eta22" type="number"></td>
              <td><input class="ata22" type="number"></td>
              <td><input class="leg_fuel22" readonly type="text"></td>
              <td><input class="fuel_burn22" type="number"></td>
            </tr>
            <tr class="row-11">
              <td><input class="revised_eta23" type="number"></td>
              <td><input class="ata23" type="number"></td>
              <td><input class="leg_fuel23" readonly type="text"></td>
              <td><input class="fuel_burn23" type="number"></td>
            </tr>
            <tr class="row-12">
              <td><input class="revised_eta24" type="number"></td>
              <td><input class="ata24" type="number"></td>
              <td><input class="leg_fuel24" readonly type="text"></td>
              <td><input class="fuel_burn24" type="number"></td>
            </tr>
          </table>
          <table id="mobile6" class="mobile6">
            <tr>
              <th rowspan="2" class="log__readonly">FUEL <br> REMAIN</th>
              <th rowspan="2">Fuel on <br> Board</th>
              <th rowspan="2">Start,<br> Taxi</th>
              <th rowspan="2">Reserve <br> Fuel</th>
            </tr>
            <tr>
            </tr>
            <tr>
              <td><input class="fuel_remain13" readonly type="text"></td>
              <td><input class="fuel_on_board13" type="number"></td>
              <td><input class="start_taxi13" type="number"></td>
              <td><input class="reserve_fuel13" type="number"></td>
            </tr>
            <tr>
              <td><input class="fuel_remain14" readonly type="text"></td>
              <td><input class="fuel_on_board14" type="number"></td>
              <td><input class="start_taxi14" type="number"></td>
              <td><input class="reserve_fuel14" type="number"></td>
            </tr>
            <tr>
              <td><input class="fuel_remain15" readonly type="text"></td>
              <td><input class="fuel_on_board15" type="number"></td>
              <td><input class="start_taxi15" type="number"></td>
              <td><input class="reserve_fuel15" type="number"></td>
            </tr>
            <tr class="row-4">
              <td><input class="fuel_remain16" readonly type="text"></td>
              <td><input class="fuel_on_board16" type="number"></td>
              <td><input class="start_taxi16" type="number"></td>
              <td><input class="reserve_fuel16" type="number"></td>
            </tr>
            <tr class="row-5">
              <td><input class="fuel_remain17" readonly type="text"></td>
              <td><input class="fuel_on_board17" type="number"></td>
              <td><input class="start_taxi17" type="number"></td>
              <td><input class="reserve_fuel17" type="number"></td>
            </tr>
            <tr class="row-6">
              <td><input class="fuel_remain18" readonly type="text"></td>
              <td><input class="fuel_on_board18" type="number"></td>
              <td><input class="start_taxi18" type="number"></td>
              <td><input class="reserve_fuel18" type="number"></td>
            </tr>
            <tr class="row-7">
              <td><input class="fuel_remain19" readonly type="text"></td>
              <td><input class="fuel_on_board19" type="number"></td>
              <td><input class="start_taxi19" type="number"></td>
              <td><input class="reserve_fuel19" type="number"></td>
            </tr>
            <tr class="row-8">
              <td><input class="fuel_remain20" readonly type="text"></td>
              <td><input class="fuel_on_board20" type="number"></td>
              <td><input class="start_taxi20" type="number"></td>
              <td><input class="reserve_fuel20" type="number"></td>
            </tr>
            <tr class="row-9">
              <td><input class="fuel_remain21" readonly type="text"></td>
              <td><input class="fuel_on_board21" type="number"></td>
              <td><input class="start_taxi21" type="number"></td>
              <td><input class="reserve_fuel21" type="number"></td>
            </tr>
            <tr class="row-10">
              <td><input class="fuel_remain22" readonly type="text"></td>
              <td><input class="fuel_on_board22" type="number"></td>
              <td><input class="start_taxi22" type="number"></td>
              <td><input class="reserve_fuel22" type="number"></td>
            </tr>
            <tr class="row-11">
              <td><input class="fuel_remain23" readonly type="text"></td>
              <td><input class="fuel_on_board23" type="number"></td>
              <td><input class="start_taxi23" type="number"></td>
              <td><input class="reserve_fuel23" type="number"></td>
            </tr>
            <tr class="row-12">
              <td><input class="fuel_remain24" readonly type="text"></td>
              <td><input class="fuel_on_board24" type="number"></td>
              <td><input class="start_taxi24" type="number"></td>
              <td><input class="reserve_fuel24" type="number"></td>
            </tr>
          </table>
          <div class="log__nav">
            <a onclick="previousBlock()" class="log__nav-button"> <svg width="24" height="24" fill="#377d22"
                xmlns="http://www.w3.org/2000/svg" fill-rule="evenodd" clip-rule="evenodd">
                <path d="M2.117 12l7.527 6.235-.644.765-9-7.521 9-7.479.645.764-7.529 6.236h21.884v1h-21.883z" />
              </svg><span></span>BACK</a>
            <a onclick="nextBlocks()" class="log__nav-button">NEXT <span></span> <svg width="24" height="24"
                fill="#8edab5" xmlns="http://www.w3.org/2000/svg" fill-rule="evenodd" clip-rule="evenodd">
                <path d="M21.883 12l-7.527 6.235.644.765 9-7.521-9-7.479-.645.764 7.529 6.236h-21.884v1h21.883z" />
              </svg></a>

          </div>
        </div>
        <div class="log__table-mobile" style="display: none;">
          <table id="mobile7" class="mobile7">
            <tr>
              <th rowspan="2">NOTES</th>
            </tr>
            <tr>
            </tr>
            <tr>
              <td><input class="notes13" type="text"></td>
            </tr>
            <tr>
              <td><input class="notes14" type="text"></td>
            </tr>
            <tr>
              <td><input class="notes15" type="text"></td>
            </tr>
            <tr class="row-4">
              <td><input class="notes16" type="text"></td>
            </tr>
            <tr class="row-5">
              <td><input class="notes17" type="text"></td>
            </tr>
            <tr class="row-6">
              <td><input class="notes18" type="text"></td>
            </tr>
            <tr class="row-7">
              <td><input class="notes19" type="text"></td>
            </tr>
            <tr class="row-8">
              <td><input class="notes20" type="text"></td>
            </tr>
            <tr class="row-9">
              <td><input class="notes21" type="text"></td>
            </tr>
            <tr class="row-10">
              <td><input class="notes22" type="text"></td>
            </tr>
            <tr class="row-11">
              <td><input class="notes23" type="text"></td>
            </tr>
            <tr class="row-12">
              <td><input class="notes24" type="text"></td>
            </tr>
          </table>
          <div class="log__nav" style="justify-content: flex-start;">
            <a onclick="previousBlock()" class="log__nav-button"> <svg width="24" height="24" fill="#377d22"
                xmlns="http://www.w3.org/2000/svg" fill-rule="evenodd" clip-rule="evenodd">
                <path d="M2.117 12l7.527 6.235-.644.765-9-7.521 9-7.479.645.764-7.529 6.236h21.884v1h-21.883z" />
              </svg><span></span>BACK</a>
          </div>
        </div>
      </div>
    </div>
  </div>
<script>
  function hideBlock(index) {
  blocks[index].style.display = "none";
}

function showBlock(index) {
  blocks[index].style.display = "block";
}

var blocks = document.getElementsByClassName("log__table-mobile");
var currentIndex = 0;

function nextBlocks() {
  if (blocks.length === 0) return;
  hideBlock(currentIndex);
  currentIndex++;
  if (currentIndex >= blocks.length) {
    currentIndex = 0;
  }
  showBlock(currentIndex);
}

function previousBlock() {
  if (blocks.length === 0) return;
  hideBlock(currentIndex);
  currentIndex--;
  if (currentIndex < 0) {
    currentIndex = blocks.length - 1;
  }
  showBlock(currentIndex);
}

const allRows = document.querySelectorAll('.row-4, .row-5, .row-6, .row-7, .row-8, .row-9, .row-10, .row-11, .row-12');
const rows = [document.querySelectorAll('.row-4'), document.querySelectorAll('.row-5'), document.querySelectorAll('.row-6'), document.querySelectorAll('.row-7'), document.querySelectorAll('.row-8'), document.querySelectorAll('.row-9'), document.querySelectorAll('.row-10'), document.querySelectorAll('.row-11'), document.querySelectorAll('.row-12')];
let clickCounter = 0;

function addRows() {
  clickCounter++;
  if (clickCounter > 0 && clickCounter <= 9) {
    rows[clickCounter - 1].forEach(row => row.classList.add('show'));
  }
}

function clearRows() {
  allRows.forEach(row => row.classList.remove('show'));
  document.querySelectorAll('input').forEach(input => input.value = '');
  clickCounter = 0;
}

document.addEventListener("input", function () {
  const airports = [
    { code: "NZLX", lat1: 45.21166667, lat2: 169.3733333 },
{ code: "NZAN", lat1: 43.79374722, lat2: 171.3939389 },
{ code: "NZAR", lat1: 37.02972222, lat2: 174.9733333 },
{ code: "NZAS", lat1: 43.90333333, lat2: 171.7966667 },
{ code: "NZAM", lat1: 43.89416667, lat2: 171.7480556 },
{ code: "NZAA", lat1: 37.00805556, lat2: 174.7916667 },
{ code: "NZAW", lat1: 36.83333333, lat2: 174.7666667 },
{ code: "NZJL", lat1: 36.85916667, lat2: 174.7688889 },
{ code: "NZAV", lat1: 41.18666667, lat2: 174.9438889 },
{ code: "NZBA", lat1: 46.24333333, lat2: 169.75 },
{ code: "NZJI", lat1: 35.38694444, lat2: 174.0694444 },
{ code: "NZBW", lat1: 43.47972222, lat2: 172.6869444 },
{ code: "NZCG", lat1: 38.66527778, lat2: 176.1347222 },
{ code: "NZCB", lat1: 46.04, lat2: 168.3116667 },
{ code: "NZCH", lat1: 43.48944444, lat2: 172.5344444 },
{ code: "NZJJ", lat1: 43.53694444, lat2: 172.6211111 },
{ code: "NZCL", lat1: 41.45611111, lat2: 174.0141667 },
{ code: "NZCX", lat1: 36.79166667, lat2: 175.5086111 },
{ code: "NZCW", lat1: 44.98, lat2: 169.2183333 },
{ code: "NZCS", lat1: 45.04861111, lat2: 169.1705556 },
{ code: "NZDV", lat1: 40.22833333, lat2: 176.0786111 },
{ code: "NZDA", lat1: 35.93972222, lat2: 173.8936111 },
{ code: "NZJE", lat1: 35.92888889, lat2: 173.8755556 },
{ code: "NZDY", lat1: 37.09638889, lat2: 174.9752778 },
{ code: "NZDN", lat1: 45.92805556, lat2: 170.1983333 },
{ code: "NZDC", lat1: 45.88333333, lat2: 170.5083333 },
{ code: "NZDH", lat1: 45.86888889, lat2: 170.5097222 },
{ code: "NZEV", lat1: 41.33972222, lat2: 173.0775 },
{ code: "NZFL", lat1: 40.25583333, lat2: 175.6058333 },
  { code: "NZFG", lat1: 46.895, lat2: 168.1116667 },
  { code: "NZFE", lat1: 43.3175, lat2: 172.5116667 },
  { code: "NZFT", lat1: 41.24305556, lat2: 175.9602778 },
  { code: "NZFF", lat1: 43.38583333, lat2: 172.3605556 },
  { code: "NZFH", lat1: 43.46305556, lat2: 169.9997222 },
  { code: "NZFO", lat1: 43.46194444, lat2: 170.0188889 },
  { code: "NZFR", lat1: 43.46861111, lat2: 170.0019444 },
  { code: "NZFP", lat1: 40.45666667, lat2: 175.2702778 },
  { code: "NZFJ", lat1: 43.36305556, lat2: 170.1344444 },
  { code: "NZGA", lat1: 38.40861111, lat2: 176.7419444 },
  { code: "NZGS", lat1: 38.66333333, lat2: 177.9783333 },
  { code: "NZJG", lat1: 38.63861111, lat2: 178.0036111 },
  { code: "NZGH", lat1: 43.38722222, lat2: 170.18 },
  { code: "NZGY", lat1: 44.87166667, lat2: 168.3975 },
  { code: "NZGT", lat1: 43.90777778, lat2: 170.1291667 },
  { code: "NZGC", lat1: 46.15666667, lat2: 168.8983333 },
  { code: "NZGO", lat1: 46.10277778, lat2: 168.9386111 },
  { code: "NZGB", lat1: 36.24138889, lat2: 175.4719444 },
  { code: "NZGM", lat1: 42.46166667, lat2: 171.19 },
  { code: "NZHT", lat1: 43.86666667, lat2: 169.0402778 },
  { code: "NZHN", lat1: 37.86638889, lat2: 175.3352778 },
  { code: "NZHM", lat1: 42.56972222, lat2: 172.7980556 },
  { code: "NZHS", lat1: 39.64666667, lat2: 176.7669444 },
  { code: "NZJH", lat1: 39.63, lat2: 176.8238889 },
  { code: "NZHA", lat1: 39.55333333, lat2: 174.2669444 },
  { code: "NZHK", lat1: 42.71361111, lat2: 170.9852778 },
    { code: "NZHF", lat1: 38.64333333, lat2: 176.0883333 },
    { code: "NZNV", lat1: 46.415, lat2: 168.32 },
    { code: "NZKO", lat1: 35.45111111, lat2: 173.8172222 },
    { code: "NZKI", lat1: 42.425, lat2: 173.6052778 },
    { code: "NZKJ", lat1: 42.395, lat2: 173.6808333 },
    { code: "NZKC", lat1: 42.40444444, lat2: 173.6808333 },
    { code: "NZKF", lat1: 36.40638889, lat2: 174.5872222 },
    { code: "NZKT", lat1: 35.07, lat2: 173.2852778 },
    { code: "NZJK", lat1: 35.11833333, lat2: 173.2608333 },
    { code: "NZKM", lat1: 41.23666667, lat2: 172.105 },
    { code: "NZWE", lat1: 36.82972222, lat2: 175.0655556 },
    { code: "NZKH", lat1: 41.145, lat2: 174.8352778 },
    { code: "NZKN", lat1: 35.70472222, lat2: 174.3127778 },
    { code: "NZKK", lat1: 35.26277778, lat2: 173.9119444 },
    { code: "NZKP", lat1: 40.55944444, lat2: 175.3330556 },
    { code: "NZKY", lat1: 39.84527778, lat2: 176.4213889 },
    { code: "NZHP", lat1: 42.60111111, lat2: 171.6991667 },
    { code: "NZLE", lat1: 41.75916667, lat2: 172.7458333 },
    { code: "NZLA", lat1: 43.23361111, lat2: 172.4941667 },
    { code: "NZLM", lat1: 45.74111111, lat2: 168.4425 },
    { code: "NZMW", lat1: 44.23166667, lat2: 169.2302778 },
    { code: "NZOG", lat1: 44.23305556, lat2: 169.23 },
    { code: "NZVL", lat1: 45.99027778, lat2: 168.8122222 },
    { code: "NZSO", lat1: 41.00888889, lat2: 174.0888889 },
    { code: "NZMJ", lat1: 44.36361111, lat2: 168.0191667 },
    { code: "NZMS", lat1: 40.97333333, lat2: 175.6336111 },
    { code: "NZMA", lat1: 37.73444444, lat2: 175.7419444 },
    { code: "NZMB", lat1: 36.84666667, lat2: 174.7886111 },
    { code: "NZME", lat1: 37.25916667, lat2: 175.1147222 },
    { code: "NZML", lat1: 43.35361111, lat2: 170.1908333 },
    { code: "NZMF", lat1: 44.67333333, lat2: 167.9233333 },
    { code: "NZKD", lat1: 36.17805556, lat2: 175.3244444 },
    { code: "NZMK", lat1: 41.12333333, lat2: 172.9886111 },
    { code: "NZMC", lat1: 43.765, lat2: 170.1333333 },
    { code: "NZMR", lat1: 41.79666667, lat2: 172.315 },
    { code: "NZUR", lat1: 41.80638889, lat2: 172.3286111 },
    { code: "NZNR", lat1: 39.46583333, lat2: 176.87 },
    { code: "NZNS", lat1: 41.29833333, lat2: 173.2211111 },
    { code: "NZNH", lat1: 41.28833333, lat2: 173.2722222 },
    { code: "NZNP", lat1: 39.00861111, lat2: 174.1791667 },
    { code: "NZNF", lat1: 39.20444444, lat2: 174.2233333 },
    { code: "NZNE", lat1: 36.65666667, lat2: 174.6552778 },
    { code: "NZJN", lat1: 36.78166667, lat2: 174.7586111 },
    { code: "NZOU", lat1: 44.97, lat2: 171.0816667 },
    { code: "NZOR", lat1: 45.09944444, lat2: 170.9675 },
    { code: "NZON", lat1: 46.90055556, lat2: 168.1244444 },
    { code: "NZOB", lat1: 46.58972222, lat2: 168.3055556 },
    { code: "NZOH", lat1: 40.20611111, lat2: 175.3877778 },
    { code: "NZOX", lat1: 36.14638889, lat2: 175.4186111 },
    { code: "NZOF", lat1: 36.34611111, lat2: 174.7602778 },
    { code: "NZOM", lat1: 41.54, lat2: 173.9219444 },
    { code: "NZOA", lat1: 44.48666667, lat2: 169.9861111 },
{ code: "NZOP", lat1: 38.0225, lat2: 177.3072222 },
{ code: "NZOT", lat1: 40.78361111, lat2: 175.1511111 },
{ code: "NZOS", lat1: 35.22277778, lat2: 174.23 },
{ code: "NZPS", lat1: 35.28194444, lat2: 174.0930556 },
{ code: "NZPM", lat1: 40.32055556, lat2: 175.6169444 },
{ code: "NZJM", lat1: 40.33777778, lat2: 175.6194444 },
{ code: "NZPW", lat1: 41.10416667, lat2: 175.5 },
{ code: "NZPI", lat1: 36.65166667, lat2: 174.4333333 },
{ code: "NZPP", lat1: 40.90472222, lat2: 174.9891667 },
{ code: "NZUN", lat1: 37.02166667, lat2: 175.8636111 },
{ code: "NZPN", lat1: 41.34833333, lat2: 173.9552778 },
{ code: "NZPK", lat1: 36.93027778, lat2: 174.8130556 },
{ code: "NZPO", lat1: 40.28083333, lat2: 176.6525 },
{ code: "NZPH", lat1: 43.58722222, lat2: 171.5277778 },
{ code: "NZUK", lat1: 44.235, lat2: 170.1183333 },
{ code: "NZPU", lat1: 37.25944444, lat2: 174.9075 },
{ code: "NZQW", lat1: 41.28583333, lat2: 174.78 },
{ code: "NZQN", lat1: 45.02111111, lat2: 168.7391667 },
{ code: "NZRA", lat1: 37.80472222, lat2: 174.86 },
{ code: "NZRN", lat1: 45.12972222, lat2: 170.1105556 },
{ code: "NZRT", lat1: 43.29, lat2: 172.5416667 },
{ code: "NZRK", lat1: 38.88666667, lat2: 176.3636111 },
{ code: "NZRI", lat1: 44.085, lat2: 171.4158333 },
{ code: "NZRO", lat1: 38.10916667, lat2: 176.3172222 },
{ code: "NZJO", lat1: 38.13194444, lat2: 176.2466667 },
{ code: "NZLF", lat1: 38.12944444, lat2: 176.2527778 },
{ code: "NZRL", lat1: 38.08333333, lat2: 176.2669444 },
{ code: "NZRX", lat1: 45.51166667, lat2: 169.3166667 },
{ code: "NZRR", lat1: 37.88388889, lat2: 178.29 },
{ code: "NZRW", lat1: 36.09583333, lat2: 173.9752778 },
{ code: "NZRC", lat1: 46.89972222, lat2: 168.1019444 },
{ code: "NZJS", lat1: 46.43722222, lat2: 168.3594444 },
{ code: "NZSF", lat1: 43.38361111, lat2: 171.9111111 },
{ code: "NZSL", lat1: 36.325, lat2: 174.5555556 },
{ code: "NZSD", lat1: 39.31888889, lat2: 174.3102778 },
{ code: "NZAH", lat1: 38.17083333, lat2: 174.7044444 },
{ code: "NZTI", lat1: 45.86, lat2: 170.3583333 },
{ code: "NZTK", lat1: 40.81333333, lat2: 172.7761111 },
{ code: "NZTC", lat1: 45.93805556, lat2: 169.2633333 },
{ code: "NZJQ", lat1: 39.07333333, lat2: 174.0552778 },
{ code: "NZTS", lat1: 41.20444444, lat2: 173.0494444 },
{ code: "NZTM", lat1: 38.84333333, lat2: 175.2552778 },
{ code: "NZJT", lat1: 38.88972222, lat2: 175.2513889 },
{ code: "NZAP", lat1: 38.73972222, lat2: 176.0844444 },
{ code: "NZJZ", lat1: 38.69861111, lat2: 176.0988889 },
{ code: "NZLT", lat1: 38.7317, lat2: 176.035 },
{ code: "NZTG", lat1: 37.67194444, lat2: 176.1961111 },
{ code: "NZJA", lat1: 37.70694444, lat2: 176.1480556 },
{ code: "NZMO", lat1: 45.53305556, lat2: 167.65 },
{ code: "NZTR", lat1: 37.62916667, lat2: 178.3475 },
{ code: "NZTE", lat1: 37.745, lat2: 175.1586111 },
{ code: "NZTT", lat1: 38.30333333, lat2: 175.1469444 },
{ code: "NZTQ", lat1: 38.33388889, lat2: 175.1519444 },
{ code: "NZJP", lat1: 38.05472222, lat2: 178.3044444 },
{ code: "NZTL", lat1: 44.005, lat2: 170.4416667 },
  { code: "NZTP", lat1: 44.01277778, lat2: 170.4066667 },
  { code: "NZTH", lat1: 37.15666667, lat2: 175.5502778 },
  { code: "NZTU", lat1: 44.30277778, lat2: 171.2252778 },
  { code: "NZTZ", lat1: 44.40916667, lat2: 171.2555556 },
  { code: "NZTO", lat1: 38.23666667, lat2: 175.8927778 },
  { code: "NZJX", lat1: 38.23194444, lat2: 175.8608333 },
  { code: "NZTN", lat1: 38.96833333, lat2: 175.8136111 },
  { code: "NZTW", lat1: 44.26111111, lat2: 170.0977778 },
  { code: "NZKE", lat1: 36.80833333, lat2: 175.0852778 },
  { code: "NZWV", lat1: 37.43, lat2: 175.9519444 },
  { code: "NZHH", lat1: 37.80611111, lat2: 175.2808333 },
  { code: "NZWM", lat1: 44.79, lat2: 171.0916667 },
  { code: "NZYP", lat1: 39.99666667, lat2: 176.5369444 },
  { code: "NZMH", lat1: 40.9475, lat2: 175.6752778 },
  { code: "NZJB", lat1: 41.53666667, lat2: 173.9436111 },
  { code: "NZWO", lat1: 39.01527778, lat2: 177.4041667 },
  { code: "NZJY", lat1: 39.0425, lat2: 177.4141667 },
  { code: "NZWQ", lat1: 34.52694444, lat2: 172.8383333 },
  { code: "NZWF", lat1: 44.72222222, lat2: 169.2455556 },
  { code: "NZHC", lat1: 44.70944444, lat2: 169.1363889 },
  { code: "NZWZ", lat1: 36.39777778, lat2: 174.6586111 },
  { code: "NZWN", lat1: 41.32722222, lat2: 174.8052778 },
  { code: "NZWH", lat1: 41.30833333, lat2: 174.7794444 },
  { code: "NZWL", lat1: 43.47666667, lat2: 172.3966667 },
  { code: "NZWS", lat1: 41.73805556, lat2: 171.5808333 },
  { code: "NZWK", lat1: 37.92027778, lat2: 176.9133333 },
  { code: "NZJF", lat1: 37.96555556, lat2: 176.9766667 },
  { code: "NZWU", lat1: 39.96222222, lat2: 175.0252778 },
  { code: "NZJU", lat1: 39.94333333, lat2: 175.0391667 },
  { code: "NZWR", lat1: 35.76833333, lat2: 174.365 },
  { code: "NZJR", lat1: 35.73472222, lat2: 174.3030556 },
  { code: "NZES", lat1: 38.14388889, lat2: 175.5502778 },
  { code: "NZWP", lat1: 36.78777778, lat2: 174.6302778 },
  { code: "NZWT", lat1: 36.83166667, lat2: 175.6786111 },
  { code: "NZWB", lat1: 41.51833333, lat2: 173.8702778 },
  { code: "NZCI", lat1: 43.8125, lat2: -176.4683333 }
  ];
  const inputs = [];
  const maxRows = 24;
  for (let i = 1; i <= maxRows; i++) {
    inputs.push({
      cas: document.getElementsByClassName("cas" + i)[0],
      feet: document.getElementsByClassName("feet" + i)[0],
      tasKts: document.getElementsByClassName("tas_kts" + i)[0],
      trkT: document.getElementsByClassName("trk_t" + i)[0],
      windT: document.getElementsByClassName("wind_t" + i)[0],
      windKts: document.getElementsByClassName("wind_kts" + i)[0],
      varEW: document.getElementsByClassName("var_e_w" + i)[0],
      hdg: document.getElementsByClassName("hdg" + i)[0],
      gsKts: document.getElementsByClassName("gs_kts" + i)[0],
      distanceNM: document.getElementsByClassName("distance_nm" + i)[0],
      eet: document.getElementsByClassName("eet" + i)[0],
      legFuel: document.getElementsByClassName("leg_fuel" + i)[0],
      fuelBurn: document.getElementsByClassName("fuel_burn" + i)[0],
      fuelRemain: document.getElementsByClassName("fuel_remain" + i)[0],
      fuelOnBoard: document.getElementsByClassName("fuel_on_board" + i)[0],
      from: document.getElementsByClassName("from" + i)[0],
      to: document.getElementsByClassName("to" + i)[0],
    });
    if (inputs[i - 1].from && inputs[i - 1].to) {
      inputs[i - 1].from.addEventListener("input", calculateDistance);
      inputs[i - 1].to.addEventListener("input", calculateDistance);
    }
    if (inputs[i - 1].cas) {
      inputs[i - 1].cas.addEventListener("input", calculateTasKts);
      inputs[i - 1].cas.addEventListener("input", updateGSandHDG);
      inputs[i - 1].feet.addEventListener("input", calculateTasKts);
      inputs[i - 1].trkT.addEventListener("input", calculateHdg);
      calculateHdg();
      calculateGsKts();
    }

    if (inputs[i - 1].windT) {
      inputs[i - 1].windT.addEventListener("input", calculateHdg);
      inputs[i - 1].windKts.addEventListener("input", calculateHdg);
      inputs[i - 1].varEW.addEventListener("input", calculateHdg);
    }
    if (inputs[i - 1].distanceNM) {
      inputs[i - 1].distanceNM.addEventListener("input", calculateEet);
    }
    if (inputs[i - 1].eet) {
      inputs[i - 1].eet.addEventListener("input", calculateLegFuel);
    }
    if (inputs[i - 1].fuelBurn) {
      inputs[i - 1].fuelBurn.addEventListener("input", calculateLegFuel);
    }

    if (inputs[i - 1].windT) {
      inputs[i - 1].windT.addEventListener("input", calculateGsKts);
      inputs[i - 1].tasKts.addEventListener("input", calculateGsKts);
      inputs[i - 1].trkT.addEventListener("input", calculateGsKts);
      inputs[i - 1].windKts.addEventListener("input", calculateGsKts);
    }

    if (inputs[i - 1].fuelOnBoard) {
      inputs[i - 1].fuelOnBoard.addEventListener("input", calculateLegFuel);
    }
  }
  function calculateDistance() {
    const index = inputs.findIndex(input => input.from === this || input.to === this);
    const fromCode = inputs[index].from.value.toUpperCase();
    const toCode = inputs[index].to.value.toUpperCase();
    const fromAirport = airports.find(airport => airport.code === fromCode);
    const toAirport = airports.find(airport => airport.code === toCode);


    if (fromAirport && toAirport) {
      const distanceNM = calculateLatLongDistance(fromAirport.lat1, fromAirport.lat2, toAirport.lat1, toAirport.lat2);
      inputs[index].distanceNM.value = distanceNM.toFixed(0);
    } else {
      inputs[index].distanceNM.value = "";
    }
    calculateEet(); // add this line
  }
  

  function calculateLatLongDistance(lat1, lon1, lat2, lon2) {
    const earthRadiusNM = 3440.07;
    const lat1Radians = lat1 * Math.PI / 180;
    const lon1Radians = lon1 * Math.PI / 180;
    const lat2Radians = lat2 * Math.PI / 180;
    const lon2Radians = lon2 * Math.PI / 180;
    const dlon = lon2Radians - lon1Radians;
    const dlat = lat2Radians - lat1Radians;
    const a = Math.pow(Math.sin(dlat / 2), 2) + Math.cos(lat1Radians) * Math.cos(lat2Radians) * Math.pow(Math.sin(dlon / 2), 2);
    const c = 2 * Math.atan2(Math.sqrt(a), Math.sqrt(1 - a));
    const distance = earthRadiusNM * c;
    return distance;
  }
  function calculateTasKts() {
    const index = inputs.findIndex(input => input.cas === this || input.feet === this);
    const cas = parseFloat(inputs[index].cas.value);
    const feet = parseFloat(inputs[index].feet.value);
    if (!isNaN(cas) && !isNaN(feet)) {
      const tasKts = cas + (cas * ((feet / 1000) * 0.02));
      inputs[index].tasKts.value = tasKts.toFixed(1);
      calculateHdg(); // calculate hdg
      calculateGsKts();
    } else {
      inputs[index].tasKts.value = "";
    }
    const someInputsFilled = inputs.some(input =>
      input.trkT && input.windT && input.windKts && input.varEW &&
      input.trkT.value.trim() !== "" && input.windT.value.trim() !== "" &&
      input.windKts.value.trim() !== "" && input.varEW.value.trim() !== ""
    );
    if (someInputsFilled) {
      calculateHdg();
    }
  }

  function calculateHdg() {
    const index = inputs.findIndex(input =>
      (input.cas === this) ||
      (input.feet === this) || // add feet input here
      (input.trkT === this) ||
      (input.windT === this) ||
      (input.windKts === this) ||
      (input.varEW === this)
    );
    if (index === -1) {
      return;
    }
    const casInput = parseFloat(inputs[index]?.cas?.value);
    const feetInput = parseFloat(inputs[index]?.feet?.value);
    const tasKtsInput = Math.round(inputs[index].tasKts.value);
    const trkTInput = parseFloat(inputs[index]?.trkT?.value);
    const windTInput = parseFloat(inputs[index]?.windT?.value);
    const windKtsInput = parseFloat(inputs[index]?.windKts?.value);
    const varEWValInput = parseFloat(inputs[index]?.varEW?.value);
    if (!isNaN(casInput) && !isNaN(feetInput) && !isNaN(tasKtsInput) && !isNaN(trkTInput) && !isNaN(windTInput) && !isNaN(varEWValInput)) {
      const windAngle = (windKtsInput !== 0) ? Math.atan((windKtsInput * Math.sin((windTInput - trkTInput) * Math.PI / 180)) / tasKtsInput) : 0;
      const windAngleDeg = windAngle * 180 / Math.PI;
      const HDG = trkTInput + varEWValInput + windAngleDeg;
      console.log(HDG);
      if (HDG < 0) {
        let newHDG = 360 + HDG;
        inputs[index].hdg.value = newHDG.toFixed(0).padStart(3, '0');
      } else if (HDG > 360) {
        newHDG = HDG - 360;
        inputs[index].hdg.value = newHDG.toFixed(0).padStart(3, '0');
      } else {
        inputs[index].hdg.value = HDG.toFixed(0).padStart(3, '0');
      }
      calculateGsKts();
      calculateEet();

      if (inputs[index].cas) {
        inputs[index].cas.addEventListener("input", calculateHdg);
      }
      if (inputs[index].feet) {
        inputs[index].feet.addEventListener("input", calculateHdg);
      }
    } else {
      inputs[index].hdg.value = "";
    }
  }

  function updateGSandHDG() {
    calculateGsKts();
    calculateHdg();
  }

  function calculateGsKts() {
    const index = inputs.findIndex(input =>
      (input.cas === this) ||
      (input.feet === this) || // add feet input here
      (input.trkT === this) ||
      (input.windT === this) ||
      (input.windKts === this) ||
      (input.tasKts === this)
    );
    if (index === -1) {
      return;
    }
    const tasKtsInput = Math.round(inputs[index].tasKts.value);
    const trkTInput = parseFloat(inputs[index]?.trkT?.value);
    const windTInput = parseFloat(inputs[index]?.windT?.value);
    const windKtsInput = parseFloat(inputs[index]?.windKts?.value);
    const feetInput = parseFloat(inputs[index]?.feet?.value);
    if (!isNaN(tasKtsInput) && !isNaN(trkTInput) && !isNaN(windTInput) && !isNaN(windKtsInput) && !isNaN(feetInput)) {
      const radians = Math.PI / 180;
      const term1 = tasKtsInput * Math.sqrt(1 - Math.pow((windKtsInput / tasKtsInput) * Math.sin((windTInput - trkTInput) * radians), 2));
      const term2 = windKtsInput * Math.cos((windTInput - trkTInput) * radians);
      inputs[index].gsKts.value = Math.round(term1 - term2);
    } else {
      inputs[index].gsKts.value = "";
    }
    calculateEet();
    if (inputs[index].cas) {
      inputs[index].cas.addEventListener("input", calculateGsKts);
    }
    if (inputs[index].feet) { // add event listener for feet input here
      inputs[index].feet.addEventListener("input", calculateGsKts);
    }
    if (inputs[index].windT) {
      inputs[index].windT.addEventListener("input", calculateGsKts);
    }
    if (inputs[index].windKts) {
      inputs[index].windKts.addEventListener("input", calculateGsKts);
    }
    if (inputs[index].tasKts) {
      inputs[index].tasKts.addEventListener("input", calculateGsKts);
    }
    if (inputs[index].trkT) {
      inputs[index].trkT.addEventListener("input", calculateGsKts);
    }
  }

  function calculateEet() {
    for (let i = 0; i < inputs.length; i++) {
      const gsKtsInput = parseFloat(inputs[i]?.gsKts?.value);
      const distanceNMInput = parseFloat(inputs[i]?.distanceNM?.value);
      if (!isNaN(gsKtsInput) && !isNaN(distanceNMInput) && gsKtsInput !== 0 && inputs[i]?.eet) {
        const eet = distanceNMInput / gsKtsInput * 60;
        inputs[i].eet.value = eet.toFixed(0);
      } else {
        if (inputs[i]?.eet) {
          inputs[i].eet.value = "";
        }
      }
    }
    calculateLegFuel();
  }

  function calculateLegFuel() {
    for (let i = 0; i < inputs.length; i++) {
      const eet = parseFloat(inputs[i]?.eet?.value);
      const fuelBurn = parseFloat(inputs[i]?.fuelBurn?.value);
      const fuelOnBoard = parseFloat(inputs[i]?.fuelOnBoard?.value);
      if (!isNaN(eet) && !isNaN(fuelBurn) && eet !== 0) {
        const legFuel = eet / 60 * fuelBurn;
        if (inputs[i].legFuel) {
          inputs[i].legFuel.value = legFuel.toFixed(1);
          if (!isNaN(fuelOnBoard)) {
            const fuelRemain = fuelOnBoard - legFuel;
            inputs[i].fuelRemain.value = fuelRemain.toFixed(1);
          }
        }
      } else {
        if (inputs[i].legFuel) {
          inputs[i].legFuel.value = "";
          inputs[i].fuelRemain.value = "";
        }
      }
    }
  }

  
});


const inputs = document.querySelectorAll('.from1, .from2, .from3,.from4, .from5, .from6,.from7, .from8, .from9,.from10, .from11, .from12,.from13, .from14, .from15,.from16, .from17, .from18, .to1, .to2, .to3,.to4, .to5, .to6,.to7, .to8, .to9,.to10, .to11, .to12,.to13, .to14, .to15,.to16, .to17, .to18');

inputs.forEach(input => {
  input.addEventListener('input', function (event) {
    const value = event.target.value;
    const onlyLetters = /^[a-zA-Z]*$/;
    if (!onlyLetters.test(value)) {
      event.target.value = value.replace(/[^a-zA-Z]/g, '');
    }
    if (value.length > 5) {
      event.target.value = value.slice(0, 5);
    }
  });
});

const sartimeInput = document.getElementById("sartime");

sartimeInput.addEventListener("keypress", function (event) {
  const charCode = event.which || event.keyCode;
  if (charCode >= 48 && charCode <= 57 || charCode === 58 || charCode === 46 || charCode === 44) {
    // Allow the character to be typed
    return true;
  }
  event.preventDefault();
  return false;
});
</script>

</body>
