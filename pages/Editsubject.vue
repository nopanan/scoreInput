<template>
  <v-container grid-list-md>
    <div><h2>แก้ไขข้อมูลรายวิชา</h2></div>
    <v-layout row wrap>
      <v-flex xs12 sm6>
        <v-text-field box label="รหัสวิชา" v-model="subcode" disabled=""></v-text-field>
      </v-flex>
      <v-flex xs12 sm6>
        <v-text-field box label="ชื่อวิชา" v-model="subname"></v-text-field>
      </v-flex>
    <v-btn color ="green" @click="submit" > submit </v-btn>
    <v-btn color ="red" @click="clear">clear</v-btn>

    </v-layout>

  </v-container>
</template>