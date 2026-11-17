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
