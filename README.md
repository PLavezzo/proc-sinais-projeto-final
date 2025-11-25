# Projeto Final - Processamento de Sinais

## Descrição
Projeto de filtros digitais para análise e decodificação de sinais DTMF contaminados com ruído da 9ª Sinfonia de Beethoven.

## Notebooks

1. **01_analise_inicial.ipynb** - Análise espectral do sinal com resolução de 10 Hz
2. **02_downsampling_antialiasing.ipynb** - Downsampling e filtro anti-aliasing IIR
3. **03_filtros_fir.ipynb** - Projeto de filtros FIR (Hamming, Kaiser, Blackman)
4. **04_analise_final_decodificacao.ipynb** - Análise final e decodificação DTMF

## Sequência Decodificada
**998116196** (após remoção da tecla 7)

## Requisitos
- Python 3.8+
- NumPy
- SciPy
- Matplotlib

## Como Usar

### Local
```bash
pip install numpy scipy matplotlib
jupyter notebook
```

### Google Colab
1. Faça upload do arquivo `dados_B.wav`
2. Execute os notebooks em ordem

## Especificações do Projeto
- Taxa de amostragem original: 80 kHz
- Taxa após downsampling: 8 kHz
- Filtro anti-aliasing: IIR Elíptico
- Filtros FIR: Hamming, Kaiser, Blackman
- Atenuação na banda de rejeição: ≥ 40 dB

## Autor
Projeto desenvolvido para a disciplina de Processamento de Sinais
