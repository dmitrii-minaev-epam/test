node {
    stage('\u2776 one') {
        echo "\u2600 BUILD_URL=${env.BUILD_URL}"
        def workspace = pwd()
        echo "\u2600 workspace=${workspace}"
        checkout scm
    }
    stage('\u2777 two') {
        echo "\u2600 BUILD_URL=${env.BUILD_URL}"
        def workspace = pwd()
        echo "\u2600 workspace=${workspace}"
        touch ok
    }
}
