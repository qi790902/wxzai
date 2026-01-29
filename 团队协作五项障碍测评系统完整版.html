<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>团队协作五项障碍测评系统</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/qrcode@1.5.3/build/qrcode.min.js"></script>
    <style>
        :root {
            --primary-blue: #1a237e;
            --secondary-blue: #283593;
            --accent-blue: #3949ab;
            --light-blue: #5c6bc0;
            --highlight-blue: #7986cb;
            --text-light: #e8eaf6;
            --text-white: #ffffff;
            --card-bg: rgba(255, 255, 255, 0.1);
            --shadow: 0 8px 32px rgba(0, 0, 0, 0.2);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', 'Microsoft YaHei', sans-serif;
        }
        
        body {
            background: linear-gradient(135deg, #0f1b3d 0%, #1a237e 50%, #283593 100%);
            color: var(--text-light);
            min-height: 100vh;
            padding: 20px;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1400px;
            margin: 0 auto;
        }
        
        header {
            text-align: center;
            padding: 30px 20px;
            margin-bottom: 30px;
            background: var(--card-bg);
            border-radius: 20px;
            backdrop-filter: blur(10px);
            box-shadow: var(--shadow);
            border: 1px solid rgba(255, 255, 255, 0.1);
            position: relative;
        }
        
        h1 {
            font-size: 2.8rem;
            margin-bottom: 10px;
            background: linear-gradient(to right, #4fc3f7, #2979ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            text-shadow: 0 2px 10px rgba(41, 121, 255, 0.3);
        }
        
        .subtitle {
            font-size: 1.2rem;
            opacity: 0.9;
            max-width: 800px;
            margin: 0 auto;
        }
        
        .dashboard {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 25px;
            margin-bottom: 30px;
        }
        
        @media (max-width: 1100px) {
            .dashboard {
                grid-template-columns: 1fr;
            }
        }
        
        .card {
            background: var(--card-bg);
            border-radius: 20px;
            padding: 25px;
            backdrop-filter: blur(10px);
            box-shadow: var(--shadow);
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 40px rgba(0, 0, 0, 0.3);
        }
        
        .card-title {
            font-size: 1.5rem;
            margin-bottom: 20px;
            color: var(--text-white);
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .card-title i {
            color: #4fc3f7;
        }
        
        .stats-grid {
            display: grid;
            grid-template-columns: repeat(5, 1fr);
            gap: 15px;
            margin-bottom: 30px;
        }
        
        @media (max-width: 900px) {
            .stats-grid {
                grid-template-columns: repeat(2, 1fr);
            }
        }
        
        .stat-item {
            background: rgba(0, 30, 96, 0.4);
            border-radius: 15px;
            padding: 20px 15px;
            text-align: center;
            border: 1px solid rgba(79, 195, 247, 0.2);
            transition: all 0.3s ease;
        }
        
        .stat-item:hover {
            border-color: rgba(79, 195, 247, 0.5);
            background: rgba(0, 30, 96, 0.6);
        }
        
        .stat-value {
            font-size: 2.2rem;
            font-weight: bold;
            color: #4fc3f7;
            margin: 10px 0 5px;
        }
        
        .stat-label {
            font-size: 0.95rem;
            opacity: 0.9;
        }
        
        .progress-bar {
            height: 10px;
            background: rgba(255, 255, 255, 0.1);
            border-radius: 5px;
            margin-top: 10px;
            overflow: hidden;
        }
        
        .progress-fill {
            height: 100%;
            background: linear-gradient(to right, #00bcd4, #2979ff);
            border-radius: 5px;
            transition: width 1.5s ease;
        }
        
        .participant-count {
            font-size: 1.2rem;
            text-align: center;
            padding: 15px;
            background: rgba(0, 30, 96, 0.4);
            border-radius: 15px;
            margin-bottom: 20px;
            border: 1px solid rgba(79, 195, 247, 0.2);
        }
        
        .count-value {
            font-size: 2rem;
            color: #4fc3f7;
            font-weight: bold;
            margin: 0 5px;
        }
        
        .chart-container {
            height: 300px;
            margin-top: 20px;
        }
        
        .high-low-container {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
            margin-top: 20px;
        }
        
        @media (max-width: 768px) {
            .high-low-container {
                grid-template-columns: 1fr;
            }
        }
        
        .high-item, .low-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 12px 15px;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 10px;
            margin-bottom: 10px;
            border-left: 4px solid;
        }
        
        .high-item {
            border-left-color: #4caf50;
        }
        
        .low-item {
            border-left-color: #f44336;
        }
        
        .item-score {
            font-weight: bold;
            font-size: 1.2rem;
        }
        
        .high-item .item-score {
            color: #4caf50;
        }
        
        .low-item .item-score {
            color: #f44336;
        }
        
        .assessment-form {
            margin-top: 20px;
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
        }
        
        .form-control {
            width: 100%;
            padding: 12px 15px;
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 10px;
            color: var(--text-white);
            font-size: 1rem;
        }
        
        .form-control:focus {
            outline: none;
            border-color: #4fc3f7;
            box-shadow: 0 0 0 2px rgba(79, 195, 247, 0.2);
        }
        
        .rating-scale {
            display: flex;
            justify-content: space-between;
            margin-top: 5px;
        }
        
        .rating-option {
            text-align: center;
            flex: 1;
            padding: 8px 5px;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 8px;
            margin: 0 5px;
            cursor: pointer;
            transition: all 0.2s ease;
            border: 1px solid transparent;
        }
        
        .rating-option:hover {
            background: rgba(79, 195, 247, 0.2);
        }
        
        .rating-option.selected {
            background: rgba(79, 195, 247, 0.3);
            border-color: #4fc3f7;
            transform: translateY(-2px);
        }
        
        .rating-value {
            font-size: 1.2rem;
            font-weight: bold;
            color: #4fc3f7;
        }
        
        .rating-label {
            font-size: 0.8rem;
            margin-top: 5px;
            opacity: 0.8;
        }
        
        .question-item {
            background: rgba(0, 0, 0, 0.2);
            padding: 20px;
            border-radius: 15px;
            margin-bottom: 20px;
            border-left: 4px solid var(--accent-blue);
        }
        
        .question-text {
            font-weight: 500;
            margin-bottom: 15px;
        }
        
        .btn {
            padding: 14px 28px;
            border: none;
            border-radius: 10px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.3s ease;
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }
        
        .btn-primary {
            background: linear-gradient(to right, #2979ff, #00bcd4);
            color: white;
        }
        
        .btn-primary:hover {
            transform: translateY(-3px);
            box-shadow: 0 7px 20px rgba(41, 121, 255, 0.4);
        }
        
        .btn-secondary {
            background: rgba(255, 255, 255, 0.1);
            color: white;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .btn-secondary:hover {
            background: rgba(255, 255, 255, 0.2);
        }
        
        .btn-success {
            background: linear-gradient(to right, #4caf50, #2e7d32);
            color: white;
        }
        
        .btn-success:hover {
            transform: translateY(-3px);
            box-shadow: 0 7px 20px rgba(76, 175, 80, 0.4);
        }
        
        .btn-full {
            width: 100%;
        }
        
        .button-group {
            display: flex;
            gap: 15px;
            margin-top: 30px;
            flex-wrap: wrap;
        }
        
        .report-content {
            background: rgba(0, 0, 0, 0.2);
            border-radius: 15px;
            padding: 25px;
            margin-top: 20px;
            max-height: 400px;
            overflow-y: auto;
            line-height: 1.7;
        }
        
        .report-section {
            margin-bottom: 25px;
        }
        
        .report-section h4 {
            color: #4fc3f7;
            margin-bottom: 10px;
            padding-bottom: 8px;
            border-bottom: 1px solid rgba(79, 195, 247, 0.3);
        }
        
        footer {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            opacity: 0.7;
            font-size: 0.9rem;
        }
        
        .pill {
            display: inline-block;
            padding: 5px 12px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            margin-right: 8px;
            margin-bottom: 8px;
        }
        
        .pill-high {
            background: rgba(76, 175, 80, 0.2);
            color: #4caf50;
        }
        
        .pill-low {
            background: rgba(244, 67, 54, 0.2);
            color: #f44336;
        }
        
        .loading {
            text-align: center;
            padding: 40px;
        }
        
        .pulse {
            animation: pulse 1.5s infinite;
        }
        
        @keyframes pulse {
            0% { opacity: 0.6; }
            50% { opacity: 1; }
            100% { opacity: 0.6; }
        }
        
        .empty-state {
            text-align: center;
            padding: 40px 20px;
            opacity: 0.7;
        }
        
        .empty-state i {
            font-size: 3rem;
            margin-bottom: 20px;
            color: #4fc3f7;
        }
        
        .alert {
            padding: 12px 15px;
            border-radius: 10px;
            margin: 10px 0;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .alert-info {
            background: rgba(33, 150, 243, 0.2);
            border-left: 4px solid #2196f3;
        }
        
        .alert-success {
            background: rgba(76, 175, 80, 0.2);
            border-left: 4px solid #4caf50;
        }
        
        .alert-warning {
            background: rgba(255, 193, 7, 0.2);
            border-left: 4px solid #ffc107;
        }
        
        .alert-error {
            background: rgba(244, 67, 54, 0.2);
            border-left: 4px solid #f44336;
        }
        
        .modal-overlay {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(0, 0, 0, 0.7);
            display: none;
            justify-content: center;
            align-items: center;
            z-index: 1000;
            backdrop-filter: blur(5px);
        }
        
        .modal {
            background: var(--card-bg);
            border-radius: 20px;
            padding: 30px;
            max-width: 500px;
            width: 90%;
            max-height: 90vh;
            overflow-y: auto;
            box-shadow: var(--shadow);
            border: 1px solid rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(10px);
        }
        
        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .modal-title {
            font-size: 1.5rem;
            color: var(--text-white);
        }
        
        .modal-close {
            background: none;
            border: none;
            color: var(--text-light);
            font-size: 1.5rem;
            cursor: pointer;
            width: 40px;
            height: 40px;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 50%;
            transition: all 0.3s ease;
        }
        
        .modal-close:hover {
            background: rgba(255, 255, 255, 0.1);
        }
        
        .modal-body {
            margin-bottom: 20px;
        }
        
        .qrcode-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 20px;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 15px;
            margin: 20px 0;
        }
        
        #qrcode {
            background: white;
            padding: 10px;
            border-radius: 10px;
            margin-bottom: 20px;
            width: 200px;
            height: 200px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .share-url {
            width: 100%;
            padding: 12px 15px;
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 10px;
            color: var(--text-white);
            font-size: 0.9rem;
            margin-top: 15px;
            word-break: break-all;
            font-family: monospace;
        }
        
        .share-instruction {
            font-size: 0.9rem;
            opacity: 0.8;
            text-align: center;
            margin-top: 15px;
        }
        
        .share-btn-container {
            position: absolute;
            top: 20px;
            right: 20px;
        }
        
        @media (max-width: 768px) {
            .share-btn-container {
                position: static;
                margin-top: 20px;
                display: flex;
                justify-content: center;
            }
            
            h1 {
                font-size: 2.2rem;
            }
        }
        
        .data-export-container {
            margin-top: 20px;
            padding: 20px;
            background: rgba(0, 0, 0, 0.2);
            border-radius: 15px;
        }
        
        .data-export-buttons {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
            margin-top: 15px;
        }
        
        .data-import-container {
            margin-top: 20px;
            padding: 20px;
            background: rgba(0, 0, 0, 0.2);
            border-radius: 15px;
        }
        
        .data-import-textarea {
            width: 100%;
            padding: 12px 15px;
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 10px;
            color: var(--text-white);
            font-size: 0.9rem;
            min-height: 120px;
            font-family: monospace;
            margin-top: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <h1><i class="fas fa-users"></i> 团队协作五项障碍测评系统</h1>
            <p class="subtitle">基于帕特里克·兰西奥尼的团队协作模型，评估团队在信任、冲突、承诺、责任和结果五个维度的表现，实时生成团队分析报告</p>
            
            <div class="share-btn-container">
                <button id="shareBtn" class="btn btn-success">
                    <i class="fas fa-qrcode"></i> 分享二维码
                </button>
            </div>
        </header>
        
        <div class="alert alert-info">
            <i class="fas fa-info-circle"></i>
            <div>团队成员可通过扫描二维码或访问链接参与测评，所有数据将实时汇总并生成团队分析报告。</div>
        </div>
        
        <div class="participant-count">
            当前已有 <span class="count-value" id="participantCount">0</span> 人参与测评
        </div>
        
        <div class="dashboard">
            <div class="card">
                <h2 class="card-title"><i class="fas fa-chart-bar"></i> 团队五项障碍得分</h2>
                <div class="stats-grid" id="scoresContainer">
                    <!-- 五项障碍得分将通过JS动态生成 -->
                </div>
                
                <div class="chart-container">
                    <canvas id="scoreChart"></canvas>
                </div>
            </div>
            
            <div class="card">
                <h2 class="card-title"><i class="fas fa-trophy"></i> 最高与最低得分项</h2>
                <div class="high-low-container">
                    <div>
                        <h3 style="color: #4caf50; margin-bottom: 15px;"><i class="fas fa-arrow-up"></i> 最高5个得分项</h3>
                        <div id="highScoresContainer">
                            <!-- 最高得分项将通过JS动态生成 -->
                        </div>
                    </div>
                    <div>
                        <h3 style="color: #f44336; margin-bottom: 15px;"><i class="fas fa-arrow-down"></i> 最低5个得分项</h3>
                        <div id="lowScoresContainer">
                            <!-- 最低得分项将通过JS动态生成 -->
                        </div>
                    </div>
                </div>
                
                <div style="margin-top: 30px;">
                    <h3 style="margin-bottom: 15px;"><i class="fas fa-calculator"></i> 平均得分</h3>
                    <div class="stat-item">
                        <div class="stat-value" id="averageScore">0.0</div>
                        <div class="stat-label">团队总体平均分</div>
                        <div class="progress-bar">
                            <div class="progress-fill" id="averageProgress" style="width: 0%"></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        
        <div class="card">
            <h2 class="card-title"><i class="fas fa-clipboard-check"></i> 个人测评问卷</h2>
            <p style="margin-bottom: 20px; opacity: 0.9;">请根据您所在团队的实际情况，对以下陈述进行评分（1-5分，1表示完全不同意，5表示完全同意）</p>
            
            <div class="assessment-form">
                <div class="form-group">
                    <label for="participantName">您的姓名（可选）</label>
                    <input type="text" id="participantName" class="form-control" placeholder="匿名参与者">
                </div>
                
                <div id="questionsContainer">
                    <!-- 问题将通过JS动态生成 -->
                </div>
                
                <div class="button-group">
                    <button id="submitBtn" class="btn btn-primary btn-full">
                        <i class="fas fa-paper-plane"></i> 提交测评
                    </button>
                </div>
            </div>
        </div>
        
        <div class="card">
            <h2 class="card-title"><i class="fas fa-file-alt"></i> 团队分析报告</h2>
            <p style="margin-bottom: 15px; opacity: 0.9;">基于当前所有参与者的测评数据生成的详细分析报告</p>
            
            <div class="button-group">
                <button id="generateReportBtn" class="btn btn-primary">
                    <i class="fas fa-sync-alt"></i> 生成/更新报告
                </button>
                <button id="downloadReportBtn" class="btn btn-secondary">
                    <i class="fas fa-download"></i> 下载报告
                </button>
                <button id="clearDataBtn" class="btn btn-secondary">
                    <i class="fas fa-trash-alt"></i> 清空数据
                </button>
            </div>
            
            <div class="report-content" id="reportContent">
                <div class="empty-state">
                    <i class="fas fa-file-alt"></i>
                    <h3>暂无分析报告</h3>
                    <p>点击"生成报告"按钮，根据当前测评数据生成详细分析报告</p>
                </div>
            </div>
            
            <div class="data-export-container">
                <h3 style="margin-bottom: 15px;"><i class="fas fa-database"></i> 数据管理</h3>
                <p style="margin-bottom: 10px; opacity: 0.9;">导出测评数据以便在其他设备导入，或与团队成员共享数据</p>
                
                <div class="data-export-buttons">
                    <button id="exportDataBtn" class="btn btn-secondary">
                        <i class="fas fa-file-export"></i> 导出数据
                    </button>
                    <button id="importDataBtn" class="btn btn-secondary">
                        <i class="fas fa-file-import"></i> 导入数据
                    </button>
                </div>
            </div>
        </div>
        
        <footer>
            <p>团队协作五项障碍测评系统 &copy; 2023 | 基于帕特里克·兰西奥尼的《团队协作的五种障碍》模型</p>
            <p style="margin-top: 5px; font-size: 0.8rem;">提示：所有数据仅存储在您的浏览器本地，不会上传到服务器。通过二维码分享可让团队成员参与测评。</p>
        </footer>
    </div>

    <!-- 二维码模态框 -->
    <div id="qrCodeModal" class="modal-overlay">
        <div class="modal">
            <div class="modal-header">
                <h3 class="modal-title"><i class="fas fa-qrcode"></i> 分享测评链接</h3>
                <button class="modal-close" id="closeModalBtn">&times;</button>
            </div>
            <div class="modal-body">
                <p>团队成员可通过微信扫描下方二维码，直接访问测评页面参与测评：</p>
                
                <div class="qrcode-container">
                    <div id="qrcode"></div>
                    <p style="font-weight: bold; margin-bottom: 10px;">团队协作五项障碍测评</p>
                    <p class="share-instruction">使用微信扫描二维码，即可打开测评页面</p>
                </div>
                
                <p style="margin-top: 20px;">或者复制以下链接分享给团队成员：</p>
                <div class="share-url" id="shareUrl"></div>
                
                <div class="button-group" style="margin-top: 20px;">
                    <button id="copyUrlBtn" class="btn btn-secondary">
                        <i class="fas fa-copy"></i> 复制链接
                    </button>
                    <button id="refreshQrBtn" class="btn btn-secondary">
                        <i class="fas fa-redo"></i> 重新生成二维码
                    </button>
                </div>
            </div>
        </div>
    </div>

    <!-- 数据导入模态框 -->
    <div id="importModal" class="modal-overlay">
        <div class="modal">
            <div class="modal-header">
                <h3 class="modal-title"><i class="fas fa-file-import"></i> 导入测评数据</h3>
                <button class="modal-close" id="closeImportModalBtn">&times;</button>
            </div>
            <div class="modal-body">
                <p>请粘贴从其他设备导出的测评数据JSON字符串：</p>
                
                <div class="alert alert-warning">
                    <i class="fas fa-exclamation-triangle"></i>
                    <div>注意：导入数据将覆盖当前所有测评数据，请谨慎操作！</div>
                </div>
                
                <textarea id="importDataText" class="data-import-textarea" placeholder="请在此处粘贴导出的JSON数据..."></textarea>
                
                <div class="button-group" style="margin-top: 20px;">
                    <button id="confirmImportBtn" class="btn btn-primary">
                        <i class="fas fa-check"></i> 确认导入
                    </button>
                    <button id="cancelImportBtn" class="btn btn-secondary">
                        <i class="fas fa-times"></i> 取消
                    </button>
                </div>
            </div>
        </div>
    </div>

    <script>
        // 团队协作五项障碍模型
        const fiveDysfunctions = [
            { id: 'trust', name: '信任', color: '#2979ff', description: '团队成员之间相互信任，敢于暴露弱点和错误' },
            { id: 'conflict', name: '冲突', color: '#00bcd4', description: '团队能够进行建设性的冲突，聚焦于问题而非人身攻击' },
            { id: 'commitment', name: '承诺', color: '#4caf50', description: '团队成员对决策和行动计划做出真正的承诺' },
            { id: 'accountability', name: '责任', color: '#ff9800', description: '团队成员互相督促，对行为和结果负责' },
            { id: 'results', name: '结果', color: '#9c27b0', description: '团队成员关注集体成果而非个人利益' }
        ];

        // 测评问题库 - 每个障碍4个问题，共20个问题
        const assessmentQuestions = [
            { id: 1, category: 'trust', text: '团队成员敢于承认自己的错误和不足', reverse: false },
            { id: 2, category: 'trust', text: '团队成员之间愿意寻求帮助，而不担心被视为无能', reverse: false },
            { id: 3, category: 'trust', text: '团队成员愿意相互提供建设性反馈', reverse: false },
            { id: 4, category: 'trust', text: '团队成员之间能够坦诚交流，不需要刻意保持谨慎', reverse: false },
            
            { id: 5, category: 'conflict', text: '团队能够就重要问题展开激烈但富有建设性的辩论', reverse: false },
            { id: 6, category: 'conflict', text: '团队成员在会议中能够充分表达不同意见', reverse: false },
            { id: 7, category: 'conflict', text: '团队冲突通常围绕问题本身而非人际关系', reverse: false },
            { id: 8, category: 'conflict', text: '不同意见能够得到充分讨论后才做出决定', reverse: false },
            
            { id: 9, category: 'commitment', text: '团队会议结束后，每个人都清楚下一步该做什么', reverse: false },
            { id: 10, category: 'commitment', text: '团队成员对团队决策有清晰的共识，即使起初有不同意见', reverse: false },
            { id: 11, category: 'commitment', text: '团队决策后，所有成员都能积极支持并执行', reverse: false },
            { id: 12, category: 'commitment', text: '团队能够及时做出明确决策，避免拖延', reverse: false },
            
            { id: 13, category: 'accountability', text: '团队成员会互相提醒未完成的工作或低标准表现', reverse: false },
            { id: 14, category: 'accountability', text: '团队成员感到有责任实现团队目标，而不仅是个人目标', reverse: false },
            { id: 15, category: 'accountability', text: '团队成员在他人表现不佳时会直接提出关切', reverse: false },
            { id: 16, category: 'accountability', text: '团队有明确的绩效标准，并且成员会互相督促遵守', reverse: false },
            
            { id: 17, category: 'results', text: '团队成员将团队成功置于个人利益之上', reverse: false },
            { id: 18, category: 'results', text: '团队成员经常讨论团队的整体进展和目标达成情况', reverse: false },
            { id: 19, category: 'results', text: '团队成员为团队目标未能达成而感到不安', reverse: false },
            { id: 20, category: 'results', text: '团队能抵制分散注意力的活动，专注于关键目标', reverse: false }
        ];

        // 初始化本地存储
        const STORAGE_KEY = 'teamAssessmentData';
        let participants = [];
        let teamScores = {
            trust: 0,
            conflict: 0,
            commitment: 0,
            accountability: 0,
            results: 0
        };
        
        let questionStats = [];
        let chart = null;

        // DOM 加载完成后初始化
        document.addEventListener('DOMContentLoaded', function() {
            loadData();
            renderQuestions();
            updateDashboard();
            setupEventListeners();
        });

        // 从本地存储加载数据
        function loadData() {
            const savedData = localStorage.getItem(STORAGE_KEY);
            if (savedData) {
                try {
                    const data = JSON.parse(savedData);
                    participants = data.participants || [];
                } catch (e) {
                    console.error('加载数据失败:', e);
                    participants = [];
                }
            }
            
            calculateTeamStats();
        }

        // 保存数据到本地存储
        function saveData() {
            const data = {
                participants: participants,
                lastUpdated: new Date().toISOString(),
                version: '1.0'
            };
            localStorage.setItem(STORAGE_KEY, JSON.stringify(data));
        }

        // 计算团队统计信息
        function calculateTeamStats() {
            for (const key in teamScores) {
                teamScores[key] = 0;
            }
            
            questionStats = assessmentQuestions.map(q => ({
                id: q.id,
                text: q.text,
                category: q.category,
                totalScore: 0,
                participantCount: 0,
                averageScore: 0
            }));
            
            if (participants.length === 0) {
                return;
            }
            
            participants.forEach(participant => {
                participant.scores.forEach((score, index) => {
                    const question = assessmentQuestions[index];
                    if (question) {
                        teamScores[question.category] += score;
                        
                        questionStats[index].totalScore += score;
                        questionStats[index].participantCount += 1;
                    }
                });
            });
            
            for (const key in teamScores) {
                const categoryQuestions = assessmentQuestions.filter(q => q.category === key).length;
                teamScores[key] = participants.length > 0 ? 
                    (teamScores[key] / (participants.length * categoryQuestions)).toFixed(1) : 0;
            }
            
            questionStats.forEach(stat => {
                stat.averageScore = stat.participantCount > 0 ? 
                    (stat.totalScore / stat.participantCount).toFixed(1) : 0;
            });
        }

        // 渲染测评问题
        function renderQuestions() {
            const container = document.getElementById('questionsContainer');
            container.innerHTML = '';
            
            assessmentQuestions.forEach((question, index) => {
                const questionElement = document.createElement('div');
                questionElement.className = 'question-item';
                questionElement.innerHTML = `
                    <div class="question-text">${index + 1}. ${question.text}</div>
                    <div class="rating-scale">
                        <div class="rating-option" data-question="${index}" data-value="1">
                            <div class="rating-value">1</div>
                            <div class="rating-label">完全不同意</div>
                        </div>
                        <div class="rating-option" data-question="${index}" data-value="2">
                            <div class="rating-value">2</div>
                            <div class="rating-label">不同意</div>
                        </div>
                        <div class="rating-option" data-question="${index}" data-value="3">
                            <div class="rating-value">3</div>
                            <div class="rating-label">一般</div>
                        </div>
                        <div class="rating-option" data-question="${index}" data-value="4">
                            <div class="rating-value">4</div>
                            <div class="rating-label">同意</div>
                        </div>
                        <div class="rating-option" data-question="${index}" data-value="5">
                            <div class="rating-value">5</div>
                            <div class="rating-label">完全同意</div>
                        </div>
                    </div>
                `;
                
                container.appendChild(questionElement);
            });
            
            document.querySelectorAll('.rating-option').forEach(option => {
                option.addEventListener('click', function() {
                    const questionIndex = parseInt(this.getAttribute('data-question'));
                    
                    const parent = this.parentElement;
                    parent.querySelectorAll('.rating-option').forEach(opt => {
                        opt.classList.remove('selected');
                    });
                    
                    this.classList.add('selected');
                });
            });
        }

        // 更新仪表板
        function updateDashboard() {
            document.getElementById('participantCount').textContent = participants.length;
            
            const scoresContainer = document.getElementById('scoresContainer');
            scoresContainer.innerHTML = '';
            
            fiveDysfunctions.forEach(dysfunction => {
                const score = parseFloat(teamScores[dysfunction.id]) || 0;
                const percentage = (score / 5) * 100;
                
                const scoreElement = document.createElement('div');
                scoreElement.className = 'stat-item';
                scoreElement.innerHTML = `
                    <div class="stat-label">${dysfunction.name}</div>
                    <div class="stat-value">${score}</div>
                    <div class="progress-bar">
                        <div class="progress-fill" style="width: ${percentage}%; background: ${dysfunction.color};"></div>
                    </div>
                `;
                scoresContainer.appendChild(scoreElement);
            });
            
            updateHighLowScores();
            
            const totalAverage = calculateTotalAverage();
            document.getElementById('averageScore').textContent = totalAverage.toFixed(1);
            document.getElementById('averageProgress').style.width = `${(totalAverage / 5) * 100}%`;
            
            updateChart();
        }

        // 计算总体平均分
        function calculateTotalAverage() {
            if (questionStats.length === 0 || participants.length === 0) return 0;
            
            const totalScore = questionStats.reduce((sum, stat) => sum + parseFloat(stat.averageScore), 0);
            return totalScore / questionStats.length;
        }

        // 更新最高和最低得分项
        function updateHighLowScores() {
            const sortedQuestions = [...questionStats].sort((a, b) => b.averageScore - a.averageScore);
            
            const highScoresContainer = document.getElementById('highScoresContainer');
            highScoresContainer.innerHTML = '';
            
            if (sortedQuestions.length > 0) {
                const highScores = sortedQuestions.slice(0, 5);
                highScores.forEach((question, index) => {
                    const questionElement = document.createElement('div');
                    questionElement.className = 'high-item';
                    questionElement.innerHTML = `
                        <div>
                            <div><strong>${getCategoryName(question.category)}</strong></div>
                            <div style="font-size: 0.9rem; opacity: 0.9;">${question.text}</div>
                        </div>
                        <div class="item-score">${parseFloat(question.averageScore).toFixed(1)}</div>
                    `;
                    highScoresContainer.appendChild(questionElement);
                });
            } else {
                highScoresContainer.innerHTML = '<div class="empty-state">暂无数据</div>';
            }
            
            const lowScoresContainer = document.getElementById('lowScoresContainer');
            lowScoresContainer.innerHTML = '';
            
            if (sortedQuestions.length > 0) {
                const lowScores = sortedQuestions.slice(-5).reverse();
                lowScores.forEach((question, index) => {
                    const questionElement = document.createElement('div');
                    questionElement.className = 'low-item';
                    questionElement.innerHTML = `
                        <div>
                            <div><strong>${getCategoryName(question.category)}</strong></div>
                            <div style="font-size: 0.9rem; opacity: 0.9;">${question.text}</div>
                        </div>
                        <div class="item-score">${parseFloat(question.averageScore).toFixed(1)}</div>
                    `;
                    lowScoresContainer.appendChild(questionElement);
                });
            } else {
                lowScoresContainer.innerHTML = '<div class="empty-state">暂无数据</div>';
            }
        }

        // 获取分类名称
        function getCategoryName(categoryId) {
            const dysfunction = fiveDysfunctions.find(d => d.id === categoryId);
            return dysfunction ? dysfunction.name : categoryId;
        }

        // 更新图表
        function updateChart() {
            const ctx = document.getElementById('scoreChart').getContext('2d');
            
            if (chart) {
                chart.destroy();
            }
            
            const labels = fiveDysfunctions.map(d => d.name);
            const scores = fiveDysfunctions.map(d => parseFloat(teamScores[d.id]) || 0);
            const colors = fiveDysfunctions.map(d => d.color);
            
            chart = new Chart(ctx, {
                type: 'bar',
                data: {
                    labels: labels,
                    datasets: [{
                        label: '平均得分',
                        data: scores,
                        backgroundColor: colors,
                        borderColor: colors.map(color => color.replace('0.8', '1')),
                        borderWidth: 1,
                        borderRadius: 5,
                        maxBarThickness: 60
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    scales: {
                        y: {
                            beginAtZero: true,
                            max: 5,
                            grid: {
                                color: 'rgba(255, 255, 255, 0.1)'
                            },
                            ticks: {
                                color: 'rgba(255, 255, 255, 0.8)',
                                callback: function(value) {
                                    return value.toFixed(1);
                                }
                            }
                        },
                        x: {
                            grid: {
                                color: 'rgba(255, 255, 255, 0.1)'
                            },
                            ticks: {
                                color: 'rgba(255, 255, 255, 0.8)'
                            }
                        }
                    },
                    plugins: {
                        legend: {
                            display: false
                        },
                        tooltip: {
                            callbacks: {
                                label: function(context) {
                                    return `得分: ${context.parsed.y.toFixed(1)}`;
                                }
                            }
                        }
                    }
                }
            });
        }

        // 生成分析报告
        function generateReport() {
            if (participants.length === 0) {
                document.getElementById('reportContent').innerHTML = `
                    <div class="empty-state">
                        <i class="fas fa-exclamation-circle"></i>
                        <h3>暂无数据</h3>
                        <p>请先提交测评数据以生成分析报告</p>
                    </div>
                `;
                return;
            }
            
            const totalAverage = calculateTotalAverage();
            const sortedQuestions = [...questionStats].sort((a, b) => b.averageScore - a.averageScore);
            const highScores = sortedQuestions.slice(0, 5);
            const lowScores = sortedQuestions.slice(-5).reverse();
            
            const dysfunctionAssessments = fiveDysfunctions.map(dysfunction => {
                const score = parseFloat(teamScores[dysfunction.id]);
                let assessment = '';
                
                if (score >= 4.0) {
                    assessment = '表现优秀，是该团队的优势领域';
                } else if (score >= 3.0) {
                    assessment = '表现良好，但有提升空间';
                } else if (score >= 2.0) {
                    assessment = '表现一般，需要关注和改进';
                } else {
                    assessment = '表现较弱，是需要重点提升的领域';
                }
                
                return { ...dysfunction, score, assessment };
            });
            
            const reportHTML = `
                <div class="report-section">
                    <h4><i class="fas fa-users"></i> 报告概览</h4>
                    <p>本报告基于 <strong>${participants.length} 名团队成员</strong> 的测评数据生成，评估了团队在协作五项障碍上的表现。总体平均分为 <strong>${totalAverage.toFixed(1)}</strong>（满分5分）。</p>
                    <p>报告生成时间: ${new Date().toLocaleString('zh-CN')}</p>
                </div>
                
                <div class="report-section">
                    <h4><i class="fas fa-chart-line"></i> 各维度得分分析</h4>
                    ${dysfunctionAssessments.map(item => `
                        <div style="margin-bottom: 15px;">
                            <div style="display: flex; justify-content: space-between; margin-bottom: 5px;">
                                <span><strong>${item.name}</strong>: ${item.description}</span>
                                <span style="font-weight: bold; color: ${item.color}">${item.score} 分</span>
                            </div>
                            <div class="progress-bar" style="height: 8px; margin-bottom: 5px;">
                                <div class="progress-fill" style="width: ${(item.score / 5) * 100}%; background: ${item.color};"></div>
                            </div>
                            <div style="font-size: 0.9rem;">${item.assessment}</div>
                        </div>
                    `).join('')}
                </div>
                
                <div class="report-section">
                    <h4><i class="fas fa-thumbs-up"></i> 优势项目 (最高5个得分项)</h4>
                    <p>以下项目团队表现较好，是团队的优势所在：</p>
                    ${highScores.map((item, index) => `
                        <div style="margin-bottom: 10px; padding: 10px; background: rgba(76, 175, 80, 0.1); border-radius: 8px;">
                            <div style="display: flex; justify-content: space-between;">
                                <span><strong>${index + 1}. ${item.text}</strong></span>
                                <span style="color: #4caf50; font-weight: bold;">${parseFloat(item.averageScore).toFixed(1)} 分</span>
                            </div>
                            <div style="font-size: 0.9rem; margin-top: 5px;">
                                <span class="pill pill-high">${getCategoryName(item.category)}</span>
                            </div>
                        </div>
                    `).join('')}
                </div>
                
                <div class="report-section">
                    <h4><i class="fas fa-exclamation-triangle"></i> 待改进项目 (最低5个得分项)</h4>
                    <p>以下项目团队得分较低，是需要重点关注的改进领域：</p>
                    ${lowScores.map((item, index) => `
                        <div style="margin-bottom: 10px; padding: 10px; background: rgba(244, 67, 54, 0.1); border-radius: 8px;">
                            <div style="display: flex; justify-content: space-between;">
                                <span><strong>${index + 1}. ${item.text}</strong></span>
                                <span style="color: #f44336; font-weight: bold;">${parseFloat(item.averageScore).toFixed(1)} 分</span>
                            </div>
                            <div style="font-size: 0.9rem; margin-top: 5px;">
                                <span class="pill pill-low">${getCategoryName(item.category)}</span>
                            </div>
                        </div>
                    `).join('')}
                </div>
                
                <div class="report-section">
                    <h4><i class="fas fa-lightbulb"></i> 改进建议</h4>
                    <p>基于测评结果，我们为您提供以下改进建议：</p>
                    <ul style="padding-left: 20px;">
                        <li><strong>建立信任</strong>: ${teamScores.trust < 3 ? '通过团队建设活动、个人经历分享和定期的一对一交流，增强团队成员间的相互了解和信任。' : '团队信任基础良好，可进一步通过共同应对挑战来深化信任关系。'}</li>
                        <li><strong>管理冲突</strong>: ${teamScores.conflict < 3 ? '建立建设性冲突的规范，鼓励团队成员在会议上表达不同意见，聚焦问题而非人身攻击。' : '团队冲突管理得当，继续保持开放讨论的氛围，确保所有观点都能被听到。'}</li>
                        <li><strong>达成承诺</strong>: ${teamScores.commitment < 3 ? '确保会议有明确的决策和行动计划，使用"同意但保留意见"的方法，让所有人支持团队决定。' : '团队承诺度较高，可进一步通过明确责任和截止日期来强化执行力。'}</li>
                        <li><strong>共担责任</strong>: ${teamScores.accountability < 3 ? '建立明确的绩效标准，定期进行进度回顾，鼓励团队成员互相提醒和督促。' : '团队责任感较强，可进一步通过公开承诺和定期检查来保持高标准。'}</li>
                        <li><strong>关注结果</strong>: ${teamScores.results < 3 ? '明确团队优先目标，定期检查进展，将团队成果与个人激励相结合。' : '团队结果导向良好，继续保持对关键目标的聚焦，防止分散注意力。'}</li>
                    </ul>
                </div>
                
                <div class="report-section">
                    <h4><i class="fas fa-calendar-check"></i> 行动计划建议</h4>
                    <p>建议团队在接下来一个月内采取以下具体行动：</p>
                    <ol style="padding-left: 20px;">
                        <li>召开团队测评结果分享会，讨论本次测评发现</li>
                        <li>针对得分最低的2-3个项目，制定具体的改进措施</li>
                        <li>设立每月检查点，回顾团队协作改进进展</li>
                        <li>考虑在3个月后重新测评，评估改进效果</li>
                    </ol>
                </div>
            `;
            
            document.getElementById('reportContent').innerHTML = reportHTML;
        }

        // 下载报告
        function downloadReport() {
            if (participants.length === 0) {
                showAlert('暂无数据可下载报告', 'error');
                return;
            }
            
            const reportContent = document.getElementById('reportContent');
            if (!reportContent || reportContent.querySelector('.empty-state')) {
                showAlert('请先生成报告再下载', 'error');
                return;
            }
            
            let textContent = '团队协作五项障碍测评分析报告\n';
            textContent += '='.repeat(50) + '\n\n';
            textContent += `报告生成时间: ${new Date().toLocaleString('zh-CN')}\n`;
            textContent += `参与测评人数: ${participants.length}\n\n`;
            
            textContent += '各维度得分:\n';
            textContent += '-'.repeat(30) + '\n';
            fiveDysfunctions.forEach(dysfunction => {
                const score = parseFloat(teamScores[dysfunction.id]) || 0;
                textContent += `${dysfunction.name}: ${score}分\n`;
            });
            
            const totalAverage = calculateTotalAverage();
            textContent += `\n总体平均分: ${totalAverage.toFixed(1)}分\n\n`;
            
            const sortedQuestions = [...questionStats].sort((a, b) => b.averageScore - a.averageScore);
            const highScores = sortedQuestions.slice(0, 5);
            const lowScores = sortedQuestions.slice(-5).reverse();
            
            textContent += '优势项目 (最高5个得分项):\n';
            textContent += '-'.repeat(40) + '\n';
            highScores.forEach((item, index) => {
                textContent += `${index + 1}. ${item.text} (${getCategoryName(item.category)}): ${parseFloat(item.averageScore).toFixed(1)}分\n`;
            });
            
            textContent += '\n待改进项目 (最低5个得分项):\n';
            textContent += '-'.repeat(40) + '\n';
            lowScores.forEach((item, index) => {
                textContent += `${index + 1}. ${item.text} (${getCategoryName(item.category)}): ${parseFloat(item.averageScore).toFixed(1)}分\n`;
            });
            
            textContent += '\n改进建议:\n';
            textContent += '-'.repeat(40) + '\n';
            textContent += teamScores.trust < 3 ? '• 建立信任: 通过团队建设活动、个人经历分享和定期的一对一交流，增强团队成员间的相互了解和信任。\n' : '• 建立信任: 团队信任基础良好，可进一步通过共同应对挑战来深化信任关系。\n';
            textContent += teamScores.conflict < 3 ? '• 管理冲突: 建立建设性冲突的规范，鼓励团队成员在会议上表达不同意见，聚焦问题而非人身攻击。\n' : '• 管理冲突: 团队冲突管理得当，继续保持开放讨论的氛围，确保所有观点都能被听到。\n';
            textContent += teamScores.commitment < 3 ? '• 达成承诺: 确保会议有明确的决策和行动计划，使用"同意但保留意见"的方法，让所有人支持团队决定。\n' : '• 达成承诺: 团队承诺度较高，可进一步通过明确责任和截止日期来强化执行力。\n';
            textContent += teamScores.accountability < 3 ? '• 共担责任: 建立明确的绩效标准，定期进行进度回顾，鼓励团队成员互相提醒和督促。\n' : '• 共担责任: 团队责任感较强，可进一步通过公开承诺和定期检查来保持高标准。\n';
            textContent += teamScores.results < 3 ? '• 关注结果: 明确团队优先目标，定期检查进展，将团队成果与个人激励相结合。\n' : '• 关注结果: 团队结果导向良好，继续保持对关键目标的聚焦，防止分散注意力。\n';
            
            const blob = new Blob([textContent], { type: 'text/plain;charset=utf-8' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = `团队协作测评报告_${new Date().toISOString().slice(0, 10)}.txt`;
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            URL.revokeObjectURL(url);
            
            showAlert('报告下载成功！', 'success');
        }

        // 生成二维码
        function generateQRCode() {
            const qrcodeElement = document.getElementById('qrcode');
            const shareUrlElement = document.getElementById('shareUrl');
            
            qrcodeElement.innerHTML = '';
            
            const placeholder = document.createElement('div');
            placeholder.className = 'qrcode-placeholder';
            qrcodeElement.appendChild(placeholder);
            
            let currentUrl = window.location.href;
            
            if (currentUrl.startsWith('file://')) {
                currentUrl = window.location.href;
                shareUrlElement.textContent = currentUrl;
                shareUrlElement.style.color = "#ff9800";
                shareUrlElement.style.borderColor = "#ff9800";
                
                qrcodeElement.innerHTML = `
                    <div style="text-align: center; padding: 20px;">
                        <i class="fas fa-exclamation-triangle" style="font-size: 3rem; color: #ff9800; margin-bottom: 15px;"></i>
                        <h4 style="color: #ff9800;">本地文件限制</h4>
                        <p>当前页面是本地文件，生成的二维码可能无法被扫描访问。</p>
                        <p>请将本文件上传到服务器后，二维码才能正常使用。</p>
                    </div>
                `;
                return;
            }
            
            shareUrlElement.textContent = currentUrl;
            shareUrlElement.style.color = "";
            shareUrlElement.style.borderColor = "";
            
            try {
                const canvas = document.createElement('canvas');
                qrcodeElement.appendChild(canvas);
                
                QRCode.toCanvas(canvas, currentUrl, {
                    width: 180,
                    height: 180,
                    margin: 1,
                    color: {
                        dark: '#1a237e',
                        light: '#ffffff'
                    }
                }, function(error) {
                    if (error) {
                        console.error('生成二维码失败:', error);
                        qrcodeElement.innerHTML = `
                            <div style="text-align: center; padding: 20px;">
                                <i class="fas fa-exclamation-circle" style="font-size: 3rem; color: #f44336; margin-bottom: 15px;"></i>
                                <h4 style="color: #f44336;">二维码生成失败</h4>
                                <p>无法生成二维码，请尝试刷新页面重试。</p>
                            </div>
                        `;
                    } else {
                        canvas.style.width = '100%';
                        canvas.style.height = '100%';
                        canvas.style.display = 'block';
                        
                        if (placeholder.parentNode === qrcodeElement) {
                            qrcodeElement.removeChild(placeholder);
                        }
                    }
                });
            } catch (error) {
                console.error('二维码生成异常:', error);
                qrcodeElement.innerHTML = `
                    <div style="text-align: center; padding: 20px;">
                        <i class="fas fa-exclamation-circle" style="font-size: 3rem; color: #f44336; margin-bottom: 15px;"></i>
                        <h4 style="color: #f44336;">二维码生成失败</h4>
                        <p>无法生成二维码，请尝试刷新页面重试。</p>
                    </div>
                `;
            }
        }

        // 显示提示消息
        function showAlert(message, type = 'info') {
            const alertElement = document.createElement('div');
            alertElement.className = `alert alert-${type}`;
            alertElement.innerHTML = `
                <i class="fas fa-${type === 'success' ? 'check-circle' : type === 'warning' ? 'exclamation-triangle' : type === 'error' ? 'times-circle' : 'info-circle'}"></i>
                <div>${message}</div>
            `;
            
            const container = document.querySelector('.container');
            container.insertBefore(alertElement, container.firstChild);
            
            setTimeout(() => {
                alertElement.style.opacity = '0';
                alertElement.style.transition = 'opacity 0.5s ease';
                setTimeout(() => {
                    if (alertElement.parentNode) {
                        alertElement.parentNode.removeChild(alertElement);
                    }
                }, 500);
            }, 3000);
        }

        // 导出数据
        function exportData() {
            const data = {
                participants: participants,
                lastUpdated: new Date().toISOString(),
                version: '1.0'
            };
            
            const dataStr = JSON.stringify(data, null, 2);
            const blob = new Blob([dataStr], { type: 'application/json' });
            const url = URL.createObjectURL(blob);
            const a = document.createElement('a');
            a.href = url;
            a.download = `团队测评数据_${new Date().toISOString().slice(0, 10)}.json`;
            document.body.appendChild(a);
            a.click();
            document.body.removeChild(a);
            URL.revokeObjectURL(url);
            
            showAlert('数据导出成功！', 'success');
        }

        // 导入数据
        function importData() {
            const importModal = document.getElementById('importModal');
            importModal.style.display = 'flex';
            
            document.getElementById('importDataText').value = '';
        }

        // 确认导入数据
        function confirmImport() {
            const dataText = document.getElementById('importDataText').value.trim();
            
            if (!dataText) {
                showAlert('请输入要导入的数据', 'error');
                return;
            }
            
            try {
                const data = JSON.parse(dataText);
                
                if (!data.participants || !Array.isArray(data.participants)) {
                    throw new Error('数据格式不正确');
                }
                
                if (confirm(`确定要导入 ${data.participants.length} 条测评记录吗？这将覆盖当前所有数据。`)) {
                    participants = data.participants;
                    saveData();
                    calculateTeamStats();
                    updateDashboard();
                    
                    document.getElementById('importModal').style.display = 'none';
                    
                    showAlert(`成功导入 ${participants.length} 条测评记录！`, 'success');
                    
                    generateReport();
                }
            } catch (error) {
                console.error('导入数据失败:', error);
                showAlert('数据格式不正确，请检查后重试', 'error');
            }
        }

        // 复制到剪贴板
        function copyToClipboard(text) {
            if (navigator.clipboard && window.isSecureContext) {
                navigator.clipboard.writeText(text).then(function() {
                    showAlert('链接已复制到剪贴板！', 'success');
                }, function() {
                    fallbackCopyText(text);
                });
            } else {
                fallbackCopyText(text);
            }
        }
        
        // 备用复制方法
        function fallbackCopyText(text) {
            const textArea = document.createElement('textarea');
            textArea.value = text;
            textArea.style.position = 'fixed';
            textArea.style.left = '-999999px';
            textArea.style.top = '-999999px';
            document.body.appendChild(textArea);
            textArea.focus();
            textArea.select();
            
            try {
                const successful = document.execCommand('copy');
                if (successful) {
                    showAlert('链接已复制到剪贴板！', 'success');
                } else {
                    showAlert('复制失败，请手动复制链接', 'error');
                }
            } catch (err) {
                console.error('复制失败:', err);
                showAlert('复制失败，请手动复制链接: ' + text, 'error');
            }
            
            document.body.removeChild(textArea);
        }

        // 设置事件监听器
        function setupEventListeners() {
            document.getElementById('submitBtn').addEventListener('click', submitAssessment);
            document.getElementById('generateReportBtn').addEventListener('click', generateReport);
            document.getElementById('downloadReportBtn').addEventListener('click', downloadReport);
            
            document.getElementById('clearDataBtn').addEventListener('click', function() {
                if (confirm('确定要清空所有测评数据吗？此操作不可撤销。')) {
                    localStorage.removeItem(STORAGE_KEY);
                    participants = [];
                    calculateTeamStats();
                    updateDashboard();
                    generateReport();
                    
                    document.querySelectorAll('.rating-option').forEach(opt => {
                        opt.classList.remove('selected');
                    });
                    document.getElementById('participantName').value = '';
                    
                    showAlert('数据已清空', 'success');
                }
            });
            
            document.getElementById('shareBtn').addEventListener('click', function() {
                const qrCodeModal = document.getElementById('qrCodeModal');
                qrCodeModal.style.display = 'flex';
                
                generateQRCode();
            });
            
            document.getElementById('closeModalBtn').addEventListener('click', function() {
                document.getElementById('qrCodeModal').style.display = 'none';
            });
            
            document.getElementById('copyUrlBtn').addEventListener('click', function() {
                const url = window.location.href;
                copyToClipboard(url);
            });
            
            document.getElementById('refreshQrBtn').addEventListener('click', function() {
                generateQRCode();
                showAlert('正在重新生成二维码...', 'info');
            });
            
            document.getElementById('exportDataBtn').addEventListener('click', exportData);
            document.getElementById('importDataBtn').addEventListener('click', importData);
            
            document.getElementById('closeImportModalBtn').addEventListener('click', function() {
                document.getElementById('importModal').style.display = 'none';
            });
            
            document.getElementById('cancelImportBtn').addEventListener('click', function() {
                document.getElementById('importModal').style.display = 'none';
            });
            
            document.getElementById('confirmImportBtn').addEventListener('click', confirmImport);
            
            document.querySelectorAll('.modal-overlay').forEach(modal => {
                modal.addEventListener('click', function(e) {
                    if (e.target === this) {
                        this.style.display = 'none';
                    }
                });
            });
            
            document.addEventListener('keydown', function(e) {
                if (e.key === 'Escape') {
                    document.querySelectorAll('.modal-overlay').forEach(modal => {
                        modal.style.display = 'none';
                    });
                }
            });
        }

        // 提交测评
        function submitAssessment() {
            const scores = [];
            let allAnswered = true;
            
            for (let i = 0; i < assessmentQuestions.length; i++) {
                const selectedOption = document.querySelector(`.rating-option.selected[data-question="${i}"]`);
                if (selectedOption) {
                    const score = parseInt(selectedOption.getAttribute('data-value'));
                    scores.push(score);
                } else {
                    allAnswered = false;
                    const questionElement = document.querySelectorAll('.question-item')[i];
                    questionElement.style.boxShadow = '0 0 0 2px rgba(255, 0, 0, 0.3)';
                    setTimeout(() => {
                        questionElement.style.boxShadow = '';
                    }, 2000);
                }
            }
            
            if (!allAnswered) {
                showAlert('请回答所有问题后再提交', 'error');
                return;
            }
            
            const name = document.getElementById('participantName').value.trim() || '匿名参与者';
            
            const participant = {
                id: Date.now(),
                name: name,
                timestamp: new Date().toISOString(),
                scores: scores
            };
            
            participants.push(participant);
            
            saveData();
            
            calculateTeamStats();
            
            updateDashboard();
            
            document.querySelectorAll('.rating-option').forEach(opt => {
                opt.classList.remove('selected');
            });
            document.getElementById('participantName').value = '';
            
            showAlert(`感谢 ${name} 提交测评！您的数据已保存。`, 'success');
            
            generateReport();
        }
    </script>
</body>
</html>
