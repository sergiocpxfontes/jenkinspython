pipeline
{
    agent
    {
        label 'SergioOC'
    }
    
    stages
    {
        stage('limpar')
        {
            steps
            {
                cleanWs()
            }
        }
        stage('checkout')
        {
            steps
            {
                git branch: 'main' ,url:'https://github.com/sergiocpxfontes/jenkinspython.git'
            }
        }
        stage('build')
        {
            steps
            {
                bat label:'', script:'C:/Python/3.9/Scripts/pip install pyodbc'
                //bat label:'', script:'pip install -r requirements.txt'
            }
        }
        stage('run')
        {
            steps
            {
                 bat label:'', script:'python PythonApplication1/PythonApplication1/app.py'
            }
        }
        stage('testes')
        {
            steps
            {
                bat label:'servidor A', script:'python PythonApplication1/PythonApplication1/test_app.py'
            }
        }
        stage('resultado')
        {
            steps
            {
                junit '**/test-reports/*.xml'   
            }
            
        }
        
    }
    
}
