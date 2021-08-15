# awesome-5g-omni

- 作成方針
  - 日本語で各種OSSやツール類の特徴・解説（使い方含）・簡易比較結果をまとめていきたい
  - ターゲット：
    - これからモバイルネットワークのOSSを開発しようとする開発者
    - これからモバイルネットワークのOSSを利用するユーザ
    - 既にOMNIに参加するメンバのノウハウ集
       - コンテンツの分類や、どこまで記載するか悩ましいですが、まずは記載してみて、少しづつ整理しながらコンテンツとして育てていければと考えています

- 参考：https://github.com/calee0219/awesome-5g

## Contents
- [RAN](#RAN)
- [Core Network](#Core-Network)
- [SIM](#SIM)
- [UE/CPE](#UE/CPE)
- [Tools](#Tools)

## RAN
- [OAI-RAN](https://gitlab.eurecom.fr/oai/openairinterface5g/)
  - OpenAirInterface　Software Alliance(OSA)が提供する3GPPプロトコルに準拠した無線アクセスネットワーク系（eNB/gNB/UE）のソフトウェア
  - 3GPP仕様に則り開発されているため、リファレンスコードとしても利用される
  
- [UERANSIM](https://github.com/aligungr/UERANSIM) 
  - オープンソースの5G端末（UE）や無線アクセスネットワーク（RAN）を実装

## Core Network
- [free5GC](https://github.com/free5gc/free5gc)
  - 3GPP Realse15に準拠したオープンソースソフトウェアの5Gコアであり、StandAlone（SA）構成に対応
  - 様々なネットワークファンクションを実装（NRF/AMF/AUSF/SMF/PCF/UDM/UDR/NSSF/UPF/N3IWF）
  - コミュニティの動きも活発で、「[free5GC forum](https://forum.free5gc.org/)」も存在
  
- [Open5GS](https://github.com/open5gs/open5gs) 
  - C言語で実装された、オープンソースソフトウェアの5Gコア及びEPC
  - 3GPP Realse16に準拠し、StandAlone（SA）構成に対応

- [OAI-CN](https://gitlab.eurecom.fr/oai/cn5g) 
  - OpenAirInterface　Software Alliance(OSA)が提供する3GPPプロトコルに準拠したコアネットワーク系（EPC and 5G）のソフトウェア
  - 3GPP仕様に則り開発されているため、リファレンスコードとしても利用される

- [magma](https://github.com/magma) 
  - 新興国にコネクティビティを届けることを目的に開発が始まったOSS。EPCの機能(A-GW)だけではなく集中管理機能(Orchestrator)やMNOとの連携機能(F-GW)を有する。
  - 5Gコアについては、Telecom Infra Projectと連携して最小構成版Minimum Viable Core(MVC版)を開発中。


## SIM
- [pysim](https://github.com/osmocom/pysim)

## UE/CPE
- [my5G-non3GPP-access ](https://github.com/my5G/my5G-non3GPP-access)

## Tools
- [speX](https://github.com/CoRfr/spex-3gpp) 
  - A WebService to deliver 3GPP specifications.
