# Comandos-para-Switch

#Para sair do modo usuário e entrar como administrador no Switch escrever no prompt comando:

#Enable
  #(O # quer dizer que já entrou como ADM)

#Para entrar na configuração:
  Dar um CONF TAB TER TAB (Configuração do Terminal)

#(colocar o nome do switch) hostname SW1
  #Acessar e criar VLAN
    vlan 10
      #Colocar o nome da VLAN
        name ADM

#Acessar outra VLAN
  vlan 20
    name EDU
      #Separação das portas VLANS 1/12
        interface range f0/1-f0/12
          switchport access vlan 10

          #Separação das VLANS 13/24
        interface range fa0/13-fa0/24 
      switchport access vlan 20
    #Interligar Switch
  int gi0/1 
#Modo trunk
  switchport mode trunk 
    switchport trunk allowed vlan 10 
      switchport trunk allowed vlan add 20 
        end

            #WR PARA SALVAR
            
