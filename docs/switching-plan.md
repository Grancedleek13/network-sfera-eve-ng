# План коммутации

## Коммутатор SW1

- e0/1 — access, VLAN10 — подключён PC1 (eth0)
- e0/2 — access, VLAN20 — подключён PC2 (eth0)
- e0/3 — access, VLAN30 — подключён WEB-SRV (e0/0)
- e0/0 — trunk, VLANs 10,20,30 — подключён к Router e0/0

## Router

- e0/0 — dot1q trunk к SW1 e0/0, подинтерфейсы 10/20/30
- e0/2 — линк к ISP e0/0 (WAN)

## ISP

- e0/0 — линк к Router e0/2
