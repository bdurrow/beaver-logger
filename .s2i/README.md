These files originally came from 
REPO: https://github.com/sclorg/s2i-nodejs-container.git
COMMIT: ce1e4821197dd5121856c2bc2d532c226fa5932a
cp -r ../../s2i-nodejs-container/18/s2i/ ./


Testing with
oc debug -n openshift ImageStreamTag/nodejs:14-ubi8

cd /tmp/ && curl --location https://github.com/bdurrow/beaver-logger/archive/refs/heads/main.zip | bsdtar -xvf- && if [[ -d src ]]; then rm -rf src; fi && mv beaver-logger-main src && if [[ -d build ]]; then rm -rf build; fi && mkdir build && cd build

sh ../src/.s2i/bin/assemble