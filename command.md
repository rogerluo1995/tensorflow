bazel build --config=opt --config=mkl --copt=-mavx --config=cuda //tensorflow/tools/pip_package:build_pip_package --local_resources=4096,8,1.0

rm $HOME/.cache/bazel -fr
sudo rm /usr/local/bin/bazel /etc/bazelrc /usr/local/lib/bazel -fr