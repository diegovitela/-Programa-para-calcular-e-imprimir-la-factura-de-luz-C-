Copia el codigo que esta abajo y cambia los valores de comicion por las que usted desee, les recomedamos cambiar el valor del IVA dependiendo su pais y tambien cambiar "Total por consumo, 1.20 por unidad" por la cantidad que te cobra tu empresa de luz 







    
    
        static void Main(string[] args)
        {
        
            int Id;
            
            string nom;
            
            int cont;
            
            
            Console.Write($"Ingrese su ID del cliente: ");
            Id = Convert.ToInt32(Console.ReadLine());
            Console.Write($"Ingrese su Nombre:");
            nom = Console.ReadLine();
            Console.Write($"Ingresese su consumo de energia: ");
            cont = Convert.ToInt32(Console.ReadLine());

            if (cont <= 100)
            {
                Console.WriteLine($"ID del cliente:{Id} ");
                Console.WriteLine($"Su Nombre es: {nom}");
                Console.WriteLine($" consumo es : {cont}");
                Console.WriteLine($"IVA:A su  cantidad no se le agrega IVA ");
                Console.WriteLine($"Usted tiene que pagar 100");
            }

            else if (cont <= 199)
            {
                Console.WriteLine($"ID del cliente:{Id} ");
                Console.WriteLine($"Su Nombre es: {nom}");
                Console.WriteLine($" consumo es: {cont}");
                Console.WriteLine($"Total por consumo, 1.20 por unidad :{cont * 1.20} ");
                Console.WriteLine($"IVA:A su  cantidad no se le agrega IVA ");
                Console.WriteLine($"Usted tiene que pagar :{cont * 1.20} ");

            }

            else if ((cont >= 200)&&(cont <300))
            {
                Console.WriteLine($"ID del cliente: {Id} ");
                Console.WriteLine($"Su Nombre es: {nom}");
                Console.WriteLine($"Consumo: {cont}");
                Console.WriteLine($"Total por consumo, 1.5 por unidad:{cont * 1.5} ");
                Console.WriteLine($"IVA: A su  cantidad no se le agrega IVA ");
                Console.WriteLine($"Usted tiene que pagar :{cont * 1.5} ");
            }
            else if ((cont >= 300)&&(cont <400))
            {
                Console.WriteLine($"ID del cliente:{Id} ");
                Console.WriteLine($"Su Nombre es:´{nom}");
                Console.WriteLine($"Consumo: {cont}");
                Console.WriteLine($"Total por consumo, 1.5 por unidad:{cont * 1.5} ");
                Console.WriteLine($"IVA:{cont * 1.5 * .15} ");
                Console.WriteLine($"Usted tiene que pagar :{cont * 1.5 * .15 + cont * 1.5} ");
            }

            else if ((cont >= 400)&&(cont <600))
            {
                Console.WriteLine($"ID del cliente: {Id} ");
                Console.WriteLine($"Su Nombre es: {nom}");
                Console.WriteLine($"Consumo: {cont}");
                Console.WriteLine($"Total por consumo, 1.8 por unidad:{cont * 1.8} ");
                Console.WriteLine($"IVA:{cont * 1.8 * .15} ");
                Console.WriteLine($"Usted tiene que pagar :{cont * 1.8 * .15 + cont * 1.8} ");
            }
           
        
         
            
            else if (cont >= 600)
            {
                Console.WriteLine($" ID del cliente:{Id} ");
                Console.WriteLine($"Su Nombre es: {nom}");
                Console.WriteLine($"Consumo: {cont}");
                Console.WriteLine($"Total por consumo, 2.0 por unidad:{cont * 2.0} ");
                Console.WriteLine($"IVA:{cont * 2.0 * .15} ");
                Console.WriteLine($"Usted tiene que pagar :{cont * 2.0 * .15 + cont * 2} ");
            }

        }


    }
}

file:///C:/Users/netce/Downloads/Examen%20Parte%202%20(3).cs    Aqui esta el link del codigo completo por cualquier cosa 
