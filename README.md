# ejercitacion-programacion

====> Ejercicio 7:

```
static bool estaOrdenado(int[] a) {
		for (int i = 1; i < a.Length; i++) 
		{
			if (a[i-1] > a[i]) 
			{
				return false;
			}
		}
		return true;
	}
	
	
	
	public static void Main()
	{
		int[] arr = {1,3,5,6,8};
		Console.WriteLine(estaOrdenado(arr));
	}
```
