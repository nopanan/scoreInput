<template>
  <v-container grid-list-md>
    <div><h2>แก้ไขข้อมูลครูผู้สอน</h2></div>
    <v-layout row wrap>
      <v-flex xs12 sm6>
        <v-text-field box label="รหัสประจำตัว" v-model="code" disabled=""></v-text-field>
      </v-flex>
      <v-flex xs12 sm6>
        <v-text-field box label="ชื่อ - นามสกุล" v-model="last"></v-text-field>
      </v-flex>
      <v-flex xs12>
        <v-text-field
          box
          label="เบอร์โทรศัพท์"
          :rules="phoneRules"
          v-model="phone"
          persistent-hint
        ></v-text-field>
      </v-flex>
      <v-flex xs12>
        <v-text-field
          box
          label="Email"
          :rules="emailRules"
          v-model="email"
          persistent-hint
        ></v-text-field>
      </v-flex>
      <v-flex xs12>
        <v-text-field box multi-line label="ที่อยู่"></v-text-field>
      </v-flex>
    <v-btn color ="green" @click="submit" > submit </v-btn>
    <v-btn color ="red" @click="clear">clear</v-btn>

    </v-layout>

  </v-container>
</template>