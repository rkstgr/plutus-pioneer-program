Getting the POSIX-Time of a slot for the Playground
```haskell
import  Ledger.Time
import Ledger.TimeSlot
import Data.Default

slotToBeginPOSIXTime def 10
-- 1596059101000

slotToBeginPOSIXTime def 20
-- 1596059111000
```


Generating the pubKeyHash for a demo wallet in the Playground
```haskell
import Wallet.Emulator

mockWalletPaymentPubKeyHash $ knownWallet 1
-- a2c20c77887ace1cd986193e4e75babd8993cfd56995cd5cfce609c2

mockWalletPaymentPubKeyHash $ knownWallet 2
-- 80a4f45b56b88d1139da23bc4c3c75ec6d32943c087f250b86193ca7

mockWalletPaymentPubKeyHash $ knownWallet 3
-- 2e0ad60c3207248cecd47dbde3d752e0aad141d6b8f81ac2c6eca27c
```


