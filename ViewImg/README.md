## H5 广告动画


## 技术栈

 ->  zepto.js

 ->	swiper

 -> sass

## 开发工具

-> koala


## 2018-5-5 
  布局 加载页面 和 light  用scss

## 2018-5-6
 布局 swiper  编写 scss 调用语法

// 	函数 用于计算 -些算法

  @function pr($size) {
  // 这计算移动端 尺寸
    @return ($size/32) *1 rem
}


// 混合优化部分
 
 // 设置 图片 居中
@mixin bgy($url,$width) {
	background:url($url) no-repeat center / 100% 100%;
	position:absolute;
	left:50%;
	// margin-left: (-$width/32/2)*1rem;
	margin-left: pr(-$width);
}

// 不居中
@mixin bg($url) {
	background:url($url) no-repeat center/ 100% 100%;
	position:absolute;
}
// 设置 尺寸 移动端宽高 
@mixin size($height,$width) {
	height: pr($height);
	width: pr(width);
}