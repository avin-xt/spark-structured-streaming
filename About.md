# Strategy

## 1. What is the schedule frequency ?
-  Many factors to be considerd to avoid **backpressure.** 
    1. *Processing time* of each batch, considering sudden peak *volumes* .
    2. Job cluster *startup time*
    3. In some cases , cleanup that job does.
  <img width="780" alt="image" src="https://github.com/avin-xt/spark-structured-streaming/assets/40514147/e14416a7-8e48-4a6b-9ed5-44b72d863e39">

## 2. Incremental data processing ?
 - How to implement check-pointing & failures.
      <img width="814" alt="image" src="https://github.com/avin-xt/spark-structured-streaming/assets/40514147/de4e534b-feef-4503-845c-93eb16789cfb">

    * Is checkpoint within workflow or is it outside of workflow.
    * If its outside , sometimes Workflow can be succesful , but checkpoint can be errored out.

## 3. Fault Tolerance ?
 -  Transactional checkpointing.

## 4. Late arriving dataset
- Late arriving dataset. Data processing begin at 9 AM, and goes for 15 min. What about data comming in between ?
