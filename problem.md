import pyspark as ps

spark = ps.sql.SparkSession.builder \
    .master('local[4]') \
    .appName("spark-lecture") \
    .getOrCreate()

sc = spark.SparkContext

