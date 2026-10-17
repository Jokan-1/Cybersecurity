# What i learn? 
**Comands**:
- ifconfig: mostra o endereço físico e lógico do hardware
- netstat (ss -lntp): mostra se há serviços de rede conectado ao pc (e especificações dos serviços)
- /etc/init.d/networking restart: reinicia o sistema de rede
- ifconfig eth0 [ip] [netmask] : redefine o ip do sistema
- route -n: mostra a configuração geral da rede (gateway, ip)
- nano /etc/network/interfaces: permite alterar a configuração de rede do sistema

Theory:
A configuração de rede do sistema pode variar entre dois fatores, o primeiro é conhecido como dhcp, na qual o sistema busca automaticamente um endereço IP dinâmico e se conecta na rede, o segundo, é o static, na qual você manualmente determina o endereço IP, o gateway e a netmask que o sistema irá utilizar para navegar na rede. Para acessar a segunda opção, você precisa ir em nano /etc/network/interface e especificar cada objeto para o funcionamento:

Exemplo de configuração estática:

auto eth0
iface eth0 inet static
address: 10.0.2.23
netmask 255.255.255.0
gateway 10.0.2.0
