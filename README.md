
# NC_Manual_Tool(V1.35)（基于AutoCAD半自动数控编程工具）

   在手工数控编程中，需人工准确输入各点坐标值、正负号，判断圆弧插补的方向、半径大小及优弧、劣弧； 数据错误(尤其是“+、-”的输错)，会造成刀具碰撞、零件损伤甚至机床损伤。所以针对实际工作中的这些问题， 编写手动NC编程工具，利用AutoCAD图形准确、快速完成数控程序手工编制的工作。
   
   相对于CAM软件的自动编程， NC_Manu_Tool工具具有建模简单、快速、数控程序简洁的特点，比较适用于车间平面数控加工短、平、快的节 奏。它在AutoCAD中绘制图形技术要求低、绘制快速，让“杀鸡”不再用“牛刀”；当然还需要少量手动工作和一点 点的技巧。并且它还可以利用加工经验，自行绘制优化的加工轨迹，生成能够超越CAM软件的数控切削路径，使 得加工效率和质量进一步提升，让操作“大师”更加“大师”。
   
   该小程序是针对Siemens 810D/840D、Fanuc系列数控系统基本指令的编程助手，利用设计人员AutoCAD图纸 （当然，也可以自行绘制）进行比例缩放和整体平移可以快速完成手工编程任务。因VBA中对Windows对象的操作 有限，所以不能使用鼠标右键，只能使用快捷键：Ctrl+A全选、Ctrl+C复制，在记事本和其它编辑器中Ctrl+V粘贴。 该小程序短小、精干，具有以下功能，并在以后进行扩充：

一、预检查手工修改过的尺寸标注，并以紫色圆标注。判断是否需要修改图形，并确保图形1：1比例准确；

二、先按加工原点将图形整体平移到(0,0)，可添加辅助路径，依次选择直线、圆弧、整圆和点等AutoCAD对象，作为加工轨迹;

三、快速、准确生成车削、铣削G功能指令和点位数据；(G41/G42刀补手工添加，Spline以拟合点FitPoints坐标数组形式提供，也可转化为圆弧和直线段间接处理(见后续内容))；

四、快速、准确生成数控点孔程序，处理点、圆弧、整圆对象；

五、刀具轨迹辅助功能：1、模型精确计算车刀进给Fn与理论Rz、Ra关系,让参数不再盲目；2、辅助生成摆线；3、可对曲线等份分线和等长度分线圆弧线,精确处理样条曲线Spline和椭圆Ellipse。

六、！！！编辑完成程序后，需用VeriCut、SmartNC或NC View等程序模拟运行,确保刀具轨迹和程序准确!

                                                       资深金属切削技术研究及应用者：IBMInfo78@126.com (//爱中国!!!)
                                                                    2020年12月8日
