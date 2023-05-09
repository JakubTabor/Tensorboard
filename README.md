# Tensorboard
# First I load the "TensorBoard" notebook extension """%load_ext tensorboard""", then I clear any logs from previous runs """!rm -rf ./logs/ """
# From "keras" i get my "dataset" and save it as "train" and "test" set """(X_train, y_train), (X_test, y_test) = keras.datasets.mnist.load_data()"""
# Then i check length of my sets "len(X_train)" "len(X_test)" and prepare my sets for my "neural network" "scaling them" "X_train / 255 "
# And "flattened" them, size will be (28*28) """X_train.reshape(len(X_train),28*28)""" """X_test.reshape(len(X_test),28*28)"""
# Now I can create my "model" using "keras.Sequential" 
# First I need to use "layers.Flatten" and "input_shape" will be (28,28) """keras.layers.Flatten(input_shape=(28,28))"""
# Next i create "hidden layer" with (100) neurons and "activation" "relu" """keras.layers.Dense(100, activation = 'relu')"""
# I have (10) output neurons and "activation" "sigmoid" """keras.layers.Dense(10, activation = 'sigmoid')"""
# Now I save my "adam model" at "directory" "log_dir = "logs/adam" and prepare my "tensorboard" "log_dir=log_dir" it will call my "model"
# I "compile" my "model" with "optimizer" as "adam", "loss" as "sparse_categorical_crossentropy", because i have values and my "metrics" "accuracy"
# I train my "model" with "X_train and y_train", set number of "epochs" at (5) and save results on my "tensorboard" 
#
