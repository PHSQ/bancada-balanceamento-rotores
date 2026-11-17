# Bancada de balanceamento de rotores

## Baixar e executar

Baixe o [quatro_corridas.py](python/quatro_corridas.py) pelo botão **Download** do GitHub. Salve o arquivo em uma nova pasta. No terminal, abra a pasta que contém o arquivo e execute:

```powershell
python quatro_corridas.py
```

Se faltarem as bibliotecas, instale uma vez com `python -m pip install numpy pyserial matplotlib`. Siga as instruções do próprio programa para realizar o ensaio.

## Controlador de velocidade

[Manual em português, com foto do painel](manual-controlador.md).

Para ligar na bancada, **pressione o botão giratório prateado (RUN/STOP) e depois ligue a chavinha**.

## Se o programa não conectar

O Arduino pode estar em outra porta COM. No Windows, confira em **Gerenciador de Dispositivos → Portas (COM e LPT)**.

No início de `quatro_corridas.py`, troque `"COM3"` pela porta que aparece no seu computador. Se aparecer **COM5**, deixe assim:

```python
PORTA_SERIAL = "COM5"
```

## Recomendações práticas e condições com bons resultados

- **Parafusos.** Ajuste, com o rotor parado, o aperto das [cantoneiras que unem os pés à estrutura](imagens/cantoneiras.png), mantendo a bancada firme. Nos ensaios, houve bons resultados com os parafusos próximos ao motor levemente apertados e os próximos ao acelerômetro totalmente folgados, ou com os parafusos de todas essas cantoneiras bem folgados.
- **Rotação.** Houve bons resultados entre **640 e 950 RPM**, mesmo com pequenas variações entre leituras.
- **Massas.** Houve bons resultados com **10 g de desbalanceamento** e **7,6 g de teste**. Use a mesma massa de teste nas três posições. Para comparar outras massas, velocidades ou ajustes de aperto, comece outro ensaio.
