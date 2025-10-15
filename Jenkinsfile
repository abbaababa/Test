pipeline {
    agent any  // 在任意 Agent 上执行

    stages {
        stage('拉取代码') {
            steps {
                echo '🔄 正在拉取 GitHub 仓库代码...'
                // Jenkins 会自动拉取，无需手动 git clone
            }
        }

        stage('构建项目') {
            steps {
                echo '⚙️ 开始构建项目...'
                // 这里写构建命令，例如：
                // sh 'python3 -m py_compile app.py'
            }
        }

        stage('测试代码') {
            steps {
                echo '🧪 运行测试中...'
                // 例如：
                // sh 'pytest tests/'
            }
        }

        stage('部署项目') {
            steps {
                echo '🚀 部署完成！'
                // 例如：
                // sh 'scp -r . user@server:/var/www/app'
            }
        }
    }
}
