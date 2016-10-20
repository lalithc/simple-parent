node {
   // Mark the code checkout 'stage'....
   stage 'Checkout'

   // Get some code from a GitHub repository
   git url: 'https://github.com/lalithc/simple-parent.git'

   // Get the maven tool.
   // ** NOTE: This 'M3' maven tool must be configured
   // **       in the global configuration.           
   def mvnHome = tool 'mvn3'

   // Mark the code build 'stage'....
   stage 'Build'
   // Run the maven build
   //sh "${mvnHome}/bin/mvn clean install sonar:sonar -Dsonar.host.url=http://192.168.224.139:9000 site"
   sh "${mvnHome}/bin/mvn clean install"
}
