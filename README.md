# Tensorboard
# First I load the "TensorBoard" notebook extension """%load_ext tensorboard""", then I clear any logs from previous runs """!rm -rf ./logs/ """
# From "keras" i get my "dataset" and save it as "train" and "test" set """(X_train, y_train), (X_test, y_test) = keras.datasets.mnist.load_data()"""
# Then i check length of my sets "len(X_train)" "len(X_test)" and prepare my sets for my "neural network" "scaling them" "X_train / 255 "
# And "flattened" them, size will be (28*28) """X_train.reshape(len(X_train),28*28)""" """X_test.reshape(len(X_test),28*28)"""
# Now I can create my "model" using "keras.Sequential" 
