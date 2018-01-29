# correlation-matrix_Pyspark_RDD

The following code will help you in generating a correlation matrix for your N no of variables in the pyspark environment. 
You just have to fill the mandatory settings-

#INPUT-TABLE-DETAILS:
#Give the name of the input schema ( if you have any else you can remove this line and make changes to the code)
input_table_schema="XXXXX"
#Give the name of input table
input_table_name=" XXXXX" 
#Give the name of the target
target_name='target'

#CHECK FOR CORRELATION MATRIX
#Give a list of variables
Var= ['entity','region_name','state','cost_amt','cdv', 'offer_play_mix_name','target']

Note: you can simply give the path of your data if you dont have it on a server.
df=spark.sql("select * from " +input_table_schema+"."+input_table_name)
Its a spark sql initialisation line. You can change it according to your database pathway.

Rest of the code will run as it is producing the matrix.
