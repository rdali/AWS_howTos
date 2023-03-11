<style>
details > summary {
  padding: 12px 12px;
  background-color: #f0f8ff;
  border: none;
  box-shadow: 1px 1px 1px grey;
}

details > p {
  border-radius: 0 0 0px 0px;
  background-color: #f0f8f7;
  padding: 10px 15px;
  margin: 0;
  border-left-width: 5px;
  border-left-style: solid;
  border-left-color: #b3dbff;
  border-radius: 0px;
  }
</style>


<img src="vecteezy_did-you-know-sticker-vector_7688896.jpg"  width="30%" height="30%">


# Lambda uses the same execution environment for seprate invocations of the same function.


This process, called "warm start", is great because it means that consecutive runs of your function are faster than the first invocation. However, you need to be careful about Global variables and the possibility that what is thought of as an isolated run might not be as isolated as you thought.


[Reference](https://docs.aws.amazon.com/lambda/latest/operatorguide/execution-environments.html)


# Now You Know!