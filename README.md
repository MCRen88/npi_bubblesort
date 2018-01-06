# npi_bubblesort
Nerual program interpreters of bubblesort

This project is based on these main resources:

1) DeepMind's Oct 19th publication: [Neural Programmer-Interpreters](https://arxiv.org/abs/1511.06279).
2)The <b>great</b> Addition development of the DeepMind ideas that @mokemokechicken did in his repo: https://github.com/mokemokechicken/keras_npi

requirement
-----------

* Python3

setup
-----

```
pip install -r requirements.txt
```

create training dataset
-----------------------
### create training dataset
```
sh src/run_create_bubblesort_data.sh
```

### create training dataset with showing steps on terminal
```
DEBUG=1 sh src/run_create_bubblesort_data.sh
```

training model
------------------
### Create New Model (-> remove old model if exists and then create new model)
```
NEW_MODEL=1 sh src/run_train_bubblesort_model.sh
```

### Training Existing Model (-> if a model exists, use the model)
```
sh src/run_train_bubblesort_model.sh
```

test model
----------
### check the model accuracy
```
sh src/run_test_bubblesort_model.sh
```

### check the model accuracy with showing steps on terminal
```
DEBUG=1 sh src/run_test_bubblesort_model.sh
```
