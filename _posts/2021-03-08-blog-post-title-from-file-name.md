## Trying out Bing character recognition capabilities against other OCR Engines

Exploring and trying to understand how GPT handles image input analysis, especially concerning Optical Character Recognition (OCR). Nowadays we almost take this for granted but usually, this task is split into Text Detection and Text Recognition. 

In this blog, we will briefly explore how OCR Engines like JaidedAI's EasyOCR, PaddleOCR, and Tesseract fare against the results obtained from analyzing images in GPT4 through a prompt. 

The images are as follows: 

Image1:


<img width="200" alt="image" src="https://github.com/vijayvanapalli96/vijay.github.io/assets/46009628/a76bdd30-4536-4f17-ba59-d3881d7b2ffd">

Bing's description of the image above:

<img width="573" alt="bingtext1" src="https://github.com/vijayvanapalli96/vijay.github.io/assets/46009628/32ceb3c4-5e37-4a14-83d0-d2ede0c06257">


Image2: 


<img width="200" alt="image" src="https://github.com/vijayvanapalli96/vijay.github.io/assets/46009628/8c71158b-ef2b-493a-939e-356c95a403bd">

Bing's description of the image above:


<img width="569" alt="bingtext2" src="https://github.com/vijayvanapalli96/vijay.github.io/assets/46009628/1e866bee-d56a-4d35-a029-6ede7d7f94a3">

From the above descriptions, we see that not only is GPT-4 Vision apt at describing the content of the text but also quite good at describing the state the box is in. 



---

### Testing other OCR Engines

EasyOCR follows the two-step process of using CRAFT (Character-Region Awareness For Text detection) for Text detection and Text Recognition to transcribe text. The framework of EasyOCR as shown in its repository is shown below 

<img width="200" alt="image" src="https://github.com/vijayvanapalli96/vijay.github.io/assets/46009628/14893598-135c-4c76-abb6-172da1e65df3">

The outputs obtained from the EasyOCR are as follows 

Image1:
![usbceasyocr](https://github.com/vijayvanapalli96/vijay.github.io/assets/46009628/861a6ca5-b495-4f5a-93bc-145041b0648a)

<img width="200" alt="image" src="https://github.com/vijayvanapalli96/vijay.github.io/assets/46009628/861a6ca5-b495-4f5a-93bc-145041b0648a">

Image1-Confidence:

<img width="200" alt="EasyOCRUSB" src="https://github.com/vijayvanapalli96/vijay.github.io/assets/46009628/2ff471f7-678b-4076-a2af-d960f9fde7d3">

Analysis:


Image2:

<img width="200" alt="image" src="https://github.com/vijayvanapalli96/vijay.github.io/assets/46009628/57857e06-c70c-4198-93ff-54d5883fc648">

Image2-Confidence:

<img width="200" alt="Screenshot 2024-01-23 142352" src="https://github.com/vijayvanapalli96/vijay.github.io/assets/46009628/26ebb70f-7567-46ea-9489-3c39950002c1">

Analysis:



#### Some T-SQL Code

```tsql
SELECT This, [Is], A, Code, Block -- Using SSMS style syntax highlighting
    , REVERSE('abc')
FROM dbo.SomeTable s
    CROSS JOIN dbo.OtherTable o;
```

#### Some PowerShell Code

```powershell
Write-Host "This is a powershell Code block";

# There are many other languages you can use, but the style has to be loaded first

ForEach ($thing in $things) {
    Write-Output "It highlights it using the GitHub style"
}
```
