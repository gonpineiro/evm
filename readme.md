ts-node src 0x60FF60AA0160FC60016001


#### Ejemplo de operaciones:

`yarn  pvm --code 0x60FF60AA0160FC600c020a --gasLimit 10000`

- Agrega 0xff al Stack: PUSH (0x60) 0xff
- Agrega 0xaa al Stack: PUSH (0x60) 0xaa
- Suma los ultimos dos valores del Stack: ADD (0x01) 0xff + 0xaa = 0x01a9

- Queda unicamente el Stack:   ['0x01a9']

- Agrega 0xfc al Stack: PUSH (0x60) 0xfc
- Agrega 0x0c al Stack: PUSH (0x60) 0x0c
- Multiplico los ultimos dos valores del Stack: MUL (0x02) 0xfc + 0x0c = 0x0bd0

- Queda unicamente el Stack:    ['0x01a9', '0x0bd0']

- Suma los ultimos dos valores del Stack: ADD (0x01) 0x01a9 + 0x0bd0 = 0x0d79


`yarn pvm --code 0x600A6000525B600660005160019003806000526000109057 --gasLimit 10000`