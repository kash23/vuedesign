<template>

  <div class="Header">
    <h3>REMOTE PATIENT MONITORING DASHBOARD -DEMO</h3>
  </div>
  <div class="Container">
    <div class="col1">
      <div class="col1-1">
        <h4>Average</h4>
        <div class="vertical"></div>
      </div>
      <div class="col1-2">
        <h4> Daily Average</h4>
        <div class="vertical"></div>
      </div>
    </div>
    <div class="col2">
      <div class="col2-1con">
        <div class="col2-1">
          <h4>Patient ID</h4>
          <div class="drop">
            <select class="dropdown" name="cars" id="cars">
              <optgroup>
                <option value="volvo">All</option>
                <option value="saab">Saab</option>
              </optgroup>
            </select>
          </div>
        </div>
        <div class="col2-2">
          <h4>Patient Name</h4>
          <div class="drop">
            <select class="dropdown_name" name="cars" id="cars">
              <optgroup>
                <option value="volvo">Name</option>
                <option value="saab">Saab</option>
              </optgroup>
            </select>
          </div>
        </div>
      </div>
      <div class="col2-3">
        <h4>Nutrition</h4>
      </div>
      <div class="col2-4">
        <h4>Average Health & Wellness Response</h4>
      </div>
    </div>
    <div class="col3">
      <div class="col3-1">
        <h4>Date</h4>
        <div class="date">
          <div>
            <select class="dropdown_last" name="cars" id="cars">
              <optgroup>
                <option value="volvo">Last</option>
                <option value="saab">Saab</option>
              </optgroup>
            </select>
          </div>
          <div>
            <input class="textbox" type="text" id="fname"> 
          </div>
          <div>
            <select class="dropdown_month" name="cars" id="cars">
              <optgroup>
                <option value="volvo">Month</option>
                <option value="saab">Saab</option>
              </optgroup>
            </select>
          </div>
        </div>
        <div>

        </div>
      </div>
      <div class="col3-2">
        <h4>Glucose (mg/dL)</h4>
      </div>
      <div class="col3-3">
        <h4>Blood Pressure (mmHg)</h4>
      </div>
    </div>
    <div class="col4">
      <div class="col4-1">
        <h4>Steps</h4>
      </div>
      <div class="col4-2">
        <h4>Calories Burned</h4>
      </div>
      <div class="col4-3">
        <h4>Body Weight (lb)</h4>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style scoped>
*{
  border-radius: 5px;
  margin: 0px;
  padding: 0;
  font-family: Arial, Helvetica, sans-serif;
}
.Header{
  width: 1239px;
  height: 80px;
  border: 1px solid black;
  margin-bottom: 10px;
  box-shadow: 0 1.5px 0 1.5px rgba(0, 0, 0, 0.5);
}

.Container{
  display: flex;
  column-gap: 20px;
}
.col1,
.col2,
.col3,
.col4{
  display: grid;
  row-gap: 10px;

}
.col1-1,
.col1-2{
  width: 165px;
  height: 307px;
  border: 1px solid black;
  box-shadow: 0 1.5px 0 1.5px rgba(0, 0, 0, 0.5);
}
.col2-1con{
  display: flex;
  column-gap: 10px;

}
.col2-1{
  width: 150px;
  height: 100px;
  border: 1px solid black;
  box-shadow: 0 1.5px 0 1.5px rgba(0, 0, 0, 0.5);
}
.col2-2{
  width: 260px;
  height: 100px;
  border: 1px solid black;
  box-shadow: 0 1.5px 0 1.5px rgba(0, 0, 0, 0.5);
}
.col2-3,
.col2-4{
  width: 423px;
  height: 250px;
  border: 1px solid black;
  box-shadow: 0 1.5px 0 1.5px rgba(0, 0, 0, 0.5);
}

.col3-1{
  width: 300px;
  height: 100px;
  border: 1px solid black;
  box-shadow: 0 1.5px 0 1.5px rgba(0, 0, 0, 0.5);
}
.col3-2{
  width: 300px;
  height: 250px;
  border: 1px solid black;
  box-shadow: 0 1.5px 0 1.5px rgba(0, 0, 0, 0.5);
}
.col3-3{
  width: 300px;
  height: 250px;
  border: 1px solid black;
  box-shadow: 0 1.5px 0 1.5px rgba(0, 0, 0, 0.5);
}
.col4-1,
.col4-2,
.col4-3{
  width: 285px;
  height: 200px;
  border: 1.5px solid black;
  box-shadow: 0 1.5px 0 1.5px rgba(0, 0, 0, 0.5);
}
.vertical {
  margin-left: 10px;
  margin-top: 10px;
	border-left: 3px solid rgb(0, 183, 255);
  border-radius: 1px;
	height: 250px;
}
h3{
  margin: 10px;
}
h4{
  margin: 10px;
}
.drop{
  text-align: center;
}
.dropdown{
  width: 125px;
  height: 25px;
  margin-top: 5px;
}
.dropdown_name{
  width: 240px;
  height: 25px;
  margin-top: 5px;
}
.date{
  display: flex;
  column-gap: 10px;
  justify-content: center;
  /* margin-left: 30px; */
}
.dropdown_last{
  width: 100px;
  height: 25px;
  margin-top: 5px;
}
.dropdown_month{
  width: 130px;
  height: 25px;
  margin-top: 5px;

}
.textbox{
  width: 30px;
  height: 20px;
  margin-top: 5px;
  border: 1px solid rgba(0, 0, 0, 0.596);
}
</style>
