# Catatan Jaringan - Belajar di rish + Termux

## DNS
- Control D Unfiltered: 76.76.2.0 / 76.76.10.0
- Private DNS: p0.freedns.controld.com
- Cara nyalain: settings put global private_dns_mode hostname

## Ping
- Ping ke DNS Control D: 16ms (deket, Singapura)
- Ping ke server HAGO tanpa WARP: 375ms (rute muter lewat Marseille -> Paris -> Frankfurt -> China)
- Ping ke server HAGO pake WARP: 208ms (rute langsung Singapura -> Hong Kong -> China, turun 44%)

## Traceroute
- Hop 1: 192.168.1.1 (router)
- Hop 7: Singapura 10ms
- Hop 8: Marseille 168ms <- penjahatnya, rute muter Eropa
- Hop 13+: China 350ms+

## Pelajaran
- Ping itu ke server, bukan ke HP orang lain
- Traceroute * * * = server nge-block ICMP, bukan putus
- Control D = buku telepon (DNS), WARP = jalan tol (rute), beda kerjaan
