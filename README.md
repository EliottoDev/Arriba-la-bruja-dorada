# Programa para obtener la formula de un prisma hexagonal
## Indice
  - Uso
  - Codigo fuente
  - Creador 😎
## Uso
Simplemente pon el valor de un lado en el cuadro de teksto, pulsa el boton y ya ta :v<br/>
En los otros dos cuadros tendras el area y volumen en funcion del lado :v<br/>
Si :v<br/>
Asi de facil :v<br/>
## Codigo fuente
Pos a ver si entiendes algo :v<br/>
```using System;

class Acciones
{
    /**
    * @description Lee archivo de texto solo 
    * @returns El area de la formula solo sabiendo un lado de la base y un lado de una cara x
    */
    public static string leerTxt(string ruta)
    {
        string appPath = System.IO.Path.GetDirectoryName(ruta);
        string[] txt = System.IO.File.ReadAllLines(appPath);
        string r = "";
        foreach(string l in txt)
        {
            if (l == txt[0])
            {
                r = $"{l}";
            }
            else
            {
                r = r+$"\n{l}";
            }
        }
        return r;
    }

    /**
     * @description Devuelve el area de la figura siguiendo la formula
     * @returns El area de la formula solo sabiendo un lado de la base y un lado de una cara x
     */
    public static double area(double x)
    {
        double s = 6 * Math.Pow(x, 2) + (6 * x * Math.Sqrt(Math.Pow(x, 2) - Math.Pow(x / 2, 2)));
        return s;
    }

    /**
     * @description Devuelve el volumen de la figura siguiendo la formula
     * @returns El volumen de la formula solo sabiendo un lado de la base y un lado de una carax
     */
    public static double volumen(double x)
    {
        double s = 3 * x * x * Math.Sqrt(Math.Pow(x, 2) - Math.Pow(x / 2, 2));
        return s;
    }
}`


## Creador
Lo ves o no lo ves? Porque io si lo veo<br/>
MIRA LA URL >:v
