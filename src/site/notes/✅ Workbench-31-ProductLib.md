---
{"dg-publish":true,"permalink":"/workbench-31-product-lib/","tags":["SK-Workbench"]}
---

<button class="mod-cta">✍️ 新建产品信息</button>


<div id="product-view-rj4bpdjcg">
    <style>
    #product-view-rj4bpdjcg .filter-panel { margin-bottom: 1.5em; display: flex; flex-direction: column; gap: 10px; }
    #product-view-rj4bpdjcg .filter-group { display: flex; align-items: center; gap: 10px; flex-wrap: wrap; }
    #product-view-rj4bpdjcg .filter-label { font-weight: bold; font-size: 0.9em; }
    #product-view-rj4bpdjcg .search-input { flex-grow: 1; border: 1px solid var(--background-modifier-border); border-radius: 5px; padding: 6px 8px; background-color: var(--background-secondary); }
    #product-view-rj4bpdjcg .filter-select { border: 1px solid var(--background-modifier-border); border-radius: 5px; padding: 6px 8px; background-color: var(--background-secondary); }
    #product-view-rj4bpdjcg .product-container { display: grid; grid-template-columns: repeat(auto-fill, minmax(220px, 1fr)); gap: 1rem; }
    #product-view-rj4bpdjcg .product-card { background: var(--background-secondary); border: 1px solid var(--background-modifier-border); border-radius: 8px; overflow: hidden; color: var(--text-normal); display: flex; flex-direction: column; transition: all 0.2s ease-out; cursor: pointer; }
    #product-view-rj4bpdjcg .product-card:hover { transform: translateY(-4px); box-shadow: 0 4px 12px rgba(0,0,0,0.1); }
    #product-view-rj4bpdjcg .product-thumbnail { width: 100%; height: 180px; object-fit: cover; background-color: var(--background-primary); }
    #product-view-rj4bpdjcg .product-info { padding: 12px; flex-grow: 1; }
    #product-view-rj4bpdjcg .product-type { font-size: 1.1em; font-weight: 600; margin-bottom: 8px; color: var(--text-normal) !important; }
    #product-view-rj4bpdjcg .product-details { font-size: 0.85em; color: var(--text-muted); line-height: 1.5; }
    #product-view-rj4bpdjcg .product-status { font-size: 0.8em; font-weight: bold; padding: 2px 6px; border-radius: 4px; display: inline-block; margin-top: 8px; }
    #product-view-rj4bpdjcg .status-mass_production { background-color: var(--color-green-faint); color: var(--color-green); }
    #product-view-rj4bpdjcg .status-on_sale { background-color: var(--color-blue-faint); color: var(--color-blue); }
    #product-view-rj4bpdjcg .status-end_of_life { background-color: var(--color-red-faint); color: var(--color-red); }
    #product-view-rj4bpdjcg .status-developing { background-color: var(--color-yellow-faint); color: var(--color-yellow); }
    #product-view-rj4bpdjcg .pagination-controls{display:none;justify-content:center;align-items:center;gap:15px;margin:20px 0;padding-top:15px;border-top:2px solid var(--background-modifier-border)}
    #product-view-rj4bpdjcg .page-btn{border:1px solid var(--background-modifier-border);border-radius:20px;padding:6px 12px;background-color:var(--background-secondary);cursor:pointer;font-size:.9em;}
    #product-view-rj4bpdjcg .page-btn:disabled{opacity:.5;cursor:not-allowed}
    #product-view-rj4bpdjcg #page-info{font-size:.9em;color:var(--text-muted)}
    </style>
    
    <div class="filter-panel">
        <div class="filter-group">
            <label class="filter-label">🔍</label>
            <input type="text" class="search-input" placeholder="搜索型号、产品、描述内容...">
        </div>
        <div class="filter-group">
            <div class="filter-group"><label class="filter-label">系列:</label><select class="filter-select" data-filter-type="series"><option value="All">所有系列</option><option value="Atom">Atom</option><option value="Classic">Classic</option><option value="DemoStation">DemoStation</option><option value="Prime">Prime</option><option value="Showroom">Showroom</option><option value="Skyline">Skyline</option><option value="TradeShow">TradeShow</option></select></div>
            <div class="filter-group"><label class="filter-label">产品:</label><select class="filter-select" data-filter-type="product"><option value="All">所有产品</option><option value="Fuel Dispenser">Fuel Dispenser</option><option value="MobileDispenser">MobileDispenser</option><option value="加油机">加油机</option><option value="配件">配件</option></select></div>
            <div class="filter-group"><label class="filter-label">型号:</label><select class="filter-select" data-filter-type="type"><option value="All">所有型号</option><option value="ADIPEC 2018">ADIPEC 2018</option><option value="I2 配件 2021">I2 配件 2021</option><option value="Istanbul 2019">Istanbul 2019</option><option value="NACS SHOW 2024">NACS SHOW 2024</option><option value="Nacs Show 2019">Nacs Show 2019</option><option value="SK18">SK18</option><option value="SK18D">SK18D</option><option value="SK22">SK22</option><option value="SK36">SK36</option><option value="SK52">SK52</option><option value="SK52-P">SK52-P</option><option value="SK56">SK56</option><option value="SK56-P">SK56-P</option><option value="SK56A-P">SK56A-P</option><option value="SK56V">SK56V</option><option value="SK65">SK65</option><option value="SK65-P">SK65-P</option><option value="Uniti 2024">Uniti 2024</option><option value="Uniti2018">Uniti2018</option><option value="东帝汶">东帝汶</option><option value="俄罗斯">俄罗斯</option><option value="北京展厅2017">北京展厅2017</option><option value="北京展厅2021">北京展厅2021</option><option value="卡塔尔">卡塔尔</option><option value="印度尼西亚">印度尼西亚</option><option value="危地马拉">危地马拉</option><option value="坦桑尼亚">坦桑尼亚</option><option value="孟加拉">孟加拉</option><option value="尼泊尔">尼泊尔</option><option value="沙特阿拉伯">沙特阿拉伯</option><option value="泰国">泰国</option><option value="澳大利亚">澳大利亚</option><option value="秘鲁">秘鲁</option><option value="肯尼亚AfriFueling 2025">肯尼亚AfriFueling 2025</option><option value="菲律宾">菲律宾</option><option value="蒙古">蒙古</option><option value="马来西亚">马来西亚</option></select></div>
        </div>
    </div>
    <div class="product-container"><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of TradeShow AfriFueling 2025.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20TradeShow%20AfriFueling%202025/IMG_0211.jpg?1751351850969" alt="肯尼亚AfriFueling 2025">
            <div class="product-info">
                <div class="product-type">肯尼亚AfriFueling 2025</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2025</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of 加油机-Tradeshow-NACS SHOW 2024-2024.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20%E5%8A%A0%E6%B2%B9%E6%9C%BA-Tradeshow-NACS%20SHOW%202024-2024/%E5%B1%95%E5%93%8102%20%E7%9B%88%E5%86%A0.jpg?1751358820916" alt="NACS SHOW 2024">
            <div class="product-info">
                <div class="product-type">NACS SHOW 2024</div>
                <div class="product-details">加油机<br>年份: 2024</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of TradeShow UNITI 2024.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20TradeShow%20UNITI%202024/PXL_20240514_131902290.MP.jpg?1750401190327" alt="Uniti 2024">
            <div class="product-info">
                <div class="product-type">Uniti 2024</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2024</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Skyline SK56V 2024.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Skyline%20SK56V%202024/%E4%B8%80%E4%BD%93%E6%9C%BA_L_%E8%83%8C%E9%9D%A2.png?1750387683069" alt="SK56V">
            <div class="product-info">
                <div class="product-type">SK56V</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2024</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Skyline SK56 2024.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Skyline%20SK56%202024/4%E6%9E%AA%E6%9C%BAL_%E8%83%8C%E9%9D%A2.png?1750387531251" alt="SK56">
            <div class="product-info">
                <div class="product-type">SK56</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2024</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Skyline SK36 2024.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Skyline%20SK36%202024/SK36_F.png?1750387480190" alt="SK36">
            <div class="product-info">
                <div class="product-type">SK36</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2024</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Prime SK65 2024.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Prime%20SK65%202024/2H_1P_%E6%AD%A3%E9%9D%A2%201.png?1750387332960" alt="SK65-P">
            <div class="product-info">
                <div class="product-type">SK65-P</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2024</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Prime SK56A 2024.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Prime%20SK56%202024/4H_%E6%AD%A3%E9%9D%A2.png?1750387201727" alt="SK56A-P">
            <div class="product-info">
                <div class="product-type">SK56A-P</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2024</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Prime SK56 2024.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Prime%20SK56%202024/4H_%E6%AD%A3%E9%9D%A2.png?1750387201727" alt="SK56-P">
            <div class="product-info">
                <div class="product-type">SK56-P</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2024</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Prime SK52 2024.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Prime%20SK52%202024/2H.png?1750386811042" alt="SK52-P">
            <div class="product-info">
                <div class="product-type">SK52-P</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2024</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 澳大利亚.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E6%BE%B3%E5%A4%A7%E5%88%A9%E4%BA%9A%202020/IMG_1205(08-12-16-47-00).jpg?1750399239748" alt="澳大利亚">
            <div class="product-info">
                <div class="product-type">澳大利亚</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2024</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 孟加拉2024.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E5%AD%9F%E5%8A%A0%E6%8B%892024/13.-EHAD-Classic-52-ko-op-1200x900.jpg?1750397004380" alt="孟加拉">
            <div class="product-info">
                <div class="product-type">孟加拉</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2024</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 东帝汶2024.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E4%B8%9C%E5%B8%9D%E6%B1%B62024/WhatsApp_Image_2025-06-13_at_13.53.48%20(1).jpg?1750397145388" alt="东帝汶">
            <div class="product-info">
                <div class="product-type">东帝汶</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2024</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 马来西亚2023.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E9%A9%AC%E6%9D%A5%E8%A5%BF%E4%BA%9A2023/2023%20BHP+OKR+2+with+SANKI+1+New.png?1750397675356" alt="马来西亚">
            <div class="product-info">
                <div class="product-type">马来西亚</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2023</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 沙特2023.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E6%B2%99%E7%89%B92023/IMG_5902.jpg?1750397537858" alt="沙特阿拉伯">
            <div class="product-info">
                <div class="product-type">沙特阿拉伯</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2023</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of 配件-TradeShow-I2-2021.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20%E9%85%8D%E4%BB%B6-TradeShow-I2-2021/_F6A2392%E5%89%AF%E6%9C%AC.jpg?1751359964802" alt="I2 配件 2021">
            <div class="product-info">
                <div class="product-type">I2 配件 2021</div>
                <div class="product-details">配件<br>年份: 2021</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of 加油机-TradeShow-北京展厅2021-2025.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20%E5%8A%A0%E6%B2%B9%E6%9C%BA-TradeShow-%E5%8C%97%E4%BA%AC%E5%B1%95%E5%8E%852021-2025/_F6A2338.jpg?1751360064183" alt="北京展厅2021">
            <div class="product-info">
                <div class="product-type">北京展厅2021</div>
                <div class="product-details">加油机<br>年份: 2021</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of 加油机-TradeShow-北京展厅2021-2021.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20%E5%8A%A0%E6%B2%B9%E6%9C%BA-TradeShow-%E5%8C%97%E4%BA%AC%E5%B1%95%E5%8E%852021-2021/_F6A2380.jpg?1751360021524" alt="北京展厅2021">
            <div class="product-info">
                <div class="product-type">北京展厅2021</div>
                <div class="product-details">加油机<br>年份: 2021</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 蒙古2021.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E8%92%99%E5%8F%A42021/208092623_4539488056103061_5026611345232861111_n.jpeg?1750397490208" alt="蒙古">
            <div class="product-info">
                <div class="product-type">蒙古</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2021</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 菲律宾2021.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E8%8F%B2%E5%BE%8B%E5%AE%BE2021/WechatIMG205.jpeg?1750397357449" alt="菲律宾">
            <div class="product-info">
                <div class="product-type">菲律宾</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2021</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 秘鲁2021.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E7%A7%98%E9%B2%812021/%E7%A7%98%E9%B2%81-Prime-56.jpg?1750399842781" alt="秘鲁">
            <div class="product-info">
                <div class="product-type">秘鲁</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2021</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 危地马拉2021.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E5%8D%B1%E5%9C%B0%E9%A9%AC%E6%8B%892021/WechatIMG226.jpeg?1750397570356" alt="危地马拉">
            <div class="product-info">
                <div class="product-type">危地马拉</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2021</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 卡塔尔2021.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E5%8D%A1%E5%A1%94%E5%B0%942021/Qatar-Mobile%20Fuel%20Skid.jpg?1750399600792" alt="卡塔尔">
            <div class="product-info">
                <div class="product-type">卡塔尔</div>
                <div class="product-details">MobileDispenser<br>年份: 2021</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 澳大利亚 2020.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E6%BE%B3%E5%A4%A7%E5%88%A9%E4%BA%9A%202020/Austrilia%20-1.jpeg?1750389989862" alt="澳大利亚">
            <div class="product-info">
                <div class="product-type">澳大利亚</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2020</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 泰国2020.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E6%B3%B0%E5%9B%BD2020/Classic-56-8H-Green-Thai-Bangchar-1.jpg?1750398946207" alt="泰国">
            <div class="product-info">
                <div class="product-type">泰国</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2020</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 尼泊尔2020.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E5%B0%BC%E6%B3%8A%E5%B0%942020/Classic%2052-2H%20Nepal.jpg?1750398175390" alt="尼泊尔">
            <div class="product-info">
                <div class="product-type">尼泊尔</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2020</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 孟加拉2020.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E5%AD%9F%E5%8A%A0%E6%8B%892020/2022-02-07%2001.38.37.jpg?1750396487914" alt="孟加拉">
            <div class="product-info">
                <div class="product-type">孟加拉</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2020</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 坦桑尼亚2020.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E5%9D%A6%E6%A1%91%E5%B0%BC%E4%BA%9A2020/Classic-52-2H-CUS1.jpg?1750398655350" alt="坦桑尼亚">
            <div class="product-info">
                <div class="product-type">坦桑尼亚</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2020</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 印度尼西亚2020.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E5%8D%B0%E5%BA%A6%E5%B0%BC%E8%A5%BF%E4%BA%9A2020/Classic-52-2H-White-Indonesia.jpg?1750399075008" alt="印度尼西亚">
            <div class="product-info">
                <div class="product-type">印度尼西亚</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2020</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of CustomerStation 俄罗斯2020.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20CustomerStation%20%E4%BF%84%E7%BD%97%E6%96%AF2020/PRIME-65-8H-2%E4%BF%84%E7%BD%97%E6%96%AF_20200506111018.jpg?1750399471323" alt="俄罗斯">
            <div class="product-info">
                <div class="product-type">俄罗斯</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2020</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of 加油机-TradeShow-Nacs Show 2019-2019.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20%E5%8A%A0%E6%B2%B9%E6%9C%BA-TradeShow-Nacs%20Show%202019-2019/Prime%20SK52%202N2P_resize.jpg?1751359096098" alt="Nacs Show 2019">
            <div class="product-info">
                <div class="product-type">Nacs Show 2019</div>
                <div class="product-details">加油机<br>年份: 2019</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Prime SK65 2019.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Prime%20SK65%202019/16.4H.png?1750313392513" alt="SK65-P">
            <div class="product-info">
                <div class="product-type">SK65-P</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2019</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Prime SK56A 2019.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Prime%20SK56A%202019/14.4H.png?1750313263310" alt="SK56A-P">
            <div class="product-info">
                <div class="product-type">SK56A-P</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2019</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Prime SK56 2019.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Prime%20SK56%202019/15.4H.png?1750313330324" alt="SK56-P">
            <div class="product-info">
                <div class="product-type">SK56-P</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2019</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Prime SK52 2019.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Prime%20SK52%202019/13.2H.png?1750313085674" alt="SK52-P">
            <div class="product-info">
                <div class="product-type">SK52-P</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2019</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Classic SK65 2019.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Classic%20SK65%202019/12.4H.png?1750312264456" alt="SK65">
            <div class="product-info">
                <div class="product-type">SK65</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2019</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Classic SK56 2019.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Classic%20SK56%202019/11.4H.png?1750310863576" alt="SK56">
            <div class="product-info">
                <div class="product-type">SK56</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2019</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Classic SK52 2019.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Classic%20SK52%202019/6.1H1.png?1750310705503" alt="SK52">
            <div class="product-info">
                <div class="product-type">SK52</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2019</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Atom SK18D 2019.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Atom%20SK18D%202019/2.1H_Pipe.png?1750386737321" alt="SK18D">
            <div class="product-info">
                <div class="product-type">SK18D</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2019</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Atom SK18 2019.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Atom%20SK18%202019/1.1H_Pipe.png?1750386644893" alt="SK18">
            <div class="product-info">
                <div class="product-type">SK18</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2019</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of TradeShow Istanbul 2019.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20TradeShow%20Istanbul%202019/IMG_2682.jpg?1750399342577" alt="Istanbul 2019">
            <div class="product-info">
                <div class="product-type">Istanbul 2019</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2019</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of 加油机-TradeShow-ADIPEC 2018-2018.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20%E5%8A%A0%E6%B2%B9%E6%9C%BA-TradeShow-ADIPEC%202018-2018/webwxgetmsgimg%20(1).jpg?1751359321214" alt="ADIPEC 2018">
            <div class="product-info">
                <div class="product-type">ADIPEC 2018</div>
                <div class="product-details">加油机<br>年份: 2018</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of TradeShow UNITI 2018.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20TradeShow%20UNITI%202018/05-20184106.jpg?1751359572119" alt="Uniti2018">
            <div class="product-info">
                <div class="product-type">Uniti2018</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2018</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of Classic SK22 2019.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20Classic%20SK22%202019/12V%E8%87%AA%E5%90%B8%E6%B3%B5%E8%BD%A6%E8%BD%BD%E6%9C%BA-2.jpg?1750216787902" alt="SK22">
            <div class="product-info">
                <div class="product-type">SK22</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2018</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div><div class="product-card" data-path="03 Marketing/031 SANKI ProductLib/Index of SK-ShowRoom 2017.md" style="display: none;">
            <img class="product-thumbnail" src="app://d57273ae47c269ca971fd38febdea054b420/D:/!iCloud/iCloudDrive/iCloud~md~obsidian/Bodreizehn/03%20Marketing/031%20SANKI%20ProductLib/assets/Index%20of%20SK-ShowRoom%202017/P70616-153553.jpg?1750388001979" alt="北京展厅2017">
            <div class="product-info">
                <div class="product-type">北京展厅2017</div>
                <div class="product-details">Fuel Dispenser<br>年份: 2017</div>
                <span class="product-status status-online">Online</span>
            </div>
        </div></div><div class="pagination-controls"><button class="page-btn" id="prev-page">上一页</button><span id="page-info"></span><button class="page-btn" id="next-page">下一页</button></div></div>




