<!DOCTYPE html>
<html>
<head>
<title>Skraiduolis: Survey Form</title>
</head>
<body>
<style>
	body {
    	background: url(https://skraiduolis.lt/wp-content/uploads/2020/03/16.jpg);
	background-position: center;       
}
    h1 {
    	font-family: cambria;
        text-align: center;
        color: white;
    	}
    #description {
    	font-style: italic;
    	font-family: cambria;
        font-size: 18px;
        text-align: center;
        color: white;
        }
    .container {
    	width: 50%;
  	margin: 40px auto 0px auto;
        font-family: cambria;
        font-size: 20px;
        text-align: left;
        color: white;
        padding: 60px;
        background-color: #E79034;
        border: 10px solid #DA760C;
        border-radius: 10px;
}
		label {
  display: flex;
  align-items: center;
  font-size: 18px;
  margin-bottom: 10px;
  
  }
  input,
button,
select,
textarea {
  margin: 0;
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
  border-radius: 4px;
}
        

</style>

<h1 id="title">Indoor Playground "Skraiduolis" Survey Form</h1>
<p id="description">Thank you for taking the time to help us improve our services</p>
<div class="container">
<form id="survey-form">
	<div class="form-group">
    	<label id="name-label" for="name">Name</label>
         <input
        	type="text"
        	name="name"
        	id="name"
        	class="form-control"
        	placeholder="Enter your name"
        	required
      		/>
     </div>
	<br>
    <div class="form-group">
    	<label id="email-label" for="email">Email</label>
         <input
        	type="email"
        	name="email"
        	id="email"
        	class="form-control"
        	placeholder="Enter your Email"
            required
      		/>
     </div>
      <br>
      <div class="form-group">
      <label id="number-label" for="number"
        >Number of kids<span class="clue">(optional)</span></label
      >
      <input
        type="number"
        name="number-of-kids"
        id="number"
        min="0"
        max="15"
        class="form-control"
        placeholder="Number of kids"
        pattern: "0-15"
        required
      />
    </div>
    
    <div class="form-group">
      <p>Choose the city for your birthday party</p>
      <select id="dropdown" name="city" class="form-control" required>
        <option disabled selected value>Choose the city</option>
        <option value="vilnius">Vilnius</option>
        <option value="kaunas">Kaunas</option>
        <option value="klaipeda">Klaipėda</option>
        <option value="panevezys">Panevėžys</option>
        <option value="siauliai">Šiauliai</option>
      </select>
    </div>
	   
       <div class="form-group">
      <p>Have you ever celebrated birthday at Skraiduolis?</p>
      <label>
        <input
          name="our-customer"
          value="yes"
          type="radio"
          class="input-radio"
          checked
        />Yes</label
      >
      <label>
        <input
          name="our-customer"
          value="no"
          type="radio"
          class="input-radio"
        />No</label
      >

      <label
        ><input
          name="our-customer"
          value="not-sure"
          type="radio"
          class="input-radio"
        />Not sure</label
      >
    </div>
     
     <div class="form-group">
      <p>What additional services would you be interested in using from our selection?
      <span class="clue">(Check all that apply)</span>
      </p>
      <label
        ><input
          name="additional-services"
          value="animator"
          type="checkbox"
          class="input-checkbox"
        />Animator</label
      >
      <label>
        <input
          name="additional-services"
          value="balloons"
          type="checkbox"
          class="input-checkbox"
        />Balloons</label
      >
      <label
        ><input
          name="additional-services"
          value="table-decoration"
          type="checkbox"
          class="input-checkbox"
        />Table decoration</label
      >
      <label
        ><input
          name="additional-services"
          value="catering"
          type="checkbox"
          class="input-checkbox"
        />Catering</label
      >
      <label
        ><input
          name="additional-services"
          value="photographer"
          type="checkbox"
          class="input-checkbox"
        />Photographer</label>
     </div>
     
      <div class="form-group">
      <p>Any comments or suggestions?</p>
      <textarea
        id="comments"
        class="input-textarea"
        name="comment"
        placeholder="Please enter your comments here"
      ></textarea>
    </div>
     <div class="form-group">
      <button type="submit" id="submit" class="submit-button">
      Submit
      </button>
    </div>
</form>
</div>

</body>
</html>
