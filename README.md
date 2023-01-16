# Projeto-PHP
Projeto de Criação de Personagem
<?php
abstract class SerVivo{

         private $vivo;
         private $pontosdeVida;
         private $poderdeAtaque;
         private $superAtaque;
         private $fraqueza;
         private $maxPontosdeVida = 100;
         private $maxPontosdeAtaque = 30;

         function__construct(){
                $this->vivo = true;
                $this->pontosdeVida = rand(50,$this->maxPontosdeVida);
                $this->poderdeAtaque = rand(5,$this->maxPontosdeAtaque);
                $this->superAtaque = rand(0,$this->maxPontosdeAtaque);
                $this->fraqueza = rand(0,$this->maxPontosdeAtaque);

         }

         function getPontosdeVida(){
                 return $this->pontosdeVida;
         }
}

?>

<?php
//Herdando da classe Ser Vivo.
class Nascer extends Ser Vivo($nome, $nomedodono){
      
      public $nome;
      public $nomedodono;
      public $pontosdeVida;
      public $pontosdeFraqueza;
      public $poderMaximo

  $pontosdeVida[] = rand[0, 100];
  $pontosdeFraqueza[] = rand[4];
  $poderMaximo[] = rand[9];
  
  if($pontosdeVida == 100){
     echo 'está vivo';
  } elif($pontosdeVida >= 1){
      echo'está vivo';
  } else($pontosdeVida == 0) {
      echo'está morto';
  }
}
?>

<?php
//Herdando da classe Ser Vivo.
class Morrer extends Ser Vivo(){
      public fuction setpontos($pontosdeVida){
           $pontosdeVida = rand[0, 100];
           $frasedeDerrota[] = 'Fui Derrotado';
     }
         
      switch($pontosdeVida){
        case 0:
         echo 'está morto';
         break:
     }  
      if($pontosdeVida == 0){
         echo $frasedeDerrota <br>
     }
 }
?>

<?php
require('Ser Vivo.php');
require('Nascer.php');
require('Morrer.php');

echo 'MONSTRO<hr>';

$monstro = new Monstro();
$monstro->nome = 'Four';
$monstro->poder = $poderMaximo;
$monstro->fraqueza = $pontosdeFraqueza;
$monstro->superpoder = 
$monstro->pontosdevida = $pontosdeVida;
$monstro->dono = 'Stefane';
$monstro->ataque = $fraseAtaque;
$monstro->derrota = $frasedeDerrota;

echo'<b>Monstro:</b><br>';
echo'Nome: '.$monstro->nome."<br>";
echo'Poder: '.$monstro->poder."<br>";
echo'Fraqueza: '.$monstro->fraqueza."<br>";
echo'Super Poder: '.$monstro->superpoder."<br>";
echo'Pontos de Vida: '.$monstro->pontosdevida."<br>"
echo'Dono: '.$monstro->dono."<br>";

$fraseAtaque[] = "Vamos lutar";
$fraseAtaque[] = "Está Derrotado";
$fraseAtaque[] = "Vou te Derrotar";
$fraseAtaque[] = "Está Acabado";
$fraseAtaque[] = "Vai ser Aniquilado";

echo $fraseAtaque[0];
echo $fraseAtaque[1];
echo $fraseAtaque[2];
echo $fraseAtaque[3];
echo $fraseAtaque[4];

$fraseAtaque[rand(0, 4)];

$frasedeDerrota[] = "Fui Derrotado";
$frasedeDerrota[] = "Acabado";
$frasedeDerrota[] = "Dessolado";
$frasedeDerrota[] = "Exaurido";
$frasedeSerrota[] = "arruinado";

echo $frasedeDerrota[0]; 
echo $frasedeDerrota[1];
echo $frasedeDerrota[2];
echo $frasedeDerrota[3];
echo $frasedeDerrota[4];

$frasedeDerrota[rand(0, 4)];
?>

<?php
class Monstro extends SerVivo implements IMonstro{

   private $nome;
   private $nomeDoDono;

 interface IMonstro{

        public function setfichaTecnica($pontosDeVida, $poderdeAtaque, $superAtaque, $fraqueza){
               $this->pontosdeVida = $pontosdeVida;
	       $this->poderdeAtaque = $poderdeAtaque;
               $this->superAtaque = $superAtaque;
               $this->fraqueza = $fraqueza;
       }
	public function setNome($nome){
               $this->nome = $nome;
	}
	public function getNome(){
               return $this->nome;
	}
	public function setNomeDono($nomeDono){
               $this->nomeDono = $nomeDono;
	}
	public function getNomeDono(){
               return $this->nomeDono;
	}
        public function setPontosDeVida($PontosdeVida){
               $pontosVida = [rand(0, 100)];
	}
	public function getPontosDeVida(){
               return $this->PontosdeVida;
        }
        public function setPoderDeAtaque($PoderdeAtaque){
                $poderAtaque = [rand(0, 30)];
	}
	public function getPoderDeAtaque(){
                return $this->PoderdeAtaque;
        }
        public function setSuperAtaque($superAtaque){
                $superAtaques = [rand(0, 30)];
          
	}
	public function getSuperAtaque(){
                return $this->SuperAtaque;
        }
        public function setFraqueza($fraqueza){
               $fraquezas = [rand(0,30)];
	}
	public function getFraqueza(){
               return $this->Fraqueza;
        }

        public function getfraseDeAtaque(){
              $fraseAtaque[rand(0, 4)];
              return $this->frasesdeAtaque;
        }

        function getfraseDeDerrota(){
             $frasedeDerrota[rand(0, 4)];
             return $this->frasedeDerrota;
        }
        function gritar(){
             echo"Vamos Lutar!!!";
        }
        function somar($numero1, $numero2){
             return $numero1+$numero2;
        }


  }
}
?>

<?php

require('IMonstro.php');
require('SerVivo.php');
require('Monstro.php');

$monstro1 = new Monstro();

echo "Nome: ".$monstro1->getNome()."<br>";

$monstro1->gritar();

echo '<br>';

$resultado = $monstro1->somar(10,3);

if($resultado == 13){
	echo 'O resultado da soma é '.$resultado.'<br>'.
	      'Teste realizado com sucesso<br>';
} else {
	echo "O método não esta funcionando corretamente.<br>";
}

$monstro2 = new Monstro();

echo $monstro2->getPontosDeVida();

?>
