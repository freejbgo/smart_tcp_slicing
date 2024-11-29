# 更新说明
## 1.0 2024-11-29
Useage: `python3 geneva2.py -q 100 -w 1 -s 7 -c 7`

1. -w: window_size
2. -s: window_scale 
3. -c: 混淆次数，建议7次，减少此值可提速（0最快）


防火墙：

iptables -I OUTPUT -p tcp --sport 80 -j NFQUEUE --queue-num 100

