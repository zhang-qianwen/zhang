//关于移动端的键盘，IOS不支持键盘展开时的resize事件
//设想1：移动端屏幕显示的高度（弹出$(window).height()与$(document).height()无效，均为603）
//设想2：虚拟键盘弹出时滚动条的高度改变，键盘弹出时滚动条设置到底部，此时的scrollTop为虚拟键盘的高度
//设想3：关于scrollIntoView(false)的应用

//关于设想1，猜测由于alert事件导致input失去焦点，导致屏幕高度没有发生改变
