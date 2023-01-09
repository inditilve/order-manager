# Simple netting engine
## Todo
1. get kafka broker running locally
2. define avro for order, execution (json) - ticker, qty, price, timestamp
3. pump - to hydrate all the topics - expose via rest (figure out a way to also purge topics easily for testing)
4. netting -
    a. group by ticker, sum, per topic
    b. group by ticker, sum, across topics
5. fill - random filler from 1-x -> expose via rest?
6. assign back to respective topic? new topic? store result so as to not recompute(if exposing to rest?) -  based on 3a / 3b -> expose via rest?