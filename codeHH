using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ClassLibrary1
{
    public static class area
    {
        public static double unknown(double[] mas) 
        {
            if (mas.Length == 1)
               return Circle(mas[0]);
            if (mas.Length == 3)
               return triangle(mas[0], mas[1], mas[2]);
            return 0;
        }
        public static double unknown(double Radius)
        {
            return Circle(Radius);
        }
        public static double unknown(double OneSide, double TwoSide, double ThreeSide)
        {
            return triangle(OneSide,TwoSide,ThreeSide);
        }

        public static double Circle(double Radius)
        {
            if(Radius<=0)
                throw new Exception("Радиус не может быть отрицательным или равен 0.");
            return 2 * Math.PI * Math.PI * Radius;
        }



        public static double triangle(double OneSide, double TwoSide, double ThreeSide) 
        {
            double p = (OneSide + TwoSide + ThreeSide) / 2;
            double s=p * (p - OneSide) * (p - TwoSide) * (p - ThreeSide);
            if (s < 0)
                throw new Exception("Треугольник с такими сторонами не существует.");  
            return Math.Sqrt(s);
        }
        


        public static bool RectangularTriangle(double OneSide, double TwoSide, double ThreeSide)
        {
            double p = (OneSide + TwoSide + ThreeSide) / 2;
            double s = p * (p - OneSide) * (p - TwoSide) * (p - ThreeSide);
            if (s < 0)
                throw new Exception("Треугольник с такими сторонами не существует.");
            if ((Math.Pow(OneSide, 2) + Math.Pow(TwoSide, 2)) == Math.Pow(ThreeSide, 2))
                return true;
            if ((Math.Pow(TwoSide, 2) + Math.Pow(ThreeSide, 2)) == Math.Pow(OneSide, 2))
                return true;
            if ((Math.Pow(OneSide, 2) + Math.Pow(ThreeSide, 2)) == Math.Pow(TwoSide, 2))
                return true;
            return false;
        }
    }

}


ВОПРОС 9--------------------------------------------------------------------------------------------

не работал с   MS SQL Server, работал только с SQL oracle apex
 select Product.name,nvl(Kategor.name,"ОТСУСТВУЕТ")
    from Product, Kategor 
    where(Product.p_id=Kategor.p_id(+)) 



