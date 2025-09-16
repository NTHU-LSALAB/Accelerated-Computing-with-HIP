# AMD HIP 加速運算技術指南

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Language](https://img.shields.io/badge/language-LaTeX-green.svg)](https://www.latex-project.org/)

**[English Version Below ↓](#english-version)**

## 專案簡介

本專案是《Accelerated Computing with HIP》第二版的中文翻譯版本。這本書由 Yifan Sun、Sabila Al Jannat、Trinayan Baruah 和 David Kaeli 共同撰寫，為高效能運算社群提供了一份具參考價值的指南，幫助程式開發人員充分利用 Exascale 計算的優勢。

**HIP（Heterogeneous-computing Interface for Portability）** 是 AMD 開發的一種可移植的平行程式設計語言，允許開發者在 AMD 和 NVIDIA GPU 上運行相同的程式碼。HIP 是 C/C++ 的擴展，提供了類似 CUDA 的程式設計模型，但具有更好的可移植性。

## 書籍內容

本書包含 13 章內容與三個附錄，提供讀者一份簡明但完整的 HIP 程式設計相關參考：

1. **第 1 章** - 圖形處理器和平行程式設計基礎
2. **第 2-3 章** - HIP 核心程式設計和 HIP runtime API
3. **第 4-5 章** - HIP 程式設計模式與 AMD GPU 架構
4. **第 6 章** - AMD GPU 架構詳細介紹
5. **第 7 章** - HIP 除錯與效能分析工具
6. **第 8 章** - 效能優化方法
7. **第 9 章** - ROCm 函式庫
8. **第 10 章** - 多 GPU 程式設計
9. **第 11 章** - 機器學習框架
10. **第 12 章** - 資料中心計算
11. **第 13 章** - 第三方工具

**附錄**：
- **附錄 A** - ROCm 安裝指南
- **附錄 B** - AMD GPU CDNA 組合語言程式碼
- **附錄 C** - OmniTools 介紹

## 翻譯團隊

**原始作者**：
- Yifan Sun
- Sabila Al Jannat
- Trinayan Baruah
- David Kaeli

**中文翻譯團隊**：
- 牟展佑
- 程詩柔
- 謝之豫
- 牟懋軒
- 林展毅
- 黃煒智
- 魏士勛
- 白宸安
- 郭品毅
- 周志遠

## 專案結構

```
AMD-hip/
├── BookTemplate.tex          # 主要 LaTeX 模板
├── Chapters/                 # 章節內容
│   ├── chap0.tex
│   ├── chap1.tex
│   └── ...
├── Appendici/                # 附錄內容
│   ├── AppendiceA.tex
│   ├── AppendiceB.tex
│   └── AppendiceC.tex
├── FileAusiliari/            # 輔助檔案
│   ├── Titolo2.tex          # 標題頁
│   ├── Introduzione.tex     # 前言
│   ├── Bibliografia.bib     # 參考文獻
│   └── ...
└── README.md                # 本檔案
```

## 編譯說明

要編譯此 LaTeX 文件，您需要：

1. **安裝 LaTeX 發行版**：
   - 推薦使用 TeX Live 或 MiKTeX
   - 確保包含 XeLaTeX 編譯器（用於中文支援）

2. **安裝中文字體**：
   - 確保系統已安裝 Noto Sans CJK TC 字體
   - 或修改 `BookTemplate.tex` 中的字體設定

3. **編譯命令**：
   ```bash
   xelatex BookTemplate.tex
   bibtex BookTemplate
   xelatex BookTemplate.tex
   xelatex BookTemplate.tex
   ```

## 相關資源

- **AMD ROCm 官方文件**：https://docs.amd.com
- **HIP 開源專案**：https://github.com/ROCm/HIP
- **範例程式碼**：https://gitlab.com/syifan/hipbookexample
- **ROCm 平台**：https://rocm.docs.amd.com

## 授權條款

本專案遵循原始書籍的授權條款。請參閱原始出版物的授權資訊。

## 貢獻指南

歡迎對翻譯品質提出建議或回報錯誤。請透過以下方式貢獻：

1. 建立 Issue 回報問題
2. 提交 Pull Request 改善翻譯
3. 提供技術建議或修正

## 聯絡資訊

如有任何問題或建議，請透過 GitHub Issues 與我們聯絡。

---

**注意**：本專案為教育用途，旨在促進 HIP 程式設計技術的學習與推廣。

---

# English Version {#english-version}

# Accelerated Computing with HIP

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Language](https://img.shields.io/badge/language-LaTeX-green.svg)](https://www.latex-project.org/)

## Project Overview

This project is a Chinese translation of the second edition of "Accelerated Computing with HIP". The book, authored by Yifan Sun, Sabila Al Jannat, Trinayan Baruah, and David Kaeli, provides a valuable guide for the high-performance computing community to help developers take full advantage of Exascale computing.

**HIP (Heterogeneous-computing Interface for Portability)** is a portable parallel programming language developed by AMD that allows developers to run the same code on both AMD and NVIDIA GPUs. HIP is an extension of C/C++ that provides a CUDA-like programming model with better portability.

## Book Contents

The book contains 13 chapters and three appendices, providing readers with a concise but comprehensive reference for HIP programming:

1. **Chapter 1** - Graphics Processors and Parallel Programming Fundamentals
2. **Chapters 2-3** - HIP Core Programming and HIP Runtime API
3. **Chapters 4-5** - HIP Programming Patterns and AMD GPU Architecture
4. **Chapter 6** - Detailed Introduction to AMD GPU Architecture
5. **Chapter 7** - HIP Debugging and Performance Analysis Tools
6. **Chapter 8** - Performance Optimization Methods
7. **Chapter 9** - ROCm Libraries
8. **Chapter 10** - Multi-GPU Programming
9. **Chapter 11** - Machine Learning Frameworks
10. **Chapter 12** - Data Center Computing
11. **Chapter 13** - Third-party Tools

**Appendices**:
- **Appendix A** - ROCm Installation Guide
- **Appendix B** - AMD GPU CDNA Assembly Language Code
- **Appendix C** - OmniTools Introduction

## Translation Team

**Original Authors**:
- Yifan Sun
- Sabila Al Jannat
- Trinayan Baruah
- David Kaeli

**Chinese Translation Team**:
- 牟展佑
- 程詩柔
- 謝之豫
- 牟懋軒
- 林展毅
- 黃煒智
- 魏士勛
- 白宸安
- 郭品毅
- 周志遠

## Project Structure

```
AMD-hip/
├── BookTemplate.tex          # Main LaTeX template
├── Chapters/                 # Chapter contents
│   ├── chap0.tex
│   ├── chap1.tex
│   └── ...
├── Appendici/                # Appendix contents
│   ├── AppendiceA.tex
│   ├── AppendiceB.tex
│   └── AppendiceC.tex
├── FileAusiliari/            # Auxiliary files
│   ├── Titolo2.tex          # Title page
│   ├── Introduzione.tex     # Introduction
│   ├── Bibliografia.bib     # Bibliography
│   └── ...
└── README.md                # This file
```

## Compilation Instructions

To compile this LaTeX document, you need:

1. **Install LaTeX Distribution**:
   - Recommended: TeX Live or MiKTeX
   - Ensure XeLaTeX compiler is included (for Chinese support)

2. **Install Chinese Fonts**:
   - Ensure Noto Sans CJK TC font is installed on your system
   - Or modify font settings in `BookTemplate.tex`

3. **Compilation Commands**:
   ```bash
   xelatex BookTemplate.tex
   bibtex BookTemplate
   xelatex BookTemplate.tex
   xelatex BookTemplate.tex
   ```

## Related Resources

- **AMD ROCm Official Documentation**: https://docs.amd.com
- **HIP Open Source Project**: https://github.com/ROCm/HIP
- **Example Code**: https://gitlab.com/syifan/hipbookexample
- **ROCm Platform**: https://rocm.docs.amd.com

## License

This project follows the license terms of the original book. Please refer to the license information of the original publication.

## Contributing

Suggestions for translation quality improvements or error reports are welcome. Please contribute by:

1. Creating Issues to report problems
2. Submitting Pull Requests to improve translations
3. Providing technical suggestions or corrections

## Contact

For any questions or suggestions, please contact us through GitHub Issues.

---

**Note**: This project is for educational purposes, aiming to promote learning and dissemination of HIP programming technology.
