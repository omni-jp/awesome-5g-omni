# awesome-5g-omni

- awesome 作成方針
  - 日本語で各種OSSやツール類の特徴・解説（使い方含）・簡易比較結果をまとめていきたい
  - ターゲット：
    - これからモバイルネットワークのOSSを開発しようとする開発者
    - これからモバイルネットワークのOSSを利用するユーザ
    - 既にOMNIに参加するメンバのノウハウ集
       - コンテンツの分類や、どこまで記載するか悩ましいですが、まずは記載してみて、少しづつ整理しながらコンテンツとして育てていければと考えています

- awesome 追加方法
  - GitHub上で文言追加し、PRしてください！

- 参考：https://github.com/calee0219/awesome-5g

## Contents
- [RAN](#ran)
- [Core Network](#core-network)
- [SIM](#sim)
- [UE/CPE](#ue/cpe)
- [Tools](#tools)

## RAN
- [OAI-RAN](https://gitlab.eurecom.fr/oai/openairinterface5g/)
  - OpenAirInterface Software Alliance(OSA)が提供する3GPPプロトコルに準拠した無線アクセスネットワーク系（eNB/gNB/UE）のソフトウェア
  - 3GPP仕様に則り開発されているため、リファレンスコードとしても利用される
  
- [UERANSIM](https://github.com/aligungr/UERANSIM) 
  - オープンソースの5G端末（UE）や無線アクセスネットワーク（RAN）を実装
  - 主にコアネットワークと接続するための上位レイヤーのプロトコル(NGAP,NASなど)が実装されている

- [5T for 5G](https://github.com/NVIDIA/5t5g)
  - DPDK ライブラリとして実装されている NVIDIA (Mellanox) Smart NIC 機能である [5T for 5G](https://developer.nvidia.com/blog/new-real-time-smartnic-technology-5t-for-5g/) の O-DU 向けの参照実装
  - 送信側の機能として、[MLX5 PMD](https://doc.dpdk.org/guides/nics/mlx5.html?highlight=tx_pp) として実装されている正確な時刻でのパケット送信スケジューリングが実装されている
  - 受信側の機能として、[DPDK flow steering rule](https://doc.dpdk.org/guides/linux_gsg/linux_drivers.html?highlight=bifurcated#bifurcated-driver) を用いて O-RAN U-plane パケットのみを GPU メモリ上の DPDK mempool に [GPUDirect RDMA](https://docs.nvidia.com/cuda/gpudirect-rdma/index.html) での高速転送が実装されている

- [Keysight's FREE Wireshark Protocol Analyzer with O-RAN WG4 CUS Decoding](https://connectlp.keysight.com/Open_RAN_Test_Solutions?elqTrackId=6DB5C2748D9C85098B282513331CEA32&elq=00000000000000000000000000000000&elqaid=4978&elqat=2&elqCampaignId=)
  - O-RAN C/U/S プレーンをデコードできるように変更された Wireshark
 
## Core Network
- [free5GC](https://github.com/free5gc/free5gc)
  - 3GPP Realse15に準拠したオープンソースソフトウェアの5Gコアであり、StandAlone（SA）構成に対応
  - 様々なネットワークファンクションを実装（NRF/AMF/AUSF/SMF/PCF/UDM/UDR/NSSF/UPF/N3IWF）
  - コミュニティの動きも活発で、「[free5GC forum](https://forum.free5gc.org/)」も存在
  
- [Open5GS](https://github.com/open5gs/open5gs) 
  - C言語で実装された、オープンソースソフトウェアの5Gコア及びEPC
  - 3GPP Realse16に準拠し、StandAlone（SA）構成に対応

- [OAI-CN](https://gitlab.eurecom.fr/oai/cn5g) 
  - OpenAirInterface Software Alliance(OSA)が提供する3GPPプロトコルに準拠したコアネットワーク系（EPC and 5G）のソフトウェア
  - 3GPP仕様に則り開発されているため、リファレンスコードとしても利用される

- [magma](https://github.com/magma) 
  - 新興国にコネクティビティを届けることを目的に開発が始まったOSS。EPCの機能(A-GW)だけではなく集中管理機能(Orchestrator)やMNOとの連携機能(F-GW)を有する。
  - 5Gコアについては、Telecom Infra Projectと連携して最小構成版Minimum Viable Core(MVC版)を開発中。


## SIM
- [pysim](https://github.com/osmocom/pysim)

## UE/CPE
- [my5G-non3GPP-access ](https://github.com/my5G/my5G-non3GPP-access)

## Tools
- [5g-trace-visualizer](https://github.com/telekom/5g-trace-visualizer) 
  - This set of Python scripts allow you to convert pcap, pcapng or pdml 5G protocol traces (Wireshark, tcpdump, ...) into SVG sequence diagrams.
- [speX](https://github.com/CoRfr/spex-3gpp) 
  - A WebService to deliver 3GPP specifications.
- [pycrate](https://github.com/P1sec/pycrate)
  - NGAP, RRC, F1APなどのASN.1で定義されているバイナリフォーマットやNASのエンコード・デコードライブラリ
