<table align="center" border="0">

<tr><td colspan=2 align="center">

![](doc/deepfacelive_intro.png)

![](doc/logo_onnx.png)
![](doc/logo_directx.png)
![](doc/logo_python.png)

</td></tr>
</table>
<table align="center" border="0">

<tr><td colspan=2 align="center">

## Available ready-to-use face models:

</td></tr>

<tr><td colspan=2 align="center">

<table align="center" border="0">
<tr><td align="center">
Margot Robbie

<img src="doc/celebs/Margot_Robbie/Margot_Robbie.png" width=128></img>

<a href="doc/celebs/Margot_Robbie/examples.md">examples</a>
</td><td align="center">
Tom Cruise

<img src="doc/celebs/Tom_Cruise/Tom_Cruise.jpg" width=128></img>

<a href="doc/celebs/Tom_Cruise/examples.md">examples</a>
</td></tr>
</table>

</td></tr>

<tr><td colspan=2 align="center">
If you want a higher quality or better face match, you can train your own face model using <a href="https://github.com/iperov/DeepFaceLab">DeepFaceLab</a>

Here is an <a href="https://www.tiktok.com/@arnoldschwarzneggar/video/6995538782204300545">example</a> of Arnold Schwarzneggar trained on a particular face and used in a video call. Read the FAQ for more information.

</td></tr>

</table>
<table align="center" border="0">

<tr><td colspan=2 align="center">

## Minimum system requirements

any DirectX12 compatible graphics card

Modern CPU with AVX instructions

4GB RAM, 32GB+ paging file

Windows 10

</td></tr>
<tr><td colspan=2 align="center">

## Setup tutorial

<tr><td colspan=2 align="center">

<a href="doc/setup_tutorial_windows/index.md">Windows 10 x64</a>

## Documentation

<a href="doc/user_faq/user_faq.md">User FAQ</a>

<a href="doc/developer_faq/developer_faq.md">Developer FAQ</a>

</td></tr>
<tr><td colspan=2 align="center">

## Releases

</td></tr>
<tr><td align="right"> <a href="https://mega.nz/folder/m10iELBK#Y0H6BflF9C4k_clYofC7yA">Windows 10 x64 (mega.nz)</a>
</td><td align="center">
DirectX12 build : NVIDIA, AMD, Intel videocards.
</td></tr>
<tr><td colspan=2 align="center">

## Communication groups

<tr><td align="right">
<a href="https://discord.gg/S2h7kPySQp">Discord</a>
</td><td align="center">Official discord channel. English / Russian.</td></tr>

<tr><td align="right">
<a href="https://mrdeepfakes.com/forums/">mrdeepfakes</a>
</td><td align="center">the biggest NSFW English deepfake community</td></tr>

</td></tr>
<tr><td colspan=2 align="center">

## How can I help the project?

</td></tr>
<tr><td colspan=2 align="center">
I need the computing power to train models. 

If you have a free computer with 2080TI or better card with 12GB+ VRAM, you can give me remote access to it. I will train 1 model in a month. Contact me(iperov#6528) in Discord channel.
</td></tr>
<tr><td colspan=2 align="center">
Register github account and push "Star" button.
</td></tr>
<tr><td colspan=2 align="center">
<a href="https://www.paypal.com/paypalme/DeepFaceLab">Donate via Paypal</a>
</td></tr>
<tr><td colspan=2 align="center">
<a href="https://money.yandex.ru/to/41001142318065">Donate via Yandex.Money</a>
</td></tr>
<tr><td colspan=2 align="center">
bitcoin:bc1qewl062v70rszulml3f0mjdjrys8uxdydw3v6rq
</td></tr>
<tr><td colspan=2 align="center">


<!--
    <a href="https://br-stone.online"><img src="doc/logo_barclay_stone.png"></img></a><a href="https://exmo.com"><img src="doc/logo_exmo.png"></img></a>

    presents 

    <tr><td align="right">


    <a href="">Windows (magnet link)</a>
    </td><td align="center">Latest release. Use torrent client to download.</td></tr>
    </tr>
-->

</table>



## Inference Pipeline
Setup config file and run the inference wrapper function:

[config.yml](apps/DeepFaceLive/backend/config.yml)

[inference.py](apps/DeepFaceLive/backend/inference.py)

### Notes:

For GPU Usage:
- install `onnxruntime-gpu`, rather than `onnxruntime`
```
pip install onnxruntime-gpu
```

- install `cupy` for specific cuda version (10.2 for instance)
```
pip install cupy-cuda102
```
or 
```
pip install cupy_cuda102-9.5.0-cp38-cp38-win_amd64.whl
```

- install latest `opencv-contrib-python` if encountering error like "module 'cv2.cv2' has no attribute 'face'"
```
pip install opencv-contrib-python
```

