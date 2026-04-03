const express = require("express");
const app = express();

let command = "";

// 📌 Phones yahan se command lenge
app.get("/get-command", (req, res) => {
  res.send(command);
});

// 📌 Master yahan se trigger karega
app.get("/run-all", (req, res) => {
  command = "RUN";
  setTimeout(() => {
    command = "";
  }, 5000);
  res.send("Triggered");
});

app.listen(3000, () => console.log("Server running"));
