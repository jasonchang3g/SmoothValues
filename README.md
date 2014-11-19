
public class SmoothValue
{
	public static void main(String[] args)
	{
		/**
		 * smooths out array
		 */
		public void smooth()
		{
			double[] values;
			double num1 = values[values.length];
			double num2 = values[values.length - 1];
			for(int i = 0; i < values.length; i++)
			{
				if(i == 0){
					values[i] = (values[i] + values[i + 1]) / 2;
				}
				
				double temp = values[i];
				values[i + 1] = (temp + values[i + 1] + values[i + 2]) / 3;
				
				
				if(i == values.length){
					values[values.length] = (num1 + num2)/2; 
				}
			}
		}
	}
}
