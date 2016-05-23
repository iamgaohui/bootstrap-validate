# bootstrap-validate
基于jquery的轻量级bootstrap检验插件

用表单的id代替古老的name来执行检验，不用再在HTML代码外套一层form。
简单易用，懒人必备。不包括JQ的话大小为7K左右。

用法：
var val = new validate({
  rule:{
  id:constant,
  id2:constant2
  },
  submitFun:function(){
    //这里是检验成功后的执行的方法
  }
})

目前提供的校验方法有：
	"notEmpty" : "不能为空",
	"password" : "请输入正确的密码",
	"rightfulString" : "请输入合法字符",// 合法字符
	"number" : "只能输入数字",// 数字
	"endlish" : "只能输入英文",// 纯英文
	"numberEnglish" : "只能输入英文或数字",// 英文和数字
	"float" : "只能输入小数",// 浮点型
	"money" : "请输入合法价格",
	"chinese" : "只能输入汉字",// 纯中文
	"mobile" : "请输入正确的手机号",// 手机号
	"tel" : "请输入正确的电话号码",// 电话
	"qq" : "请输入正确的QQ号",// qq
	"zipCode" : "请输入正确的QQ号",
	"email" : "请输入正确的邮箱",// 邮箱
	"positive":"请输入大于0的数字",//大于0的数字
	"checkIdCard" : "请输入正确的身份证号"// 校验身份证
