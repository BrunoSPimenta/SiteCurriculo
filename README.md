# SiteCuriculo
Site pessoal que serve para curriculo e para mostrar trabalho em css e html



BG: background: linear-gradient( #0157ff, #1b9fbc, #390c78);

COLOR BOX: background: linear-gradient(90deg, #971ab4, #974dff, #4e00ba);


FLIP BOX

.box{ /* Caixa com flip */
    /* background: linear-gradient( 90deg, #831ab4, #8233ee, #5206bc); */
    /* background: linear-gradient(90deg, #971ab4, #974dff, #4e00ba); */
    border: 1px solid black;
    border-radius: 100%;
    height: 400px;
    width: 400px;
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
    box-shadow: 4px 4px black;
}


/* Efeitos de carta */

.card .box{
    transition: transform 0.9s;
    transform-style: preserve-3d;
}

.card:hover .box{
    transform: rotateY(180deg);
}

.frente, .tras{
    position: absolute;
    backface-visibility: hidden;
}

.tras {
    transform: rotateY(180deg);
}

.frente , .tras{
    border-radius: 12px;
    box-shadow: 0 0 8px 0 rgba(0, 0, 0, .3)
}
