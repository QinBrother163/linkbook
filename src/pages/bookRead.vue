<template>
    <div :class="idx_sex == 1?'male':'female'" class="root">
        <div class=" bg">
            <!------------ 顶部 ------------>
            <div class="list-content ">
                <div class="list-content-top">
                    <div class="top_left">
                        <p>第一章</p>
                        <p>霸王硬上弓</p>
                    </div>
                    <div class="top_right">
                        <p><i :class="iconMenu" @click="openTopMenu"></i></p>
                        <div class="set_bg">
                            <span v-for="item in set_bg" :class="item"></span>
                        </div>
                        <div class="set_font">
                            <span>A+</span>
                            <span>A-</span>
                        </div>
                        <topMenu v-show="topMenu_status"></topMenu>
                    </div>
                </div>
            </div>
            <div class="bookInfo list-content mtb30">
                <p>“不，我总共要五十万，是一年也好，两年也好，随你便。不过我有个条件，我要立即拿到这五十万”男人摇摇头说道。</p>
                <p>“五十万一年这个价格还算是合理，不过现在就给你这不可能，虽然我们签订了劳务合同，但是你不是保安公司的，我怎么约束你？你要是拿着钱跑了我找谁去？”李先元皱着眉头问道。</p>
                <p>
                    “这是我的身份证，上面也有我的家庭住址，你可以核对，我可以把身份证押在你这里，另外，我可以给你写张欠条，如果我没有履行好义务，你可以随时报警来抓我，我想有身份证再你那儿我也跑不了，对不对？”男人淡淡地说道。</p>
                <p>
                    “好，所谓疑人不用用人不疑，我李先元做生意从来都是按照规矩办事，不过今天我就破例一回，我相信你，就按照五十万一年来办，你要是真拿着钱跑了就当我李先元瞎了眼了”李先元说完之后就拿起笔和纸写了起来，写完后把纸递给面前的男人，在男人伸手来接的时候又收了回去，然后说道：“不过，在这之前我有几件事情要先说明。我是找你做我女儿的贴身保镖，你必须每天二十四小时保证她的人生安全，这是最基本的，其次，你不能干涉到他的生活，也更加不能有其它任何的逾越之举，不然，即使你身手再好，我也一样能让你付出代价的”。</p>
                <p>“这个不用你说我也知道，我知道该怎么做。这些你可以在雇佣合同里说明，如果我违约了，就必须立即偿还你这五十万块钱，并且承担相应的法律责任”男人点头说道。</p>
                <p>“好，小王，去起草一份合同”李先元说完之后对身边的秘书说道，然后又把那张纸条递给男人说道：“你到秘书那边签完合同之后，拿着这个去财务领钱。我希望你能够马上开始工作”。</p>
                <p>“这个不行，我领完钱之后必须出去一趟，最多一个小时，一个小时之后我再来你这找你”男人摇摇头说着。</p>
                <p>李先元仔细地看着男人，随后点了点头道：“好，可以，我相信你，告诉我，你叫什么名字？”。</p>
                <p>“我叫叶凌天”男人说完之后拿着条子就走到了外面的秘书办公室去了。</p>
                <p>
                    叶凌天签订了合同拿了钱之后就直接出了这家三元集团，叫了辆出租车便直接去了医院，在医院里找到了主治医生的办公室，进去就问道：“王医生，我凑到钱了，请问我现在马上去交钱什么时候能够手术？”。</p>
                <p>
                    “下周吧，具体什么时候我们要根据病人的身体情况来定，你还是赶紧先把钱去交了，因为总共就这么一个合适的肾源，现在另外还有一个病人也在准备换肾手术，你要赶紧，先把这个肾源买下来再说”医生对叶凌天说道。</p>
                <p>“好的，我现在马上去交钱”叶凌天点点头，然后走了出去。</p>
                <p>
                    叶凌天总共刷卡刷了二十多万，肾源十万块，手术费十多万，这还只是这次手术的费用，按照医生的估计，后续的治疗还要十几万，如果保险的话，要准备五十万，这也是叶凌天为什么一定开口要五十万而且是要先拿钱的原因所在。</p>
                <p>交完钱之后，叶凌天又忙完了一些手续上的事情然后走进了病房里，看着病房里那个女孩子苍白的脸，即使是叶凌天这样的铁汉眼睛也忍不住地湿润了。</p>
                <p>“哥，你来了啊，你今天怎么这么早就来了”女孩看到叶凌天后高兴地问道。</p>
                <p>女孩大约二十岁的样子，长的很是乖巧。</p>
                <p>“哥今天放假，怎么样？感觉好些了吗？”叶凌天问道。</p>
                <p>
                    “还是那样，没什么用。哥，我们不治了，我们出院吧。我都听说了，治疗费要好几十万，我们上哪去找几十万？即使现在呆在这里也什么用都没有，一天还要那么多的钱。其实我知道你是舍不得我，可是哥，生老病死都是上天注定，不是谁可以改变的，我已经活了二十年了，有你这个哥哥的疼爱，我已经很满足了，真的。不要在我这个没希望的人身上花那么多的钱了，你还要娶媳妇还要买房子的”女孩说着说着眼泪也流了出来。</p>
                <p>
                    “你在胡说八道什么啊你，谁说你没希望了？你听谁说的？我告诉你，我已经问过医生了，你这个病能够治好，只要找到合适的肾源做个换肾手术，再保守治疗一段时间就能够康复。钱的事情你不用担心，我已经去医院交了钱了，你现在什么也不用想，安安心心地养好身子准备手术。知道吗？”叶凌天呵斥着女孩。</p>
                <p>“已经交了？哥，你哪来的钱啊？这可是几十万啊？”女孩惊讶地看着叶凌天。</p>
                <p>
                    “这个你就不用管了，反正是你哥我赚来的，没抢没偷。另外，哥这段时间要加班，可能没有机会来看你了，这个手机你拿好，我帮你办了卡的，有什么事情你直接给我打电话，听到了没有。想吃什么跟护士说，我都跟护士交代了，到时候我来给钱给她。哥还要回去上班，就不多说了，你一定要听话配合医生的治疗，知道吗？”叶凌天再次嘱咐着女孩。</p>
                <p>“嗯，好的，哥，你千万不要太辛苦了”女孩听说自己有救了，也非常的高兴，她心里清楚，这笔钱肯定是来之不易的。</p>
                <p>叶凌天走出病房的时候眼泪终于下来了，连忙用手擦着，走到一边的长椅上点了根烟开始抽着。</p>
                <p>
                    里面那个女孩叫叶霜，是他的亲妹妹，他们俩兄妹从小便命运多舛，叶凌天只有十岁的时候父亲就去世了，她母亲独自支撑起了整个家，叶凌天十八岁那年出去当兵，因为身体素质各方面表现优异，直接被选进了神秘部队集训，在集训部队里，经过了两年地狱般的训练，叶凌天成为了两百个人里面选出来的十个人中的一个，进入了神秘部队。今年早些时候，他收到了一封家书，是叶霜写给他的，信里写了，他母亲病危，希望能够见到他最后一面。只可惜，叶凌天当时在出任务，根本没看到这封信，等他回来看到这封信的时候，他母亲已经去世一个月了。父母双亡，只剩下了在上大学的妹妹，叶凌天觉得自己愧对这个家太多了，所以，便向部队打了退伍报告，部队领导本来是不同意的，但是考虑到了叶凌天家里特殊的情况还是批准了他的退伍申请。叶凌天回来后便带着妹妹一起生活，只是，他除了会杀人外，其余的什么都不会，最后没有办法才进了一家安保公司去一个仓库里当了个保安，可是好景不长，半个月前，叶霜被送进医院，被检查出了尿毒症，而且很严重，必须要换肾，可是换肾总共加起来需要五十万，叶凌天家里是一穷二白，当兵这些年的工资他都是全部寄回家了。这时，刚好听说安保公司需要一个身手好的人去做保镖，听说保镖工资都不低，于是叶凌天自告奋勇的去了，这也就有了本文开始的那一幕。</p>
                <p>在叶凌天心里，叶霜是他在这个世界上唯一的亲人，他已经愧对了自己的母亲，连她最后一眼都没有见上，所以，不管怎么样，即使让自己去死他也一定要照顾好自己的妹妹。</p>
            </div>
            <div class="list-content">
                <div class="list-content-top mtb30 ">
                    <div class="btn_item">< 上一章</div>
                    <div class="btn_item">菜单</div>
                    <div class="btn_item">下一章 ></div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
    import TopMenu from '../components/TopMenu.vue';

    import {getCookie, setCookie, delCookie} from '../../static/js/util';

    export default {
        name: 'getService',

        data () {
            return {
                idx_sex: 1,
                topMenu_status: false,
                iconMenu: 'icon iconfont icon-mulu',

                set_bg: ['b_c_fff', 'b_c_ccc', 'b_c_f7c', 'b_c_e4d', 'b_c_e0e', 'b_c_000'],
            }
        },
        mounted() {
            let that = this;
            this.setSex();



            let Obj_proxy = {
                name : 'Qin'
            };

            let proxy = new Proxy(Obj_proxy,{
                set(target, key, value, receiver){
                    if (!target.hasOwnProperty(key)){
                        if (isNaN(value)){
                            console.log('error is no number')
                        }
                        return Reflect.set(target, key, value, receiver)
                    }
                }
            });
            proxy.num = 'kk';
            console.log(proxy['num']);




            class Qin {
                constructor() {
                    this.name = 'Qin';
                }

                getName() {
                    return console.log(`my is ${this.name}`)
                }

                setList(arr) {
                    let r = [];
                    for (let i = 0; i < arr.length; i++) {
                        r.push(arr[i])
                    }
                    console.log(r)
                }
            }
            let p3 = new Qin();
            p3.getName();
            p3.setList(['q', 'u', 'y', 't', 'r', 'e', 'w',]);


            function LiangDan() {
                this.name = '梁单';
                this.age = 19;
                this.stature = '150cm';
                this.describe = '浓眉大眼睛，小小的嘴巴，矮胖胖的身体蹦跳的时候像个小兔子';
            }

            LiangDan.prototype = {
                constructor: LiangDan,

                start: function () {
                    this.setStatus();
                    console.log(`小妮子代号：${this.name},家住柳州融水，记忆中还是 ${this.age}岁，身高大概 ${this.stature},${this.describe}`)
                },
                setStatus: function () {
                    let that = this;
                    setTimeout(function () {

                        that.end();
                    }, 3000)
                },
                end: function () {
                    console.log('函数注销!')
                }
            };

            let P1 = new LiangDan();

            P1.start();
        },
        methods: {
            setSex: function () {
                this.idx_sex = getCookie('is_sex');
            },
            openTopMenu: function () {
                let open_k = 'icon iconfont icon-mulu';
                let open_g = 'icon iconfont icon-quxiao';

                let o = this.iconMenu == open_k;

                this.iconMenu = o ? open_g : open_k;

                this.topMenu_status = !this.topMenu_status;
                document.getElementsByTagName("body")[0].className = o ? 'no_overflow' : '';
            },
            go_return: function () {
                window.history.go(-1);
                document.getElementsByTagName("body")[0].className = '';
            },
        },
        components: {
            'topMenu': TopMenu,
        },
    }
</script>

<style lang="scss" scoped type="text/css">
    @import "../assets/scss/pages/bookRead.scss";
</style>