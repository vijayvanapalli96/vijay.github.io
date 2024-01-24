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


---

### This is a header

![test](https://github.com/vijayvanapalli96/vijay.github.io/assets/46009628/f2ed167e-4c86-4a3a-98df-2a3c1085cc61)

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
