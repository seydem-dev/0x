# Verify Signature
**Verify Signature is a contract for signing messages from wallet pop ups (such as Metamask). All verification signature functions don't cost any gas.**

```
verify()
```
*Funtion takes in a signer and a signature and makes sure that both are valid. Returns true if passed, else false.*

```
getMessageHash()
```
*Returns hash of parameter `message`*

```
getEthSignedMessageHash()
```
*Returns the actual signed hash with a prefix (prefix is added and then hashed again to get the final hash).*

```
recover()
```
*Takes `ethSignedMessage` and `_sig` and recover the signer from the two inputs.*

```
_split()
```
*Splits `_sig` from `recover()` into `r`, `s`, and `v` of `recover()`*
