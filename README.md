**Environment Setup:**

1. Install Python:
    - Download the latest version of Python from the official website (https://www.python.org/downloads/windows/) and follow the installation instructions.

2. Create a Virtual Environment:
    - Open a anaconda prompt.
    - Create a new virtual environment by running the command:
      ```
      conda create -n myenv
      ```
      Replace `myenv` with the desired name for your virtual environment.

3. Activate the Virtual Environment:
    - Run the following command:
      ```
      conda activate myenv
      ```
    - install cuda toolkit and cudnn library:
        ```
        conda install -c conda-forge cudatoolkit=11.8 cudnn=8.1.0
        ```

4. Install Required Packages:
    - clone the repository into a directory
      ```
      git clone https://github.com/Panhayuthh/DenTeeth-Model.git
      ```
    - Run the following command to install the required packages:
      ```
      pip install absl-py==2.1.0 asttokens==2.4.1 astunparse==1.6.3 cachetools==5.3.3 certifi==2023.7.22 chardet==4.0.0 charset-normalizer==3.3.2 colorama==0.4.6 comm==0.2.2 contourpy==1.2.1 cycler==0.10.0 debugpy==1.8.1 decorator==5.1.1 exceptiongroup==1.2.1 executing==2.0.1 filelock==3.14.0 flatbuffers==24.3.25 fonttools==4.53.0 fsspec==2024.5.0 gast==0.4.0 google-auth==2.29.0 google-auth-oauthlib==0.4.6 google-pasta==0.2.0 grpcio==1.64.0 h5py==3.11.0 idna==2.10 intel-openmp==2021.4.0 ipykernel==6.29.4 ipython==8.25.0 jedi==0.19.1 Jinja2==3.1.4 jupyter_client==8.6.2 jupyter_core==5.7.2 keras==2.10.0 Keras-Preprocessing==1.1.2 kiwisolver==1.4.5 libclang==18.1.1 Markdown==3.6 MarkupSafe==2.1.5 matplotlib==3.9.0 matplotlib-inline==0.1.7 mkl==2021.4.0 mpmath==1.3.0 nest-asyncio==1.6.0 networkx==3.3 numpy==1.26.4 oauthlib==3.2.2 opencv-python==4.9.0.80 opencv-python-headless==4.8.0.74 opt-einsum==3.3.0 packaging==24.0 pandas==2.2.2 parso==0.8.4 pillow==10.3.0 pip==24.0 platformdirs==4.2.2 prompt_toolkit==3.0.45 protobuf==3.19.6 psutil==5.9.8 pure-eval==0.2.2 py-cpuinfo==9.0.0 pyasn1==0.6.0 pyasn1_modules==0.4.0 Pygments==2.18.0 pyparsing==3.1.2 python-dateutil==2.9.0.post0 python-dotenv==1.0.1 python-magic==0.4.27 pytz==2024.1 pywin32==306 PyYAML==6.0.1 pyzmq==26.0.3 requests==2.32.3 requests-oauthlib==2.0.0 requests-toolbelt==1.0.0 roboflow==1.1.30 rsa==4.9 scipy==1.13.1 seaborn==0.13.2 setuptools==69.5.1 six==1.16.0 stack-data==0.6.3 sympy==1.12.1 tbb==2021.12.0 tensorboard==2.10.1 tensorboard-data-server==0.6.1 tensorboard-plugin-wit==1.8.1 tensorflow==2.10.0 tensorflow-estimator==2.10.0 tensorflow-io-gcs-filesystem==0.31.0 termcolor==2.4.0 thop==0.1.1.post2209072238 torch==2.3.0+cu118 torchaudio==2.3.0+cu118 torchvision==0.18.0+cu118 tornado==6.4 tqdm==4.66.4 traitlets==5.14.3 typing_extensions==4.12.0 tzdata==2024.1 ultralytics==8.2.27 urllib3==2.2.1 wcwidth==0.2.13 Werkzeug==3.0.3 wheel==0.43.0 wrapt==1.16.0dio torchvision tornado tqdm traitlets typing_extensions tzdata ultralytics urllib3 wcwidth Werkzeug wheel wrapt
      ```

**(windows Only) GPU Configuration:**

1. Install NVIDIA GPU Drivers:
    - Visit the NVIDIA website (https://www.nvidia.com/Download/index.aspx) and download the appropriate GPU drivers for your system. Follow the installation instructions provided by NVIDIA.

2. Install CUDA Toolkit:
    - Visit the NVIDIA CUDA Toolkit website (https://developer.nvidia.com/cuda-toolkit-archive) and download the CUDA Toolkit compatible with your GPU and operating system. Follow the installation instructions provided by NVIDIA.

3. Install cuDNN Library:
    - Visit the NVIDIA cuDNN website (https://developer.nvidia.com/cudnn) and download the cuDNN library compatible with your CUDA Toolkit version. Follow the installation instructions provided by NVIDIA.

4. Verify GPU Availability:
    - After installing the drivers, CUDA Toolkit, and cuDNN library, you can verify the availability of the GPU by running the following code in a Python script or Jupyter Notebook cell:
      ```python
      import torch
      print(torch.cuda.is_available())
      ```
      If the output is `True`, the GPU is successfully configured.

**Changing Directory:**

To change the necessary directory, follow these steps:

1. Open a command prompt.

2. Navigate to the desired directory using the `cd` command. For example, to change to the directory `C:\Users\PC\Desktop\Programming\Python\Denteeth_Model`, run the following command:
    ```
    cd C:\Users\PC\Desktop\Programming\Python\Denteeth_Model
    ```

That's it! You have now set up the environment, installed the required packages, configured the GPU, and changed the necessary directory. You can proceed with running the program and utilizing the installed packages.
