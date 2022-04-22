# TP_Hechiceros

module Library where
import PdePreludat

doble::Number->Number
doble numero = numero + numero
--Jujitsu Haskell

data Hechicero= Hechicero{
    nombre::String,
    antiguedad::Number,
    clan::String,
    grado::Number
}deriving (Show)
nobara= Hechicero{nombre="Nobara",antiguedad=1,clan="Kugisaki",grado=3}
satoru= Hechicero{nombre="Satoru",antiguedad=15,clan="Gojo",grado=0}
maki= Hechicero{nombre="Maki",antiguedad=3,clan="Zenin",grado=4}
yuji= Hechicero{nombre="Yuji",antiguedad=0,clan="Itadori", grado=1}

tieneExperiencia::Hechicero->Bool
tieneExperiencia Hechicero= antiguedad Hechicero>1

equipo1=[nobara,satoru,yuji]

equipoListo::[Hechicero]->Bool
equipoListo equipo=length equipo >3

subirGrado persona | grado persona >0 = 
