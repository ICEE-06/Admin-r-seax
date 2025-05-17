
## Configuration:

![[Pasted image 20250513201211.png]]

- **Jaune**: RIP
- **Bleu**: OSPF
- **Violet**: EIGRP

## Configuration des routeurs

### RIP
- **Activation du routage dynamique**
    `#router rip`
- **Ajoutes des réseaux directement connectés**
	`#network 192.168.195.0`
	`#network 10.10.1.0`


### EIGRP
- **Activation du routage dynamique**
	`#router eigrp 10`
- **Ajouter les réseaux directement connectés**
	`#network 172.28.0.0 0.0.0.3`
	`#network 192.168.1.0 0.0.0.255`

### OSPF
- **Activation du routage dynamique**
	`#router ospf 10`
- **Ajouter les réseaux directement connectés**
	`#network 10.10.10.0 0.0.0.3 area 0`
	`#network 192.168.98.0 0.0.0.255 area 0`

## Configuration du Backbone

Le **backbone** sert de centre de distribution entre les protocoles
