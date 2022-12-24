## Part 1 zk-SNARKs と zk-STARKS の理論的背景

- SNARK が信頼できるセットアップを必要とし、STARK がそうしない理由を 2-4 文で説明しなさい。

- SNARK と STARK の証明の違いをあと 2 つ挙げてください。

## コマンド系

- circom ファイルをコンパイルして`sol`ファイルを生成するスクリプトを実行する。

```bash
sh ./scripts/compile-HelloWorld.sh
```

結果

```bash
Compiling HelloWorld.circom...
template instances: 1
non-linear constraints: 1
linear constraints: 0
public inputs: 0
public outputs: 1
private inputs: 2
private outputs: 0
wires: 4
labels: 4
Written successfully: HelloWorld/HelloWorld.r1cs
Written successfully: HelloWorld/HelloWorld.sym
Written successfully: HelloWorld/HelloWorld_js/HelloWorld.wasm
Everything went okay, circom safe
[INFO]  snarkJS: Curve: bn-128
[INFO]  snarkJS: # of Wires: 4
[INFO]  snarkJS: # of Constraints: 1
[INFO]  snarkJS: # of Private Inputs: 2
[INFO]  snarkJS: # of Public Inputs: 0
[INFO]  snarkJS: # of Labels: 4
[INFO]  snarkJS: # of Outputs: 1
[INFO]  snarkJS: Reading r1cs
[INFO]  snarkJS: Reading tauG1
[INFO]  snarkJS: Reading tauG2
[INFO]  snarkJS: Reading alphatauG1
[INFO]  snarkJS: Reading betatauG1
[INFO]  snarkJS: Circuit hash:
                4289918f b00ce352 b426119d 49059905
                382c440e 3439767d b58836b9 6ce102b4
                ea11be67 46375b98 850f3fe6 d5db5730
                122e33c7 65c9a1ec 5e9480aa cbb49b5d
[DEBUG] snarkJS: Applying key: L Section: 0/2
[DEBUG] snarkJS: Applying key: H Section: 0/4
[INFO]  snarkJS: Circuit Hash:
                4289918f b00ce352 b426119d 49059905
                382c440e 3439767d b58836b9 6ce102b4
                ea11be67 46375b98 850f3fe6 d5db5730
                122e33c7 65c9a1ec 5e9480aa cbb49b5d
[INFO]  snarkJS: Contribution Hash:
                9a2e095d 01789815 adf03a32 cf4bde33
                60d53cdb 7480ec6e ba4d21b0 d420c0cb
                ccf869d7 6fcafa4a c553ac8e c146a57d
                ed04dcc3 210dd0ae 25903229 bab55aaa
```

## 検証方法

1. コマンドで実行する場合
