# 渲染与显示
>结构
>同步
>信号量
>从交换链中获取图像
>提交到 command buffer
>Subpass以来
>显示
>帧变换
>结论

所有内容都会在这一章中一同呈现出来。首先我们需要编写一个名为 **_drawFrame_** 的方法用来在主循环中把三角形显示到屏幕上。定义这个方法并在 **_mainLoop_** 中调用：
`void mainLoop() {
    while (!glfwWindowShouldClose(window)) {
        glfwPollEvents();
        drawFrame();
    }
}

...

void drawFrame() {

}`
