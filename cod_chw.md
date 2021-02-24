# GroupCHW
Repositório criado para fazermos o trabalho de Linguagem de Programação pedido pela professora Elisângela Bibá.

#IFRO
#2º DE INFORMÁTICA MATUTINO
#Caroliny De Matos Chaves, Helen Vitória S Fraça e Walleri Vitória P Chaves
#POO
#USO DO TRY E EXCEPT LINHAS: 17, 157, 163, 177, 217, 225, 233, 292, 299 e etc...
#USO DO RAISE LINHA: 316
import os
import random
import time

class Endereço:
  def __init__(self):
    self.RuaCliente=str(input('Digite o nome da rua: '))
    self.BairroCliente=str(input('Digite so nome do bairro: '))
    while True:
      try:
        self.NumeroCasa=int(input('Digite o número da casa: '))
        break
      except:
        os.system('clear')
        print('Digite um valor númerico')
        continue
    self.Complemento=str(input('Digite o complemento: '))
  def VerificarEndereço(self):
    print('Bairro:', self.BairroCliente, '\nRua:',self.RuaCliente,'   Número:',self.NumeroCasa,'\nComplemento:',self.Complemento,'\n')
 
class Pedido:#6 metodos
  def __init__(self):
    self.Valor=None
    self.TaxaEntrega=None
    self.QuantidadeItens=[]
    self.AddCupom=None
    self.FormaPag=None
  def RegistrarPedido(self):
    while True:
      print('Produtos disponíveis:\n1-Banana\n2-Brigadeiro \n3-Romeu e Julieta\n\n4-Calabresa\n5-Portuguesa\n6-Quatro Queijos\n\n7-Voltar')
      a = input('Digite um número: ')
      if a== '1':
        os.system('clear')
        print('DescriçãoProduto:', banana.DescricaoProduto, '\nUnidades:',banana.Unidades,'\nNomeProduto:',banana.NomeProduto,'\nCategoriaProd:',banana.CategoriaProd,'\nCódigoProduto:',banana.CodigoProduto,'\nSabor:',banana.Sabor,'\nTamanho:',banana.Tamanho,'\nQntSabores:', banana.QntSabores)
        print('Deseja Confirmar pedido?\n1-Sim\n2-Voltar')
        a = input('Digite um número: ')
        if a== '1':
          self.QuantidadeItens.append(banana)
          os.system('clear')
          self.ConfirmarPedido()
        elif a== '2':
          os.system('clear')
          self.RegistrarPedido()
        else:
          os.system('clear')
          print ('ERRO. TENTE NOVAMENTE')
          self.RegistrarPedido()
        break
      elif a== '2':
        os.system('clear')
        print('DescriçãoProduto:', morango.DescricaoProduto, '\nUnidades:',morango.Unidades,'\nNomeProduto:',morango.NomeProduto,'\nCategoriaProd:',morango.CategoriaProd,'\nCódigoProduto:',morango.CodigoProduto,'\nSabor:',morango.Sabor,'\nTamanho:',morango.Tamanho,'\nQntSabores:', morango.QntSabores)
        print('Deseja Confirmar pedido?\n1-Sim\n2-Voltar')
        a = input('Digite um número: ')
        if a== '1':
          self.QuantidadeItens.append(morango)
          os.system('clear')
          self.ConfirmarPedido()
        elif a== '2':
          os.system('clear')
          self.RegistrarPedido()
        else:
          os.system('clear')
          print ('ERRO. TENTE NOVAMENTE')
          self.RegistrarPedido()
        break
      elif a== '3':
        os.system('clear')
        print('DescriçãoProduto:', romeu.DescricaoProduto, '\nUnidades:',romeu.Unidades,'\nNomeProduto:',romeu.NomeProduto,'\nCategoriaProd:',romeu.CategoriaProd,'\nCódigoProduto:',romeu.CodigoProduto,'\nSabor:',romeu.Sabor,'\nTamanho:',romeu.Tamanho,'\nQntSabores:', romeu.QntSabores)
        print('Deseja Confirmar pedido?\n1-Sim\n2-Voltar')
        a = input('Digite um número: ')
        if a== '1':
          self.QuantidadeItens.append(romeu)
          os.system('clear')
          self.ConfirmarPedido()
        elif a== '2':
          os.system('clear')
          self.RegistrarPedido()
        else:
          os.system('clear')
          print ('ERRO. TENTE NOVAMENTE')
          self.RegistrarPedido()
        break
      elif a== '5':
        os.system('clear')
        print('DescriçãoProduto:', portuguesa.DescricaoProduto, '\nUnidades:',portuguesa.Unidades,'\nNomeProduto:',portuguesa.NomeProduto,'\nCategoriaProd:',portuguesa.CategoriaProd,'\nCódigoProduto:',portuguesa.CodigoProduto,'\nSabor:',portuguesa.Sabor,'\nTamanho:',portuguesa.Tamanho,'\nQntSabores:', portuguesa.QntSabores)
        print('Deseja Confirmar pedido?\n1-Sim\n2-Voltar')
        a = input('Digite um número: ')
        if a== '1':
          self.QuantidadeItens.append(portuguesa)
          os.system('clear')
          self.ConfirmarPedido()
        elif a== '2':
          os.system('clear')
          self.RegistrarPedido()
        else:
          os.system('clear')
          print ('ERRO. TENTE NOVAMENTE')
          self.RegistrarPedido()
        break
      elif a== '4':
        os.system('clear')
        print('DescriçãoProduto:', calabresa.DescricaoProduto, '\nUnidades:',calabresa.Unidades,'\nNomeProduto:',calabresa.NomeProduto,'\nCategoriaProd:',calabresa.CategoriaProd,'\nCódigoProduto:',calabresa.CodigoProduto,'\nSabor:',calabresa.Sabor,'\nTamanho:',calabresa.Tamanho,'\nQntSabores:', calabresa.QntSabores)
        print('Deseja Confirmar pedido?\n1-Sim\n2-Voltar')
        a = input('Digite um número: ')
        if a== '1':
          self.QuantidadeItens.append(calabresa)
          os.system('clear')
          self.ConfirmarPedido()
        elif a== '2':
          os.system('clear')
          self.RegistrarPedido()
        else:
          os.system('clear')
          print ('ERRO. TENTE NOVAMENTE')
          self.RegistrarPedido()
        break  
      elif a== '6':
        os.system('clear')
        print('DescriçãoProduto:', queijos.DescricaoProduto, '\nUnidades:',queijos.Unidades,'\nNomeProduto:',queijos.NomeProduto,'\nCategoriaProd:',queijos.CategoriaProd,'\nCódigoProduto:',queijos.CodigoProduto,'\nSabor:',queijos.Sabor,'\nTamanho:',queijos.Tamanho,'\nQntSabores:', queijos.QntSabores)
        print('Deseja Confirmar pedido?\n1-Sim\n2-Voltar')
        a = input('Digite um número: ')
        if a== '1':
          self.QuantidadeItens.append(queijos)
          os.system('clear')
          self.ConfirmarPedido()
        elif a== '2':
          os.system('clear')
          self.RegistrarPedido()
        else:
          os.system('clear')
          print ('ERRO. TENTE NOVAMENTE')
          self.RegistrarPedido()
        break 
      elif a=='7':
        os.system('clear')
        cliente.ver_menu()
      else:
        os.system('clear')
        print ('ERRO. TENTE NOVAMENTE')
        continue
  def ConfirmarPedido(self):
    while True:
      print('1-Fazer outro pedido\n2-encerar compras e solicitar entregar\n3-Ver pedidos\n4-Excluir pedido do Carrinho')
      a = input('Digite um número: ')
      if a== '1':
        os.system('clear')
        self.RegistrarPedido()
      elif a=='3':
        os.system('clear')
        try:
          Pizza_Doce.ConsultaProduto(self)
        except:
          print('Infelizmente tivemos um problema ao exibir seus pedidos')
      elif a=='4':
        os.system('clear')
        try:
          Pizza_Doce.ExcluiProduto(self)
        except:
          print('Infelizmente tivemos um problema ao exibir seus pedidos')
      elif a=='2':
        os.system('clear')
        self.FinalizarPedido()
      else:
        os.system('clear')
        print ('ERRO. TENTE NOVAMENTE')
        continue
  def troco(self):
    pass
  def FinalizarPedido(self):
    try:
      print('-------Produtos no Carrinho:-------')
      for x in range(len(pedido.QuantidadeItens)):
        print('Nome do Produto:',pedido.QuantidadeItens[x].NomeProduto)
      print('-------Endereço:-------')
      endereço_cliente.VerificarEndereço()
      print('-------Dados do cliente:-------')
      cliente.AlterarConta()
      print('Valor da compra: R$',len(pedido.QuantidadeItens)*30)
      while True:
        print('Confirmar Pedido\n1-Sim\n2-Não')
        a = input('Digite um número: ')
        if a== '1':
          os.system('clear')
          print('O pedido esta sendo enviado para o endereço informado, aguarde...')
          time.sleep(10)
          self.QuantidadeItens=[]
          os.system('clear')
          cliente.ver_menu()
        elif a=='2':
          os.system('clear')
          cliente.ver_menu()
        else:
          os.system('clear')
          print ('ERRO. TENTE NOVAMENTE')
          continue
    except:
      print('Infelizmente tivemos um problema')
  def EntregarPedido(self):
    pass
  def Retirar_restaurante(self):
    pass

class Cliente:
  def __init__(self):
    self.CadastroCliente=str(random.randrange(1000,9999))
    self.Nome=str(input('Digite seu nome nome: '))
    self.Sobrenome=str(input('Digite seu sobrenome nome: '))
    self.Email=str(input('Digite seu Email: '))
    while True:
      try:
        self.CPF=int(input('Digite seu CPF: '))
        break
      except:
        os.system('clear')
        print('Digite um valor númerico')
        continue
    while True:
      try:
        self.DataNascimento=int(input('Digite sua data de nascimento: '))
        break
      except:
        os.system('clear')
        print('Digite um valor númerico')
        continue
    while True:
      try:
        self.Telefone=int(input('Digite seu Telefone: '))
        break
      except:
        os.system('clear')
        print('Digite um valor númerico')
        continue    
  def ver_menu(self):
    while True:
      print('Menu Principal\n1-Fazer Pedido\n2-Ver endereço\n3-Ver perfil')
      a = input('Digite um número: ')
      if a== '1':
        os.system('clear')
        pedido.RegistrarPedido()
        break
      elif a== '2':
        os.system('clear')
        endereço_cliente.VerificarEndereço()
      elif a== '3':
        os.system('clear')
        self.AlterarConta()
       
      else:
        os.system('clear')
        print ('ERRO. TENTE NOVAMENTE')
        continue
  def AlterarConta(self):
    print('Nome:', self.Nome+' '+self.Sobrenome,'\nCadastro Cliente:',self.CadastroCliente,'\nEmail:',self.Email,'\nTelefone:',self.Telefone,'\nCódigoProduto:')
    self.ConsultarCPF()
    self.ConsultarDataNascimento()
  def ConsultarCPF(self):
    print('CPF:', self.CPF)
  def ConsultarDataNascimento(self):
    print('Data de nascimento:',self.DataNascimento)

class Empresa:
  def __init__(self):
    self.CNPJ=None
    self.NomeEmpresa=None
    self.EmailEmpresa=None
    self.Telefone=None
    self.SiteEmpresa=None
    self.EndereçoEmp=None
  def RegistroEmpresa(self):
    pass
  def ConsultarEmp(self):
    pass

class Produtos:#metodos
  def __init__(self,DescricaoProduto,Unidades,NomeProduto,CategoriaProd, CodigoProduto): # Atributos
    self.DescricaoProduto=DescricaoProduto
    self.Unidades=Unidades
    self.NomeProduto=NomeProduto
    self.CategoriaProd=CategoriaProd
    self.CodigoProduto=CodigoProduto
  def CadastroProduto(self): # metodos
    
      os.system('clear')
  def ConsultaProduto(self): # metodos
    try:
      for x in range(len(pedido.QuantidadeItens)):
        print('Descrição do Produto:', pedido.QuantidadeItens[x].DescricaoProduto, '\nUnidades:',pedido.QuantidadeItens[x].Unidades,'\nNome do Produto:',pedido.QuantidadeItens[x].NomeProduto,'\nCategoria:',pedido.QuantidadeItens[x].CategoriaProd,'\nCódigo do Produto:',pedido.QuantidadeItens[x].CodigoProduto,'\nSabor:',pedido.QuantidadeItens[x].Sabor,'\nTamanho:',pedido.QuantidadeItens[x].Tamanho,'\nQuantidades de Sabores:', pedido.QuantidadeItens[x].QntSabores)
        print('-----------------------------------------------')
    except:
      raise
  def ExcluiProduto(self): # metodos
    try:
      for x in range(len(pedido.QuantidadeItens)):
        print('------------------Pedido',x+1,'----------------------')
        print('Descrição do Produto:', pedido.QuantidadeItens[x].DescricaoProduto, '\nUnidades:',pedido.QuantidadeItens[x].Unidades,'\nNome do Produto:',pedido.QuantidadeItens[x].NomeProduto,'\nCategoria:',pedido.QuantidadeItens[x].CategoriaProd,'\nCódigo do Produto:',pedido.QuantidadeItens[x].CodigoProduto,'\nSabor:',pedido.QuantidadeItens[x].Sabor,'\nTamanho:',pedido.QuantidadeItens[x].Tamanho,'\nQuantidades de Sabores:', pedido.QuantidadeItens[x].QntSabores)
      while True:
        a = input('Digite um número do pedido que você deseja excluir: ')
        if int(a)>len(pedido.QuantidadeItens):
          os.system('clear')
          print('Pedido não encontrado\nTente novamente')
          Pizza_Doce.ExcluiProduto(self)
          break
        else:
          os.system('clear')
          pedido.QuantidadeItens.pop(int(a)-1)
          break
    except:
      raise
         
class Pizza_Doce(Produtos):#1 metodo
  def __init__(self,Sabor,Tamanho,QntSabores,DescricaoProduto,Unidades,NomeProduto,CategoriaProd, CodigoProduto):
    self.Sabor=Sabor
    self.Tamanho=Tamanho
    self.QntSabores=QntSabores
    self.Unidades=Unidades
    self.NomeProduto=NomeProduto
    super().__init__(DescricaoProduto,Unidades,NomeProduto,CategoriaProd, CodigoProduto)
  def ExcluiProduto(self): # metodos
    pass

class Pizza_Salgada(Produtos):#1 metodo
  def __init__(self,Sabor,Tamanho,QntSabores,DescriçaoProduto,Unidades,NomeProduto,CategoriaProd, CodigoProduto):
    self.Sabor=Sabor
    self.Tamanho=Tamanho
    self.QntSabores=QntSabores
    self.Unidades=Unidades
    self.NomeProduto=NomeProduto
    super().__init__(DescriçaoProduto,Unidades,NomeProduto,CategoriaProd, CodigoProduto)
  def ExcluiProduto(self): # metodos
    pass

banana = Pizza_Doce('Chocolate com banana', 'G', 2, 'Pizza de Banana com Chocolate', 1, 'Pizza de Banana com Chocolate', 'Doce','123456')
morango = Pizza_Doce('Brigadeiro com Morango', 'M', 2, 'Pizza de Brigadeiro com Morango', 1, 'Pizza de Brigadeiro com Morango', 'Doce','123451')
romeu = Pizza_Doce('Romeu e Julieta', 'GG', 1, 'Pizza Romeu e Julieta', 1, 'Pizza Romeu e Julieta', 'Doce','123459')
portuguesa = Pizza_Salgada('Portuguesa', 'P', 1, 'Pizza Portuguesa', 1, 'Pizza Portuguesa', 'salgada','123453')
calabresa = Pizza_Salgada('Calabresa', 'M', 1, 'Pizza de Calabresa', 1, 'Pizza de Calabresa', 'Salgada','123457')
queijos = Pizza_Salgada('Quatro Queijos', 'GG', 1, 'Pizza Quatro Queijos', 1, 'Pizza Quatro Queijos', 'Salgada','123410')

pedido=Pedido()
cliente=Cliente()
endereço_cliente=Endereço()
os.system('clear')
cliente.ver_menu()
