<template>
  <div>
    <el-dialog title="选择"
               :visible.sync="box"
               width="50%">
      <el-radio-group v-model="text"
                      class="list">
        <el-row :span="24">
          <el-col v-for="(item,index) in list"
                  :key="index"
                  :md="4"
                  :xs="12"
                  :sm="4">
            <el-radio :label="item.value">{{item.name}}</el-radio>
          </el-col>
        </el-row>
      </el-radio-group>
    </el-dialog>

    <span>
      <i class="icon-iframe"
         @click="open"></i>
    </span>
  </div>
</template>

<script>
import { setLayout } from "@/util/util";
import { mapGetters } from "vuex";
export default {
  data() {
    return {
      box: false,
      text: "",
      list: [
        {
          name: "默认布局",
          value: "default"
        },
        {
          name: "头部栏布局",
          value: "layout-top"
        },
        {
          name: "右边栏布局",
          value: "layout-right"
        },
        {
          name: "底部栏布局",
          value: "layout-bottom"
        }
      ]
    };
  },
  watch: {
    text: function(val) {
      this.$store.commit("SET_LAYOUT_NAME", val);
      setLayout(val);
    }
  },
  computed: {
    ...mapGetters(["layoutName"])
  },
  mounted() {
    this.text = this.layoutName;
    if (!this.text) {
      this.text = "";
    }
  },
  methods: {
    open() {
      this.box = true;
    }
  }
};
</script>

<style lang="scss" scoped>
.list {
  width: 100%;
}
</style>

