# Assignement 5

## Model 1
```python
model = keras.models.Sequential(
            [
                keras.layers.Conv2D(32, (3, 3), activation="relu", input_shape=(28, 28, 1)),  # layer 1
                keras.layers.MaxPool2D((2, 2)),  # layer 2
                keras.layers.Flatten(),
                keras.layers.Dense(10, activation="softmax"),
            ]
        )
```

#### Training with Training loss & Test Accuracy
![Training](./model_1/accuracy.png)

#### Images and corresponding probability that predicted Right
![right](./model_1/output.png)

#### Images and corresponding probability that predicted Wrong
![wrong](./model_1/output_error.png)

<br>

## Model 2
```python
model = keras.models.Sequential(
            [
                keras.layers.Conv2D(32, (3, 3), activation="relu", input_shape=(28, 28, 1)),  # layer 1
                keras.layers.MaxPool2D((2, 2)),  # layer 2
                keras.layers.Conv2D(64, (3, 3), activation="relu"),  # layer 3
                keras.layers.MaxPool2D((2, 2)),  # layer 4
                keras.layers.Flatten(),
                keras.layers.Dense(10, activation="softmax"),
            ]
        )
```

#### Training with Training loss & Test Accuracy
![Training](./model_2/accuracy.png)

#### Images and corresponding probability that predicted Right
![right](./model_2/output.png)

#### Images and corresponding probability that predicted Wrong
![wrong](./model_2/output_error.png)

<br>

## Model 3
```python
model = keras.models.Sequential(
            [
                keras.layers.Conv2D(32, (3, 3), activation="relu", input_shape=(28, 28, 1)),  # layer 1
                keras.layers.MaxPool2D((2, 2)),  # layer 2
                keras.layers.Conv2D(64, (3, 3), activation="relu"),  # layer 3
                keras.layers.Conv2D(64, (3, 3), activation="relu"),  # layer 4
                keras.layers.MaxPool2D((2, 2)),  # layer 5
                keras.layers.Conv2D(128, (3, 3), activation="relu"),  # layer 6
                keras.layers.Flatten(),
                keras.layers.Dense(10, activation="softmax"),
            ]
        )
```

#### Training with Training loss & Test Accuracy
![Training](./model_3/accuracy.png)

#### Images and corresponding probability that predicted Right
![right](./model_3/output.png)

#### Images and corresponding probability that predicted Wrong
![wrong](./model_3/output_error.png)