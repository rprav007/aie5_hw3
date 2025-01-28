# Homework 3 Answers

1. Why do we want to support streaming? What about streaming is important, or useful?

We are using streaming to primarily provide the user with a better experience and improved efficiency. Here are some of the advantages of using streaming
  * Without streaming the user has to wait the entire length of time the LLM generates the response with nothing on screen
  * Gives the perception of reduced latency as the user sees the response as it gets generated
  * Long responses can have memory issues and streaming safeguards against that
    
2. Why are we using User Session here? What about Python makes us need to use this? Why not just store everything in a global variable?

We are using user session here because we want the application to be multi-tenant. Multiple users can potentially work with the same application at the same time and each users interaction and context is maintained within a session. If the scope of the variable is global, then the context and other aspects overwritten while multiple users are using the application.
