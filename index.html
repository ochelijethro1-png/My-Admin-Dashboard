<!DOCTYPE html>
<html>
<head>
<title>Admin Dashboard - Jethro</title>
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
body{
  font-family: Arial;
  background:#0b1426;
  color:#fff;
  margin:0;
}

.container{
  max-width:500px;
  margin:40px auto;
  padding:20px;
}

h2{
  text-align:center;
}

input{
  width:70%;
  padding:10px;
  border:none;
  border-radius:5px;
}

button{
  padding:10px;
  border:none;
  border-radius:5px;
  cursor:pointer;
}

.add-btn{
  background:#00c853;
  color:#fff;
}

ul{
  list-style:none;
  padding:0;
  margin-top:20px;
}

li{
  background:#111a33;
  padding:10px;
  margin-bottom:10px;
  border-radius:5px;
  display:flex;
  justify-content:space-between;
  align-items:center;
}

li.active span{
  text-decoration:line-through;
  opacity:0.6;
}

.actions button{
  margin-left:5px;
}

.edit{
  background:#2196f3;
  color:#fff;
}

.delete{
  background:#ff3d00;
  color:#fff;
}

.toggle{
  background:#ffc107;
}
</style>
</head>

<body>

<div class="container">
  <h2>Admin Dashboard</h2>

  <input id="userInput" placeholder="Add user">
  <button class="add-btn" id="addBtn">Add</button>
  <h3>Total Users: <span id="count">0</span></h3>

  <ul id="userList"></ul>
</div>

<script>
const input = document.getElementById("userInput");
const addBtn = document.getElementById("addBtn");
const list = document.getElementById("userList");

// ===== STATE =====
let users = JSON.parse(localStorage.getItem("users")) || [];

// ===== SAVE TO STORAGE =====
function save(){
  localStorage.setItem("users", JSON.stringify(users));
}

// ===== RENDER FUNCTION =====
function render(){
  document.getElementById("count").innerText = users.length;
  
  list.innerHTML = users.map(user => `
    <li class="${user.active ? 'active' : ''}">
      <span>${user.name}</span>
      <div class="actions">
        <button class="toggle" onclick="toggleUser('${user.id}')">Toggle</button>
        <button class="edit" onclick="editUser('${user.id}')">Edit</button>
        <button class="delete" onclick="deleteUser('${user.id}')">Delete</button>
      </div>
    </li>
  `).join("");
}

// ===== ADD USER =====
addBtn.onclick = () => {
  const name = input.value.trim();
  if(!name) return;
  
  if(users.some(user => user.name.toLowerCase() === name.toLowerCase())){
  alert("User already exists");
  return;
}

  users.push({
    id: Date.now().toString(),
    name: name,
    active: false
  });

  input.value = "";
  save();
  render();
};

// ===== TOGGLE =====
function toggleUser(id){
  users = users.map(user =>
    user.id === id ? {...user, active: !user.active} : user
  );
  save();
  render();
}

// ===== DELETE =====
function deleteUser(id){
  if(!confirm("Delete this user?")) return;

  users = users.filter(user => user.id !== id);
  save();
  render();
}

// ===== EDIT =====
function editUser(id){
  const newName = prompt("Edit user name:");

if(!newName || !newName.trim()) return;

  users = users.map(user =>
    user.id === id ? {...user, name: newName} : user
  );

  save();
  render();
}

input.addEventListener("keypress", e => {
  if(e.key === "Enter"){
    addBtn.click();
  }
});

// ===== INITIAL LOAD =====
render();
</script>

</body>
</html>