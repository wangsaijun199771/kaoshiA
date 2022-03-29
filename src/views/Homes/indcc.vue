<template>
  <div class="homeIndex">
    <div class="gk">
      <p>概况</p>
      <ul>
        <li><img src="@/assets/a1.png" alt="" /></li>
        <li><img src="@/assets/a2.png" alt="" /></li>
        <li><img src="@/assets/a3.png" alt="" /></li>
        <li><img src="@/assets/a4.png" alt="" /></li>
      </ul>
    </div>

    <div class="bt">
      <p>Element ui组件</p>
    </div>

    <el-form :inline="true" :model="formInline" class="demo-form-inline">
      <div class="f1">
        <el-form-item>
          <el-select v-model="formInline.region" placeholder="活动区域">
            <el-option label="区域一" value="shanghai"></el-option>
            <el-option label="区域二" value="beijing"></el-option>
          </el-select>
        </el-form-item>

        <div class="demo-input-suffix">
          <el-input placeholder="请选择日期" suffix-icon="el-icon-date">
          </el-input>
        </div>

        <template>
          <el-input-number v-model="num" @change="handleChange" :min="1" :max="10" label="描述文字"></el-input-number>
        </template>

        </div>
      </el-form>
  </div>
</template>
      </div>
    </el-form>
  </div>
</template>