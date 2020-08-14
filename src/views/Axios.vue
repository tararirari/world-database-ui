<template>
  <div>
    <button @click="sendGet">get</button>
    <button @click="sendPost">post</button>
    <button @click="sendPut">put</button>
    <button @click="sendDelete">delete</button>
  </div>
</template>

<script>
import axios from "axios";
export default {
  name: "Axios",
  methods: {
    sendGet() {
      axios.get("https://c3b51ce956a9e8e4324d1115bf425ef3.m.pipedream.net");
    },
    sendPost() {
      axios.post("https://c3b51ce956a9e8e4324d1115bf425ef3.m.pipedream.net", {
        traQID: "pure_white_404",
        grade: 20
      });
    },
    sendPut() {
      axios.put("https://c3b51ce956a9e8e4324d1115bf425ef3.m.pipedream.net", {
        testData: { string: "string", number: 1 }
      });
    },
    sendDelete() {
      axios.delete("https://c3b51ce956a9e8e4324d1115bf425ef3.m.pipedream.net", {
        data: { po: 1 }
      });
    }
  }
};
</script>
