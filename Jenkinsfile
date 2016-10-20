stage 'prepare'
node {
    checkout scm
    def files = findFiles(glob: "*.bat")
    for (file : files) {
        bat file.name
    }
}