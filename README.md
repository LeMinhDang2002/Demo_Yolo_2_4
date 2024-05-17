## :wrench: Dependencies and Installation

- Python 3.10

### Installation

1. Clone repo

    ```bash
    git clone https://github.com/LeMinhDang2002/Demo_Yolo_2_4.git
    cd Demo_Yolo_2_4
    ```
2. Create ENV
    ```bash
    C:\Users\Tên Máy\AppData\Local\Programs\Python\Python310\python.exe -m venv env
    .\env\Scripts\Activate.ps1
    ```

3. Clone GFPGAN
    ```bash
    git clone https://github.com/TencentARC/GFPGAN.git
    cd .\GFPGAN

    pip install basicsr

    pip install facexlib

    python setup.py develop

    pip install -r requirements.txt

    ```
4. Install dependent packages
    ```bash
    cd ..
    pip install -r requirements.txt
    ```
5. In file .\MultiPage\env\lib\site-packages\basicsr\data\degradations.py
    ```bash
    Change
    from torchvision.transforms.functional_tensor import rgb_to_grayscale
    to
    from torchvision.transforms.functional import rgb_to_grayscale
    ```

6. Download weights
    1. Download all file weight on [Google Drive](https://drive.google.com/drive/u/0/folders/107Mbd57HGSR5UPSTwB4yCKrMrJfbn-ri)
    2. Save it in the Weights folder

7. Download Image
    1. Download images [Google Drive](https://drive.google.com/drive/u/0/folders/1FdTowwdpC7T-9KiS_Edi-DK1Ch90R144)

8. Run code
    ```bash
    streamlit run home.py
    ```