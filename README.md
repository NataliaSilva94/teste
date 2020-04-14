# teste

public class calculadora {
	
	
	private int resultado =0;
	
	public int somar (int n1,int n2) {
		resultado = n1+ n2;
		return resultado;
	}
	
	public int subtrair (int n1, int n2) {
		
		resultado = n1 - n2;
		return resultado;
	}
	
	public int multiplicar( int n1, int n2 ){
		resultado = n1 * n2;
		return resultado;
	}
	
	public int dividir( int n1, int n2 ){
		resultado = n1 / n2;
		return resultado;
	}

	
	
	

}




import static org.junit.jupiter.api.Assertions.*;

import org.junit.jupiter.api.Test;

import junit.framework.TestCase;

public class calculadoraTest extends TestCase {

	@Test
	public void testSomar() {
		int nro1 = 5;
		int nro2 = 5;
		
		calculadora calc = new calculadora();
		int resultadoEsperado =10;

		int resultadoReal= calc.somar(nro1, nro2);
		assertEquals(resultadoEsperado, resultadoReal);
		}
	
	
	@Test
	
	public void testeSubtrair() {
		int nro1 = 5;
		int nro2 = 3;
	
		calculadora calc = new calculadora();
		int resultadoEsperado= 2;
		
		int resultadoReal= calc.subtrair(nro1, nro2);
		assertEquals(resultadoEsperado, resultadoReal);
	
	}
	
	
	@Test
	public void testeMultiplicar() {
		int nro1 = 3;
		int nro2 = 3;
		
		calculadora calc = new calculadora();
		int resultadoEsperado = 9;
		
		int resultadoReal = calc.multiplicar(nro1, nro2);
		assertEquals(resultadoEsperado, resultadoReal);
	}
		
	
	
	@Test
	public void testeDividir() {
	
		int nro1 = 6;
		int nro2 = 2;
		
		calculadora calc = new calculadora();
		int resultadoEsperado= 3;
		
		int resultadoReal = calc.dividir(nro1, nro2);
		assertEquals(resultadoEsperado, resultadoReal);
	}
		
	
}


















