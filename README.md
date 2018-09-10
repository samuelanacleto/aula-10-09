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









