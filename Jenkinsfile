stage 'prepare'
node {
    checkout scm
    if (isUnix()) {
        def files = findFiles(glob: "*.sh")
        for (int i = 0; i < files.length; i++) {
            sh "./" + files[i].name
        }
    } else {
        def files = findFiles(glob: "*.bat")
        for (int i = 0; i < files.length; i++) {
            bat files[i].name
        }
    }
    echo "done!!!!"
}