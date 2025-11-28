## Network conceptos
---
- LAN: Local Area Network (red local/personal en la que tienen control total). Tienes ancho de banda alto y barato. Tú eres el dueño de los cables. ^a80a01

- WAN: Wide Area Network. El ancho de banda es más costoso y limitado. **Importante:** Usas la infraestructura de un **ISP (Proveedor de Servicios)**. No eres dueño del cable que cruza la ciudad.

- Node: Cualquier "caja" en la red. Un Switch, un Router, un AP.

- Host: Dispositivo final que tiene una dirección IP y ejecuta aplicaciones de usuario. (PC, Móvil, Impresora).

- DNA center: Digital Network Architecture punto de gestión centralizado para todos los dispositivos que conforma una red. Proporciona una plataforma para automatizar y analizar tu red basada en la intención. Tiene la capacidad de gestionar gran cantidad de switches desde un único punto. Ademas, puedes actualizar todos los dispositivos de la red desde un único punto. DNA Center es el "cerebro" en una red definida por software (SDN) para entornos empresariales (Campus). No solo configura, sino que _vigila_ la salud de la red usando IA/Machine Learning.

- ACL: Acces Control List. Lista de reglas que permiten o bloquean trafico en un router o switch segun varios criterios (IPs, Protocolo, Puerto...). Funciona como un colador. Mira el paquete, mira la lista, y decide. **Implicit Deny (Denegación Implícita):** Al final de todas las listas ACL hay una regla invisible que dice "Denegar todo lo demás". Si no permites algo explícitamente, la ACL lo mata al final. ^4dadad