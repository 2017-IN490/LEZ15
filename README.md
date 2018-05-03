# LEZ15

per esercizio: eliminare la parte di codice 
che serve a differenziare la creazione di un elemento 
Matrix quando Filter e' l'ultimo della lista oppure no.

in quadratic.Filter appare sostanzialmente identico per 
due volte questo pezzo di codice, come fare per trattare questo caso 
in modo appropriato ?

      if( p.compareTo(new BigInteger("2")) == 0 )
				{
					tmp = null ;
			
					System.out.println(" reference to next object (2): "+tmp);
					this.column = new Matrix(tmp , tmp, BigInteger.ONE);
				}
			else
				{	
					tmp = ((Filter)tail).column();
					System.out.println(" reference to next object (step): "+tmp);
					this.column = new Matrix(tmp , this.setzerocolumn(tmp), BigInteger.ONE);
				};
        
        
