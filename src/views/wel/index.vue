<template>
  <div>
    <basic-container>
      <third-register></third-register>
      <p style="text-align: center;">
        欢迎您的来访!我们让您每天轻松十分钟！
      </p>
    </basic-container>
    <el-col :span="16">
      <basic-container>
        <el-collapse v-model="activeNames" @change="handleChange">
          <el-collapse-item title="上集" name="1">
            <div>1、看别人的脸色行事,并不说明你为人处事就替别人着想</div>
            <div>2、改变自己很难,改变环境更难,我该肿么办?</div>
            <div>3、脸说:你为什么不要我了?!快回答呀,我在问你话呢。</div>
            <div>4、昨夜睡觉,梦见自己家的房子被强拆了,醒来后才发现是虚惊一场,我根本买不起房子。</div>
            <div>5、什么东西看不见摸不着但很重要?普通青年:空气;文艺青年:爱情;我: WIFI……</div>
          </el-collapse-item>
          <el-collapse-item title="下集" name="2">
            <div>1、人是铁,贱是钢,一天不犯闷得慌。</div>
            <div>2、便秘有一种委婉的说法:我有一种不翔的预感。拉肚子也有一种委婉的说法:我有一种滑翔的感觉……</div>
            <div>3、比起惊喜,我更喜欢惊吓,因为前者不好意思发飙。</div>
            <div>4、女人和恐怖份子唯一的区别是,恐怖份子是可以谈判的。</div>
            <div>5、人生的三大错觉:手机震动、有人敲门、还有,他(她)喜欢你。。。</div>
          </el-collapse-item>
          <el-collapse-item title="爆逗,笑醉是种什么感受?" name="3">
            <div>1、精神分裂的好处就是遇到事情有个人商量。</div>
            <div>2、养金鱼真的挺方便的，第一天养，第二天就都死光了，饲料都不用喂。</div>
            <div>3、年纪大了最显著的特征是，八卦讲到一半，姐妹说上次已经讲过了。</div>
            <div>4、保险公司的存在并不是为了给你提供保险。他们其实是想从你不需要保险的计算风险中赚钱。</div>
            <div>5、我有一种特别厉害的能力，总能在人们丢东西前找到它们。但是警察却坚持说我这叫偷窃。</div>
            <div>6、“代沟”存在的好处就是让上一代的劣俗和毛病不会传承下去。</div>
            <div>7、用一副对联概括目前我的生活态度</div>
            <div>8、上联：具体问题具体分析;下联：以后事情以后再说;横批：顺其自然。</div>
          </el-collapse-item>
          <el-collapse-item title="爆囧,脑壳有点昏。。。" name="4">
            <div>1、闺蜜牙疼，决定把这颗病牙拔了。我陪着捂着腮帮子哼哼唧唧的闺蜜去了附近牙科小诊所。牙医大哥给闺蜜检查的时候，闺蜜痛的大声啊埃。。大哥擦擦头上的汗，对我说：你出去叫几个街坊邻居过来，你嫂子不在家，我害怕误会。</div>
            <div>2、我对我妈说，我喜欢一个很优秀的男生，但是感觉没有机会。我妈说，你怕啥，你虽然差劲，但能有机会接触到这么好的人，说明他命中注定有此一劫。</div>
            <div>3、一大早刚到公司，就看到女主管发飙，不停骂人，摔东西，后来听同事讲，女主管经人介绍相亲，媒人对她说男方家挺有实力，是做铁矿生意的。后来才知道，对方家是收废铁的！</div>
            <div>4、打扫卫生翻到老公的私房钱，不好意思给他没收了，把手上的手链褪下来，跟他私房钱放一起。跑去跟老公说手链找不到了，让他帮忙找找。没多久，老公拿着手链跟私房钱过来：“老婆，手链找到了，你看看这个钱是不是你一起掉的？”</div>
            <div>5、现在的小偷是越来越善良了，今天在饭店吃饭，付账的时候发现钱包和手机都不见了。。。跟老板说明天付，老板告诉我：刚刚有人为你付过了。。。</div>
            <div>6、“学长学姐好，我是临床医学的新生，请问解剖课的尸体是自己带还是学校发？”“自己带不怎么新鲜，学校发的质量又不好，我们一般都是现杀，有关系好的同学也可以互相解剖！ ”</div>
          </el-collapse-item>
          <el-collapse-item title="笑话定制开发" name="5">
            <div>1、接笑话系列的定制服务</div>
            <div>2、接3个月以内工期的笑话系列等定制服务</div>
            <div>3.有意向请联系唯一指定扣扣:168168168</div>
          </el-collapse-item>
        </el-collapse>
      </basic-container>
    </el-col>
    <el-col :span="8">
      <el-row>
        <basic-container>
          <div class="el-font-size">
            <span>产品名称</span>
            <el-divider direction="vertical"/>
            <span><el-tag>哈哈一笑级微服务平台</el-tag></span>
            <el-divider content-position="right"><i class="el-icon-star-off"/></el-divider>
            <span>账号密码</span>
            <el-divider direction="vertical"/>
            <el-tag effect="plain">管理员(admin)</el-tag>
            <el-divider content-position="right"><i class="el-icon-star-off"/></el-divider>
            <span>官网地址</span>
            <el-divider direction="vertical"/>
            <span><el-link href="https://www.168168168.com" target="_blank"
                           type="primary">https://www.168168168.com</el-link></span>
            <el-divider content-position="right"><i class="el-icon-star-off"/></el-divider>
            <span>社区地址</span>
            <el-divider direction="vertical"/>
            <span><el-link href="https://www.168168168.com" target="_blank"
                           type="primary">https://www.168168168.com</el-link></span>
            <el-divider content-position="right"><i class="el-icon-star-off"/></el-divider>
          </div>
        </basic-container>
      </el-row>
      <el-row>
        <basic-container>
          <el-collapse v-model="logActiveNames" @change="handleChange">
            <el-collapse-item title="一句话超级经典小笑话!" name="20">
              <div>1.别紧张,我又不是什么好人……</div>
              <div>2.手拿菜刀砍电线，一路火花带闪电。</div>
              <div>3.最近总是失眠，16小时就醒一次。</div>
              <div>4.人人都说我丑，其实我只是美得不明显。</div>
              <div>5.我从不以强凌弱～～～我欺负他之前真不知道他比我弱…</div>
              <div>6.绅士无非就是耐心的狼。</div>
              <div>7.我又不是人民币，怎么能让人人都喜欢我？！</div>
              <div>8.你为什么不找个安静的地方自个儿数数脑细胞儿去？</div>
              <div>9.知道你过得不好，我也就安心了。</div>
              <div>10.人生只有三天，活在昨天的人迷惑；活在明天的人等待；活在今天的人最踏实。</div>
            </el-collapse-item>
          </el-collapse>
        </basic-container>
      </el-row>
    </el-col>
  </div>
</template>

<script>
  import {mapGetters} from "vuex";

  export default {
    name: "wel",
    data() {
      return {
        activeNames: ['1', '2', '3', '5'],
        logActiveNames: ['20']
      };
    },
    computed: {
      ...mapGetters(["userInfo"]),
    },
    created() {
    },
    methods: {
      handleChange(val) {
        console.log(val);
      }
    }
  };
</script>

<style>
  .el-divider--horizontal {
    margin: 12px 0 !important;
  }

  .el-font-size {
    font-size: 14px;
  }
</style>

