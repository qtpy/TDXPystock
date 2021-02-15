# 使用python 玩股票  (代码基于python3 数据库为mysql)
首先申明:使用本项目中的程序抓取或分析股票数据进行的投资行为,造成的损失本人概不负责,如果不能接受请勿查看下载相关代码


使用方法：
---------
一、---通达信操作：
   1、导出个股竞价数据
   
   早盘开盘后（9.25分）当集合竞价数据生成完成了
    
    定位到在A股板块信息列表中，选择"选项，数据导出"--导出所有数据---格式为EXCEL" 等待几十秒后打开文件，删除今日未开盘的个股，
    再另存为EXCEL为 xls的文件
   2、导出板块竞价数据
   
    定位到板块指数列表，在列表中，点选所有板块，选择"选项，数据导出"--导出所有数据---格式为EXCEL" 等待几秒后打开文件
    再另存为excel (格式选择 excel97~2003的xls )
---通达信数据导出完成

二、---写数据：

       写竞价数据 执行：执行“通达信写自定义总价数据文件.py”  
       此功能会将导出的板块与个股的竞价数据导入到通达信用，以供通达信自写指标读取使用
三、---早盘板块异动
       
       执行通达信早盘板块异动.py
       此功能将会读到板块竞价数据，通过自定的条件算出今日异动的板块
       
       
四、---早盘主力异动个股提示
       
       执行通达信早盘异动将会算出早盘异动的个股
       
五、 --- 早盘选股

        执行通达信早盘选股.py 
        会根据导出的excel 算出符合量比组合条件或换手组合条件筛选出符合 条件的个股 

六、 ---查询概念相关联的股票或个股对应的相关概念，与主营业务，公司亮点（支持多条件查询）
   
         概念与早盘数据查询.py 
         python 概念与早盘数据查询.py  "info like '%光伏%'"'"   #查询光伏概念相关的股票
         
         python 概念与早盘数据查询.py  “name='中直股份'”         #查询中直股份的概念与主营业务，公司亮点（支持多只个股查询例："name in('隆基股份','通威股份')"）

         python 概念与早盘数据查询.py stockopendata name='福耀玻璃'  #查询耀玻璃 的早盘数据

七、 ---南北向资金查询
        
        python 南向资金.py  #获取南向资金,并入库
        python 北向资金.py  #获取北赂资金并入库
        python 南向资金分析工具.py 
        python 北向资金分析工具.py 
八、   ---港股优秀企业
      
       python 港股领先企业.py   #获取港股(数据来源于富途证券的"股票百科")关键字:['全球领先' , '行业第一' , '全球第一' ,'市占率第一', '全球最大' , '龙头' ,'全球唯一','中国最大']
        
       
        
感谢您的关注，使用中有任何疑问，请与我联系：QQ:860760123  微信：newhackerman@163.com                          

如果您认为还不错，也可以随意打享



![微信](https://d.pcs.baidu.com/file/c22c1e3feh808eccb67d8967423b2cf7?fid=2617716508-250528-575886981107502&rt=pr&sign=FDtAERVCY-DCb740ccc5511e5e8fedcff06b081203-OTBF%2BButUMfK8J5c9EQJzOB75Qk%3D&expires=8h&chkv=1&chkbd=1&chkpc=et&dp-logid=1053929494857579640&dp-callid=0&dstime=1613356593&r=262792336&vip=0)

