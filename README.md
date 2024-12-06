# Task_1
import numpy as np
x=np.arrange(1,1001) #thats the input
y=x*2 #thats the output 
print (x)
print (y)
import tensorflow as tf
model=tf.keras.sequential([
      tf.keras.layers.dense(1)
      tf.keras.layers.dense(10)
      tf.keras.layers.dense(10)
      tf.keras.layers.dense(1) ])
model.compile(optimizer='adam' , loss='mse')
model.fit(x,y, epochs=200)
model.predict(np.array([500]))
