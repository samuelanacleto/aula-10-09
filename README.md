# aula-10-09
package aluno;

public class aluno {
	
	private String nome;
	private String curso;
	private String semestre;
	private String periodo;
	private Double N1;
	private Double N2;
		
	aluno (String nome,String curso,String semestre,String periodo){
	
	this.nome=nome;
	this.curso=curso;
    this.semestre=semestre;
    this.periodo=periodo; }
	
	public void setN1(Double n){
	    this.N1=n;}
	public void setN2(Double n){
		this.N1=n;}
	public double media (){
		return (this.N1+this.N2)/2;
	}
	
	public String  getNome(){
		return this.nome;}
	public String getCurso(){
		return this.curso; }
	public String getSemestre(){
		return this.semestre; }
	public String getPeriodo(){
		return this.periodo; }

}

/////////////////////////////////////////////////////////////////////////

package aluno;

public class teste {
	aluno a1 = new aluno ("maria","redes","1s","noite");
    aluno a2 = new aluno ("jose","engenharia","3s","manha");
    
    System.out.println("listagem alunos");
    System.out.println(a1.getNome());
    System.out.println(a2.getNome());
    
    a1.setN1(5.0);
    a2.setN2(6.0);
    
    if (a1.media()>=5)
    	system.out.println("aprovado");
    else
    	system.out.println("reprovado");
    }

||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||

package banco;

public class conta {
	private double numero;
	private double saldo;
	private double limite;
	private String nome;
	
	conta (double numero,double saldo,double limite,String nome){
	this.numero=numero;
	this.saldo=saldo;
	this.limite=limite; }
	
	public boolean saca(double valor){
		if (this.saldo>=valor){
			this.saldo=this.saldo-valor;
			return true;}
	
	else
		   return false;
	}
		
	
	public void deposita (double valor){
	this.saldo=this.saldo+valor;
	

}}
|||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||||

package banco;

public class teste {

	public static void main(String[] args) {
		conta c1 = new conta(9000,1000.00,0.00,"Pedro de Alcantara");
		
		c1.deposita(1000);
		
		if (c1.saca(2500)==true)
			System.out.println("Saque realizado!");
		else
			System.out.println("Limite insuficiente!");

	}

}
