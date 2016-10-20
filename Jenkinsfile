stage 'prepare'
node {
    checkout scm
    def files = findFiles(glob: "*.bat")
    for (int i = 0; i < files.size; i++) {
        bat files[i].name
    }
}