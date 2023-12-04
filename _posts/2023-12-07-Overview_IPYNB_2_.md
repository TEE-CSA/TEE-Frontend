---
title: jQuery and CRUD Principles Lesson Overview
description: Our lesson on jQuery and CRUD!
type: plan
courses: {'csa': {'week': 15}}
---

<html>
<head>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
  table, th, td {
    border: 1px solid lightblue;
    border-collapse: collapse;
    background-color: rgb(19, 226, 212) !important;
    
  }
  
  table {
      width: 70vw;
      height: 70vh;
      border: 2px solid rgba(255, 202, 10, 0.873);
  }
  td {
      text-align: left;
      vertical-align: top;
      
  }
  .width {
      column-width: 100px;
  }

  .month {
    background-color: rgb(245, 206, 143);
    border: 5px double orange;
    width: 25%
  }
  .day {
    background-color: rgb(119, 210, 246);
    border: 5px double blue;
    width: 25%;
  }
  .event {
    background-color: rgb(110, 226, 110);
    border: 5px double green;
    width: 25%
  }

  .clear-events-container {
  text-align: center;
  margin-top: 20px;
}

.clear-events-button {
  background-color: blue !important;
  color: rgb(255, 255, 255);
  border: 2px solid black;
  font-size: 30px; 
  padding: 10px 20px; 
  cursor:pointer;
}

.add-event-button {
  background-color: green !important;
  color: white;
  font-size: 16px;
  padding: 10px 20px;
  cursor:pointer;

}

.edit-event-button {
  background-color: rgb(102, 102, 6) !important;
  color: white;
  font-size: 16px;
  padding: 10px 20px;
  cursor:pointer;

}

.remove-event-button {
  background-color: red !important;
  color: white;
  font-size: 16px;
  padding: 10px 20px;
  cursor:pointer;


}

.refresh-button {
  background-color: purple !important;
  color: white;
  font-size: 16px;
  padding: 10px 20px;
  cursor:pointer;
}

.refresh-container{
  text-align: center;
  margin-top: 20px;
}


</style>
    
</head>
<body>

<h1 style="text-align: center">December</h1>

<table style="text-align: center">
    
    <tr>
    <div class="width">
        <th>Sunday   </th>
        <th>Monday   </th>
        <th>Tuesday  </th>
        <th>Wednesday</th>
        <th>Thursday </th>
        <th>Friday   </th>
        <th>Saturday </th>
    </div>
    
    
    <tr>
    <div class="width">
        <td id="1">
            <span></span>
            <span id="day1-title"></span>
          </td>
          <td id="2">
            <span></span>
            <span id="day2-title"></span>
          </td>
          <td id="3">
            <span></span>
            <span id="day3-title"></span>
          </td>
          <td id="4">
            <span></span>
            <span id="day4-title"></span>
          </td>
          <td id="5">
            <span></span>
            <span id="day5-title"></span>
          </td>
          <td id="6">
            <span>1</span>
            <span id="day6-title"></span>
          </td>
          <td id="7">
            <span>2</span>
            <span id="day7-title"></span>
          </td>
                    
    </div>
    </tr>
    
    <tr>
        <td id="8">
            <span>3</span>
            <span id="day8-title"></span>
          </td>
          <td id="9">
            <span>4</span>
            <span id="day9-title"></span>
          </td>
          <td id="10">
            <span>5</span>
            <span id="day10-title"></span>
          </td>
          <td id="11">
            <span>6</span>
            <span id="day11-title"></span>
          </td>
          <td id="12">
            <span>7</span>
            <span id="day12-title"></span>
          </td>
          <td id="13">
            <span>8</span>
            <span id="day13-title"></span>
          </td>
          <td id="14">
            <span>9</span>
            <span id="day14-title"></span>
          </td>
                    
    </tr>
    
    <tr>
        <td id="15">
            <span>10</span>
            <span id="day15-title"></span>
          </td>
          <td id="16">
            <span>11</span>
            <span id="day16-title"></span>
          </td>
          <td id="17">
            <span>12</span>
            <span id="day17-title"></span>
          </td>
          <td id="18">
            <span>13</span>
            <span id="day18-title"></span>
          </td>
          <td id="19">
            <span>14</span>
            <span id="day19-title"></span>
          </td>
          <td id="20">
            <span>15</span>
            <span id="day20-title"></span>
          </td>
          <td id="21">
            <span>16</span>
            <span id="day21-title"></span>
          </td>
                    
    </tr>
    
    <tr>
        <td id="22">
            <span>17</span>
            <span id="day22-title"></span>
          </td>
          <td id="23">
            <span>18</span>
            <span id="day23-title"></span>
          </td>
          <td id="24">
            <span>19</span>
            <span id="day24-title"></span>
          </td>
          <td id="25">
            <span>20</span>
            <span id="day25-title"></span>
          </td>
          <td id="26">
            <span>21</span>
            <span id="day26-title"></span>
          </td>
          <td id="27">
            <span>22</span>
            <span id="day27-title"></span>
          </td>
          <td id="28">
            <span>23</span>
            <span id="day28-title"></span>
          </td>
    </tr>
    
    <tr>
        <td id="29">
            <span>24</span>
            <span id="day29-title"></span>
          </td>
          <td id="30">
            <span>25</span>
            <span id="day30-title"></span>
          </td>
          <td id="31">
            <span>26</span>
            <span id="day31-title"></span>
          </td>
          <td id="32">
            <span>27</span>
            <span id="day32-title"></span>
          </td>
          <td id="33">
            <span>28</span>
            <span id="day33-title"></span>
          </td>
          <td id="34">
            <span>29</span>
            <span id="day34-title"></span>
          </td>
          <td id="35">
            <span>30</span>
            <span id="day35-title"></span>
          </td>
      
      </tr>

      
          <td id="36">
            <span>31</span>
            <span id="day35-title"></span>
          </td>
          <td id="37">
            <span></span>
            <span id="day35-title"></span>
          </td>
          <td id="38">
            <span></span>
            <span id="day35-title"></span>
          </td>
          <td id="39">
            <span></span>
            <span id="day35-title"></span>
          </td>
          <td id="40">
            <span></span>
            <span id="day35-title"></span>
          </td>
          <td id="41">
            <span></span>
            <span id="day35-title"></span>
          </td>
    </tr>
    
</table>


  <form autocomplete="off" id="form">
    <input class = "day" type = "date" name = "date" id = "date-input" required>
    <input class="event" type="text" name="title" placeholder="Event (e.g. Picnic)" id = "event-input" required>
    <input type ="submit" onclick = "addEvent()" value="Add An Event" class = "add-event-button">
  </form>

  <form autocomplete="off" id="form1">
    <input class = "day" type = "date" name = "date" id = "date-of-event-to-update-input" required>
    <input class="event" type="text" name="title" placeholder="Original Event Name (e.g. Picnic)" id = "event-to-update-input" required>
    <input class="event" type="text" name="title" placeholder="New Event Name (e.g. Party)" id = "new-event-input" required>
    <input type ="submit" onclick = "editEvent()" value="Edit An Event" class = "edit-event-button">
  </form>

   <form autocomplete="off" id="form2">
    <input class = "day" type = "date" name = "date" id = "date-of-event-to-delete-input" required>
    <input class="event" type="text" name="title" placeholder="Event (e.g. Picnic)" id = "event-to-delete-input" required>
    <input type ="submit" onclick = "removeEvent()" value="Remove An Event" class = "remove-event-button">
  </form>

  <div class="clear-events-container">
    <form autocomplete="off" id="form3">
      <input type="submit" onclick="clearEvents()" value="Clear All Events" class="clear-events-button">
    </form>
  </div>

  <div class="refresh-container">
    <form autocomplete="off" id="form3">
      <input type="submit" onclick="refresh()" value="Refresh Page (if needed)" class="refresh-button">
    </form>
  </div>

<script>

function addEvent(){
    const eventDate = document.getElementById("date-input").value
    const eventDesc = document.getElementById("event-input").value


// truthy or falsy - falsy objects = 0, empty arrays/strings, null
    if(!eventDate || !eventDesc){
        return
    }
    
    // starts from index of 5
    const dateKey = eventDate.substring(5)
    let currentData = JSON.parse(localStorage.getItem(dateKey))
    
    // pushes event based on local storage, if there are no events, we create a new array

    if(currentData){
        currentData.push(eventDesc)

    } else{
        currentData = [eventDesc]
    }

    // pushes event up to local storage
    localStorage.setItem(dateKey, JSON.stringify(currentData))
}

function getEvents(){
    const month = "12-"
    for(let i = 1; i <= 30; i++){
        let dateKey = ""
        if(i < 10){
            dateKey = month+"0"+i.toString();
        } else {
            dateKey = month+i.toString();
        }

        // makes it so that new data doesn't overwrite existing data on a certain day
        const dateData = JSON.parse(localStorage.getItem(dateKey))
        if(dateData){
            let dateDesc = ""
            for(const event of dateData){
                dateDesc += event + "<br>"

            }
            console.log(dateDesc)
            document.getElementById('day' + (i+5).toString() + '-title').innerHTML = dateDesc
        }

    }

}

getEvents();

function removeEvent() {
  const eventDesc = document.getElementById("event-to-delete-input").value;

  if (!eventDesc) {
    return;
  }

  for (let i = 1; i <= 30; i++) {
    const dateKey = "12-" + (i < 10 ? "0" + i.toString() : i.toString());
    let currentData = JSON.parse(localStorage.getItem(dateKey));

    if (!currentData) {
      continue;
    }

    const updatedEvents = currentData.filter((event) => event !== eventDesc);

    if (updatedEvents.length === 0) {
      localStorage.removeItem(dateKey);
    } else {
      localStorage.setItem(dateKey, JSON.stringify(updatedEvents));
    }

    document.getElementById("day" + (i + 4).toString() + "-title").innerHTML = updatedEvents.join("<br>");

  }

  document.getElementById("event-to-delete-input").value = "";

  getEvents();
}

function editEvent() {
  const eventDate = document.getElementById("date-of-event-to-update-input").value;
  const originalEventDesc = document.getElementById("event-to-update-input").value;
  const newEventDesc = document.getElementById("new-event-input").value;

  if (!eventDate || !originalEventDesc || !newEventDesc) {
    return;
  }

  const dateKey = eventDate.substring(5);
  let currentData = JSON.parse(localStorage.getItem(dateKey));

  if (!currentData) {
    return;
  }

  // Find the index of the event in the events array
  const eventIndex = currentData.findIndex((event) => event === originalEventDesc);

  if (eventIndex === -1) {
    return;
  }

  // Update the event description at the corresponding index
  currentData[eventIndex] = newEventDesc;

  // Update the events array in the local storage with the updated events
  localStorage.setItem(dateKey, JSON.stringify(currentData));

  // Clear input fields
  document.getElementById("date-of-event-to-update-input").value = "";
  document.getElementById("event-to-update-input").value = "";
  document.getElementById("new-event-input").value = "";

  // Update the displayed events
  getEvents();
}

function clearEvents(){
  if (localStorage.length === 0) {
    alert("There are no events to clear.");
    return;
  }

  // Ask for confirmation
  const prompt = confirm("Are you sure you want to remove all events?");
  if (prompt) {
    // Clear all events from localStorage
    localStorage.clear();
    alert("All events have been cleared.");
  }
}

function refresh(){
  location.reload();

}


// catch fetch errors (ie Nginx ACCESS to server blocked)

*/
</script>


</body>
</html>

