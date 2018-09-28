# Desenvolvimento-movel

class Casa(cor:String, qtGaragem:Int){
    //Propriedades.
    var cor: String
    var garagem: Int	
    
    //Construtor
    init {
        this.cor = cor
        this.garagem = qtGaragem
    }
    
   
    fun abrirPorta(){
        println("Porta aberta.")
    }
	fun abrirJanela(qt:Int){
        println("$qt Janela aberta.")
    }
	fun pintar(cor:String){
        this.cor = cor
    }
    fun abrirCasa(){
        this.abrirPorta()
        this.abrirJanela(2)
    }
}



fun main(args: Array<String>) {
    var casaJoao = Casa("verde",2)
    casaJoao.abrirCasa()
    casaJoao.cor = "azul"
  
    
    println(casaJoao.cor)
}
