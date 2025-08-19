# ejercitacion-programacion

====> Ejercicio 7:

```
	static bool estaOrdenado(int[] a) {
		if (a.Length != 10) {
			return false;
		}
		
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
====> Ejercicio 8:

```
	static string[,] pedirNombres() {
		string[,] data = new string[5, 2];

		for (int i = 0; i < 5; i++) 
		{
			Console.WriteLine("****** Persona {0} ******", i+1);
			Console.Write("Nombre: ");
			data[i,0] = Console.ReadLine();
			Console.Write("Edad: ");
			data[i,1] = Console.ReadLine();
		}
		
		return  data;
	}
	
	static void imprimirMayores(string[,] mtz) 
	{
		for (int i = 0; i < 5; i++) 
		{

			if (int.Parse(mtz[i,1]) > 18)
			{
				Console.WriteLine("eeeeaaaaaaaaa");
				Console.WriteLine("{0} es mayor de edad", mtz[i,0]);
			}
		}
	}
	
	
	
	public static void Main()
	{
		string[,] data = pedirNombres();
		imprimirMayores(data);
	}
```

====> Ejercicio 9:

```
	static string[,] ingresarProductos() {
		string[,] data = new string[5, 2];

		for (int i = 0; i < 5; i++) 
		{
			Console.WriteLine("****** Producto {0} ******", i+1);
			Console.Write("Nombre: ");
			data[i,0] = Console.ReadLine();
			Console.Write("Precio: ");
			data[i,1] = Console.ReadLine();
		}
		
		return  data;
	}
	
	static void imprimirMayores(string[,] mtz) 
	{
		int p = int.Parse(mtz[0,1]);
		for (int i = 0; i < 5; i++) 
		{

			if (int.Parse(mtz[i,1]) > p)
			{
				Console.WriteLine("*******===<3=>******");
				Console.WriteLine("{0} es más caro que el 1er producto: {1}", mtz[i,0], mtz[0,0]);
			}
		}
	}
	
	
	
	public static void Main()
	{
		string[,] data = ingresarProductos();
		imprimirMayores(data);
	}
```
