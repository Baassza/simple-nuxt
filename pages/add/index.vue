<template >
    <div>
        <v-col>
            <div class="set_center">
                <img src="avatar.png" class="avatar" id="avatar" />
                <v-btn variant="outlined" style="margin-left: 4rem;">
                    เลือกภาพ
                </v-btn>
            </div>
            <br>
            <v-text-field clearable label="ชื่อ" variant="outlined"></v-text-field>
            <v-text-field clearable label="นามสกุล" variant="outlined"></v-text-field>
            <v-combobox label="เพศ" :items="['ชาย', 'หญิง']" variant="outlined"></v-combobox>
            <v-text-field clearable label="วันเกิด" type="date" variant="outlined"></v-text-field>
            <v-text-field clearable label="เบอร์โทร" variant="outlined"></v-text-field>
            <v-text-field clearable label="facebook" variant="outlined"></v-text-field>
            <v-combobox label="การศึกษา" :items="['ไม่ระบุ',
                'ต่ำกว่าชั้นประถมศึกษา',
                'ชั้นประถมศึกษา',
                'ชั้นมัธยมศึกษาตอนต้น',
                'ชั้นมัธยมศึกษาปลายหรือเทียบเท่า',
                'อนุปริญญาตรีหรือเทียบเท่า',
                'ปริญญาตรี',
                'สูงกว่าปริญญาตรี',]" variant="outlined">
            </v-combobox>
            <v-text-field clearable label="ที่อยู่" variant="outlined"></v-text-field>
            <br>
            <div class="set_center">
                <v-btn variant="outlined" style="margin-left: 4rem;" size="x-large">
                    บันทึก
                </v-btn>
            </div>
        </v-col>
    </div>
</template>
<script setup>
</script>
<style>
.avatar {
    border-radius: 50%;
    width: 200px;
    height: 200px;
    margin-bottom: 20px;
    margin-left: 65px;
}

.set_center {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    margin: 1rem;
    margin-top: -0.75rem;
}
</style>