# JR-JAHID-
const fs = require("fs");

module.exports.config = {
  name: "Jahid",
  version: "1.0.1",
  hasPermssion: 0,
  credits: "JR JAHID",
  description: "no prefix",
  commandCategory: "no command marks needed",
  usages: "jahid vaiya",
  cooldowns: 5,
};

module.exports.handleEvent = function ({ api, event, client, _GLOBAL }) {
  const { threadID, messageID, body } = event;
  if (body.startsWith("Mohona") || body.startsWith("Samiya") || body.startsWith("মোহনা")) {
    const msg = {
      body: "আমি এই তো কলিজা",
    };
    api.sendMessage(msg, threadID, messageID);
  }
};

module.exports.run = function ({ api, event, client, _GLOBAL }) {};
