const express = require("express");
const mongoose = require("mongoose");
const cors = require("cors");

const app = express();

app.use(cors());
app.use(express.json());

mongoose.connect(process.env.MONGO_URL);

app.get("/api", (req, res) => {
  res.json({ message: "Hello from server" });
});

app.listen(5000, () => {
  console.log("Server running on port 5000");
});
