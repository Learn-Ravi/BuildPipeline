node {
   stage 'Checkout'
   		echo 'Checkout'
         git url: 'https://github.com/Learn-Ravi/BuildPipeline.git'
   
   stage 'Build'
         //bat 'nuget restore CodeProject.sln'
         bat "\"${tool 'MSBuild'}\" CodeProject.sln /p:Configuration=Release /p:Platform=\"Any CPU\" /p:ProductVersion=1.0.0.${env.BUILD_NUMBER}"
   stage 'Stage 2'
   		echo 'Hello World 2'
}
