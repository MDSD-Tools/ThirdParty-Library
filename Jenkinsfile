@Library('MDSDtoolsLib@master') _
MDSDToolsPipeline {
    buildWithGradle {}
    dockerWithRunParameters """
       -e GITHUB_PACKAGES_USER=MDSD-Tools-Bot
       -e GITHUB_PACKAGES_TOKEN=${credentials('f216be9b-6081-4b9f-889e-470f131cb755')}
    """
    deployUpdatesite 'build/updatesite'
    skipQualityMetrics true
    skipDeploy false
}
