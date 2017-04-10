node {
    stage('\u2776 one') {
        echo "\u2600 BUILD_URL=${env.BUILD_URL}"
        def workspace = pwd()
        echo "\u2600 workspace=${workspace}"
        f = new File('test.file')
        if (!f.exists()) {
            sh("touch test.file")
        } else {
            fail("file exists")
        }
        checkout scm
    }
    stage('\u2777 two') {
        echo "\u2600 BUILD_URL=${env.BUILD_URL}"
        def workspace = pwd()
        echo "\u2600 workspace=${workspace}"
        sh("if [ -f test.file ]; then echo 'touch ok'; else echo 'touch failed'; fi")
        sh("rm test.file")
    }
}
