import random
lista = ["pedra","spock","papel","lagarto","tesoura"]
placar_pc = 0
placar_usuario = 0
while placar_pc <3 and placar_usuario <3: 
      computador = random.choice(lista)    
      jogo = input("Escolha uma opção para jogar: pedra; Spock; Papel; lagarto; tesoura:  ")
      print("computador jogou:"+computador)
      print ("jogador escolheu:"+jogo) 
      if jogo == lista[0]:
          if computador == lista[1] or computador == lista[2]:
              placar_pc +=1
              placar_usuario == 0
              print("Computador venceu!")
          elif computador == lista[3] or computador == lista[4]:
              placar_usuario +=1
              placar_pc == 0
              print ("Jogador venceu!")    
          elif computador == jogo: 
              print("empate")
         
 
      if jogo == lista[1]:
          if computador == lista[2] or computador == lista[3]:
              placar_pc +=1
              placar_usuario == 0
              print("Computador venceu!")
          elif computador == lista[0] or computador == lista[4]:
              placar_usuario +=1
              placar_pc == 0
              print ("Jogador venceu!")    
          elif computador == jogo: 
              print("empate")
         
      if jogo == lista[2]:
          if computador == lista[3] or computador == lista[4]:
              placar_pc +=1
              placar_usuario == 0
              print("Computador venceu!")
          elif computador == lista[0] or computador == lista[1]:
              placar_usuario +=1
              placar_pc == 0
              print ("Jogador venceu!")    
          elif computador == jogo: 
              print("empate")
          
        
      if jogo == lista[3]:
          if computador == lista[0] or computador == lista[4]:
              placar_pc +=1
              placar_usuario == 0
              print("Computador venceu!")
          elif computador == lista[1] or computador == lista[2]:
              placar_usuario +=1
              placar_pc == 0
              print ("Jogador venceu!")    
          elif computador == jogo: 
              print("empate")
             
        
      if jogo == lista[4]:
          if computador == lista[0] or computador == lista[1]:
              placar_pc +=1
              placar_usuario == 0
              print("Computador venceu!")
          elif computador == lista[2] or computador == lista[3]: 
              placar_usuario +=1
              placar_pc == 0
              print ("Jogador venceu!")    
          elif computador == jogo: 
              print("empate")
            
      if placar_pc == 3: 
          print("O computador ganhou!")
      elif placar_usuario == 3:
             print("O jogador ganhou!")  
