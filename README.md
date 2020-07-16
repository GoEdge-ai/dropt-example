# dropt-example
This repo provides examples of parameter tuning with DrOpt.


## Directory structure
```
.
|
+- trials/	# parameter tuning trial examples
|
+- data/	# datasets for trials
|
+- util/	# utility Python scirpt
|
+- log/		# trial logs (create upon running)
```


## Models
Our trial examples include the following models:
- `func-eggholder`: test function for optimization
- `func-rosenbrock`: another test function for optimization
- `titanic-xgboost`: Titanic survival prediction by XGBoost
- `mnist-pytorch`: handwritten digit recognition with PyTorch framework
- `imagenet-pytorch`: image classification with PyTorch framework


## Run a trial
1. Set up Python enviroment.
   - (Optional) Set up Python virtual enviroment.
2. Go to the folder of a trial example.
3. Install required Python package:
   ```console
   $ pip install -r requirements.txt
   ```
4. Run the trial with DrOpt:
   ```console
   $ droptctl -t TOKEN create
   ```
5. Inspect the trial result on the DrOpt service cloud.


## References
1. DrOpt official service cloud: <https://dropt.goedge.ai>
2. DrOpt documentation: <https://dropt-cli.readthedocs.io>
3. dropt-cli source repo: <https://github.com/GoEdge-ai/dropt-cli>
