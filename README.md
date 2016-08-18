# face-processing
face-processing

[![Build Status](https://travis-ci.org/chakkritte/docker-face-processing.svg?branch=master)](https://travis-ci.org/chakkritte/docker-face-processing)

Build your own pyannote/video docker image

    git clone https://github.com/pyannote/pyannote-video.git
    docker pull chakkritte/docker-face-processing
    cd pyannote-video
    
Download sample video and {dlib|openface} models

    git clone https://github.com/pyannote/pyannote-data.git
    mv pyannote-data data
    
Launch jupyter notebook

    docker run -p 80:8888 -v scripts:/scripts \
                      -v data:/data \
                      -v doc:/notebooks \
                      chakkritte/docker-face-processing
Now visit http://localhost to run this notebook locally.

Ref https://github.com/pyannote/pyannote-video
