# Streaming 

1. Streaming query is a background thread (co-ordinator ) thats started to manage execution of streaming job.
2. SQ will prepare the checkpointDirectory & also watches for new data.
3. When new data lands , **SQ configures the input for micro batch & then triggeres it.**
4. SQ will monitor the Micro-batch execution ,and once its succesful it commits the check-point.
<img width="460" alt="image" src="https://github.com/avin-xt/spark-structured-streaming/assets/40514147/8707a700-de96-42b4-b01a-0c520abeb437">
