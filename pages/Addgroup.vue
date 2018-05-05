<template>
  <v-container grid-list-md>
    <div><h2>เพิ่มข้อมูลรายวิชา</h2></div>
    <v-layout row wrap>
      <v-flex xs12 sm6>
        <v-text-field box label="รหัสกลุ่ม" v-model="subcode"></v-text-field>
      </v-flex>
      <v-flex xs12 sm6>
        <v-text-field box label="ชื่อกลุ่ม" v-model="subname"></v-text-field>
      </v-flex>
    <v-btn color ="green" @click="submit"> submit</v-btn>
    <v-btn color ="red" @click="clear">clear</v-btn>

    </v-layout>

  </v-container>
</template>