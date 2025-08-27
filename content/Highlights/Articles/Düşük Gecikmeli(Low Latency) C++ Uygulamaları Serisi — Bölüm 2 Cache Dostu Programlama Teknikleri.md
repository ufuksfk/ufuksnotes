---
draft: true
description:
socialDescription:
title: Düşük Gecikmeli(Low Latency) C++ Uygulamaları Serisi — Bölüm 2 Cache Dostu Programlama Teknikleri
tags:
  - highlight/articles
date: 2025-08-18
modified: 2025-08-21
---
author: [[Kemal Candan]]
url: https://medium.com/p/ec6ea4c4de66
last highlighted date: [[2025-W33#1]] 2025-08-11
published date: [[]]

## Highlights
- Cache dostu paradigmalar geliştirebilmek için için son olarak bahsetmek istediğim konsept ise AoS(Arrays of Structures) yerine SoA(Structures of Arrays) kullanılmasıdır. Verinin bellekte nasıl organize edildiği, cache kullanımını ve dolayısıyla işlem hızını belirler. Aşağıdaki benchmark testinde bu durumu ele alalım.
- Yaptığımız benchmark testinde, SoA yapısının AoS yapısına kıyasla belirgin şekilde daha hızlı olduğunu gözlemledik. Bunun temel sebebi, SoA’da aynı tip verilerin ardışık şekilde cache’te yer alması ve bu sayede cache satırlarının daha verimli kullanılmasıdır. AoS’da ise farklı türdeki veriler karışık şekilde saklandığından, cache etkinliği azalır, cache miss miktarı artar ve veri erişimi yavaşlar.
