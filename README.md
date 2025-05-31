import cv2

# Carrega a imagem em cores
imagem = cv2.imread('caminho/para/sua/imagem.jpg', cv2.IMREAD_COLOR)

# Verifica se a imagem foi carregada com sucesso
if imagem is None:
    print('Erro ao carregar a imagem.')
else:
    # Exibe a imagem em uma janela
    cv2.imshow('Imagem', imagem)
    
  # Aguarda o pressionamento de uma tecla
  cv2.waitKey(0)
    
  # Fecha todas as janelas
  cv2.destroyAllWindows()

  # Salva a imagem em um novo arquivo (opcional)
  cv2.imwrite('imagem_salva.jpg', imagem)
