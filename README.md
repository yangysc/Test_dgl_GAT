# Test_dgl_GAT
Report the bug of the increasing GPU usage.

In the gat.py, what I have changed is that **I remove the internal graph g in the model, and pass it into the model as an input each time**.

After installing the latest dgl library, just download these two files and run the following command, and then watch the GPU usage.

`python3 train.py --dataset=cora --gpu=0 --epochs=20000`

