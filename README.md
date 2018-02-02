# caffe
some instruction when training model
# 训练示例 （参数： 求解文件）
caffe train -solver examples/mnist/lenet_solver.prototxt

# 从训练一半的模型快照中恢复训练 （参数：求解文件 快照）
caffe train -solver examples/mnist/lenet_solver.prototxt -snapshot examples/mnist/lenet_iter_5000.solversta

# 由其它训练好的模型 fine-tune  （参数：求解文件 其它训练好的模型参数） 
caffe train -solver examples/finetuning_on_flickr_style/solver.prototxt -weights models/bvlc_reference_caffenet/bvlc_reference_caffenet.caffemodel

# anaconda python 2 3的切换
source activate test_py3
