# TPU-Exploration

Where I explore how TPUs work and how to use them.

For that, I will be using free TPU credits offered by 


First, you need to create a google cloud [project](https://cloud.google.com/resource-manager/docs/creating-managing-projects?hl=en&visit_id=637586001278214806-617489911&rd=1)


# Some useful commands


```
gcloud components install alpha
gcloud components update alpha
```


To configure the TPU service using the cloud GPU: 

`gcloud config set compute/zone your-zone-here`


export PROJECT_ID=tpu-exploration
gcloud config set project $PROJECT_ID

europe-west4-a


To get the ctpu CLI locally: 

`wget https://dl.google.com/cloud_tpu/ctpu/latest/linux/ctpu && chmod a+x ctpu`


The easiest method is to use gcloud init and follow the commands you are asked to perform.

# Some useful links: 

TODO: Improve and reorder the links. 


- https://github.com/tensorflow/tpu/tree/master/tools/ctpu 
- https://cloud.google.com/tpu/docs/quickstart
- https://cloud.google.com/tpu/docs/tutorials 
- https://cloud.google.com/tpu/docs/
- Useful Pytorch + XLA tutorial for Kaggle: https://www.kaggle.com/tanlikesmath/the-ultimate-pytorch-tpu-tutorial-jigsaw-xlm-r


- TPU official [doc](https://cloud.google.com/tpu/docs/tpus?hl=en)
- ctpu [repo](https://github.com/tensorflow/tpu/tree/master/tools/ctpu) (useful to run on GCP using the command line)
- XLA [repo](https://github.com/pytorch/xla)(useful to run Pytorch on TPUs)
- XLA [documentation](https://pytorch.org/xla/release/1.8/index.html)


# TODO: Write a blog post here: https://www.kaggle.com/tags/tpu/discussion/new/


curl -O https://dl.google.com/dl/cloudsdk/channels/rapid/downloads/google-cloud-sdk-344.0.0-linux-x86_64.tar.gz



# TODO: Works for Python3.7 only?

pip install -Uqq cloud-tpu-client==0.10 https://storage.googleapis.com/tpu-pytorch/wheels/torch_xla-1.7-cp37-cp37m-linux_x86_64.whl


=> Maybe the answer could be found here? https://github.com/pytorch/xla/blob/master/contrib/scripts/env-setup.py



conda install pytorch==1.7.1 torchvision==0.8.2 torchaudio==0.7.2 cudatoolkit=11.0 -c pytorch