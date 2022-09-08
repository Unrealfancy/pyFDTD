# pyFDTD
A fast simulation program based on python and ansys-lumerical-FDTD for optical simulation, allowing users to quickly model, run and read simulation results for analysis

本程序主要用于实现计算周期性结构的光学仿真计算，通过lumerical-FDTD提供的pothon API,实现对FDTD的建模控制，同时通过可以对计算结果进行快速分析：    
  
实现的功能：  
1，一键建模，打开文件后会自动读取fsp文件中的材料光参（如果需要添加材料可以预先在fsp文件中添加），添加层数，设置层的厚度，最后点击建模即可一键完成建模，点击运行会进入计算，勾选表格中场可以选择需要观察场的结构层  
2，重叠建模，在建模表右边重叠层处选择除0选项后，会将该层往下平移至与上一层顶端齐平，可用于灵活设置包括刻蚀，十字，包覆层等特异结构。  
3，光谱查看，文件计算完后可以在右边分析面板中选择查看反射透射光谱，程序会根据光谱自动算出吸收，可以选择展示选定线段，点击作图即可观看， 同时如果打开的文件已经有计算结果，也可以直接在分析面板中查看，默认的监视器名称为'R','T','A'，可以选择输入想看的monitor  
4，场分布，右边分析面板可以获得分布图，输入monitor的名字，点击作图，可以获得场分布图，自动获得该monitor的点数，通过point条可以看不同的波长，下面的Interp可以实现场图的插值， 使图片更清晰。

![image](https://user-images.githubusercontent.com/109337832/189107873-ba443ce0-27ac-4a4b-9b03-af221db79df2.png)
![image](https://user-images.githubusercontent.com/109337832/189108036-68ed5361-b7df-4b59-a5d6-4d9e9e3adeb9.png)
