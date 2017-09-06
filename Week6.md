# Week 6































For textbook RSA, signing and decrypt is the same...









<hr>

---



### why use hash function before signature

* get fixed size output computation

* integrity check of message -> make sure massage has not been changed

* against replace attack

  ​



### Hash function requirement

* collision resistant(weak) -> computation infeasible
* collision resistant(Strong) -> cannot find a pair of (x,y) that H(x) = H(y)
* input -> can be any size
* output -> must be fixed size for all input -> larger size the more collision resistant
* easy to compute H(x) from x
* Infeasible to compute x from H(X) -> one way function