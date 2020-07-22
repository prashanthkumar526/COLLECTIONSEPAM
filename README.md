# COLLECTIONSEPAM
package behavioural;

public class CollectionofNames implements Container {
	public String name[]={"Manjula", "SriRamulu","Shyam","Kranthi","Kiranmai"};   
    
	public Iterator getIterator() {  
	        return new CollectionofNamesIterate() ;  
	    }  
	    private class CollectionofNamesIterate implements Iterator{  
	        int i;  
	        public boolean hasNext() {  
	            if (i<name.length){  
	                return true;  
	            }  
	            return false;  
	        }  
	        public Object next() {  
	            if(this.hasNext()){  
	                return name[i++];  
	            }  
	            return null;      
	        }  
	    }  
	}  


