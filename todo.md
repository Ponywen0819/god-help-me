  🟡 建議優化

  6. 章節篇幅落差

  ch1=45, ch2=44, ch3=523, ch4=632, ch5=58 行。ch2 我們剛剛精簡得乾淨，但若觀感上想再加深度，可在
  §2.4 補上「fragment reconnection paradigm 於道路網/血管網之 prior
  art」這個我先前提過的中優先建議（Mosinska 2018 等）。不加也 OK——methods-heavy 碩論這比例正常。

  7. ch3 演算法 alg:ael 第 8 步交代不足

  Skeletonize(Dilate(DrawPaths(G_mst), r_d) ∪ A)

  把膨脹、聯集、細化三件事壓在一行，讀者必須回 §3.5
  才能展開。建議：拆成兩步寫，或在演算法後加一個「展開細節見 §3.5」的脚注。

  9. ch4 §4.7.4「敏感度與可遷移性」與 §4.3 結論衝突

  §4.3 line 345 結論說「前處理階段五個參數變動幅度皆小、$\tau$ 影響最劇」；§4.7.4 line 632
  卻說「校正 $\sigma$ 之範圍以及 $\tau$」——把 $\sigma$ 提到與 $\tau$ 同等地位，但 §4.3
  並沒有支持這個強敘述。建議將 §4.7.4 改為「主要校正 $\tau$，$\sigma$
  須符合纖維像素寬度」以與實驗結論對齊。

  11. fig:dataset-inputs 用 minipage 不用 subfigure

  ch4 §4.1 的資料示意圖（fig 4.1）使用 \begin{minipage} + 手動 (a)(b)(c)(d)(e) 標籤而非
  \begin{subfigure}，失去自動編號與 \subref{} 引用一致性。其他圖（如 fig:enhance、fig:bs）都用
  subfigure。建議統一——除非有特殊版面需求否則改 subfigure。

