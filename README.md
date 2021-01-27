# pyneedn

pyneedn aims to build a data integraion and ETL toolkit for any popular open source compute engines or databases.

## Usage

    etl_function_list = [load_d_payment_method]
    etl_spark_session = SparkETL.get_spark_session("dimension_loading")
    spark_etl = SparkETL("ETL demo", etl_spark_session, "CLIENT")
    spark_etl.process_etl(spark_table_list, *etl_function_list)
