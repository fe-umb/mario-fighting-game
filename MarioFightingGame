heroi(mario,100). %HP do herói Mario.
heroi(luigi,150). %HP do herói Luigi.
heroi(peach,120). %HP da heroina Peach.

vilao(goomba,15). %HP do vilão Goomba.
vilao(spike,40). %HP do vilão Spike.
vilao(piranhaplant,30). %HP do vilão Piranha Plant.

ataque(mario,25). %Ataque do herói Mario.
ataque(luigi,15). %Ataque do herói Luigi.
ataque(peach,20). %Ataque da heroína Peach.
ataque(goomba,30). %Ataque do vilão Goomba.
ataque(spike,50). %Ataque do vilão Spike.
ataque(piranhaplant,40). %Ataque do vilão Piranha Plant.

maisforte(Personagem1,Personagem2):- %Verifica se Personagem1 é mais forte que o Personagem2.
    ataque(Personagem1,Atk1),
    ataque(Personagem2,Atk2),
    Atk1>Atk2.

derrotado(Heroi,Vilao):- %Verifica se o herói consegue derrotar o vilão com um único ataque.
    ataque(Heroi,Atk),
    vilao(Vilao,Hp),
    Atk>=Hp.

combate(Heroi,Vilao,X,Y):- %Retorna X (HP do herói) e Y (HP do vilão) após um turno de combate.
    ataque(Heroi,Atk),
    ataque(Vilao,Atk2),
    heroi(Heroi,Hp),
    vilao(Vilao,Hp2),
    X is Hp-Atk2,
    Y is Hp2-Atk.