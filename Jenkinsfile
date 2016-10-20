stage 'prepare'
node {
    checkout scm
    def files = findFiles(glob: "*.bat")
    for (file in files) {
        bat file.name
    }
}