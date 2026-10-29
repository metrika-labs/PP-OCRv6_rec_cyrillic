<div align="center">
  <img src="media/banner.webp" alt="Logo" width="100%"/>
  <br>
  <a href="https://huggingface.co/collections/metrika-labs/cyrillic-ocr"><img src="https://img.shields.io/badge/🤗_Hugging_Face-Cyrillic_OCR-FFD21E" alt="Hugging Face"></a>
  <a href="https://github.com/metrika-labs/PP-OCRv6_rec_cyrillic"><img src="https://img.shields.io/badge/GitHub-PP--OCRv6__rec__cyrillic-181717?logo=github" alt="GitHub"></a>
</div>

## Fast OCR models for printed and handwritten Cyrillic text, based on PP-OCRv6

Results on challenging OCR benchmarks featuring distortions, printing defects, and low-quality images.

<img src="media/benchmark-cyrillic.png" alt="Multilingual Cyrillic benchmark" width="50%"/>

<img src="media/benchmark-russian.png" alt="Russian-language benchmark" width="90%"/>

Russian-language OCR benchmark: [ru-ocr-benchmark-hard](https://huggingface.co/datasets/metrika-labs/ru-ocr-benchmark-hard)

## Usage

### 🚀 Recommended for CPU (RapidOCR / ONNX)
* [**PP-OCRv6 Medium Cyrillic (RapidOCR)**](https://huggingface.co/metrika-labs/PP-OCRv6_medium_rec_cyrillic_onnx)
* [**PP-OCRv6 Tiny Cyrillic (RapidOCR)**](https://huggingface.co/metrika-labs/PP-OCRv6_tiny_rec_cyrillic_onnx)

### 🚀 Recommended for GPU (PaddlePaddle)
* [**PP-OCRv6 Medium Cyrillic**](https://huggingface.co/metrika-labs/PP-OCRv6_medium_rec_cyrillic)
* [**PP-OCRv6 Tiny Cyrillic**](https://huggingface.co/metrika-labs/PP-OCRv6_tiny_rec_cyrillic)

## Details
PP-OCRv6 is a family of fast, lightweight text recognition models from PaddlePaddle. The models were trained by Metrika Labs on 7.5 million varied examples of printed and handwritten text from real document scans and synthetic images.

80% of the examples are in Russian. The other 20% are in Kazakh, Belarusian, Uzbek, Tajik, Ukrainian, Bulgarian, Serbian, Macedonian, Tatar, Kyrgyz, Mongolian, Bashkir, Ossetian, Chuvash, Chechen, Yakut, Avar, and other languages that use Cyrillic.

The models work with PaddleOCR and are also available in ONNX format for fast CPU inference with RapidOCR.

The current version supports handwritten text only in Russian. It reads clear handwriting well, but may make mistakes with cursive or less legible handwriting.


<img src="https://raw.githubusercontent.com/metrika-labs/PP-OCRv6_rec_cyrillic/master/media/sample1.png" alt="Пример 1" width="50%"/><br>
PP-OCRv6 Medium: Мир меняется быстро (score: 0.9882)<br>
PP-OCRv6 Tiny: Пир меняется быстро (score: 0.8412)<br>

## Links

Benchmark for evaluating OCR model quality on Russian text: [metrika-labs/ru-ocr-benchmark-hard](https://huggingface.co/datasets/metrika-labs/ru-ocr-benchmark-hard)

Some handwriting examples come from [AntiplagiatCompany/HWR200](https://huggingface.co/datasets/AntiplagiatCompany/HWR200)

Original PaddleOCR repository: [PaddlePaddle/PaddleOCR](https://github.com/PaddlePaddle/PaddleOCR)<br>
RapidOCR repository: [RapidAI/RapidOCR](https://github.com/RapidAI/RapidOCR)
