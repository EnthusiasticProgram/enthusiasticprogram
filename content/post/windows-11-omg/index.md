+++
title = "Windows11？なんすかWindows11って？"
date = "2021-07-05"
slug = "windows-11-omg"
image = "windows11.png"
description = "だめだこりゃ（笑）"
categories = [
    "デジタル"
]
tags = [
    "パソコン"
    "Windows"
]
+++

お久しぶりです。PeeNuです。

PeeNuです。

どうもPeeNuです。

みなさんWindows 11のInsider Preview入れましたか？

私はビビりながらやりました。

なんかいろいろ躓いたことがあったので、そこらへんを後世のWindows 11インストールしたいマンに受け継ぐために書き残していこうと思います。



と思ったんですけど、なんかここで紹介してるツールとかもう公開されてないやつあるんで、どんな挑戦をしたかだけみてってください。

## PCの性能

CPU: Ryzen 5 2600X(6C12T、3.6GHz)

GPU: GTX1650(4GB)

マザーボード: ASRock Fatal1ty B450 Gaming-ITX/ac

ストレージ:WD BLUE M.2 500GB SSD

##  PC正常性チェックツール

まずWindows 11(Win11)を動かせるかどうかの診断をするMicrosoftのツール「PC正常性チェックツール」を回してみました。

「「この PC では Windows 11 を実行できません」」

おｋですおｋです。

ここまでは想定内です。

ただ、何が原因で実行できないのかが明記されてないのが微妙なところです。

## WhyNotWin11

次になんでWin11が実行できないのかまで明記されているツール「[WhyNotWin11](https://github.com/rcmaehl/WhyNotWin11)」を試してみます。

すると、

× Secure Boot

× TPM Version

と出ました。なんかセキュアブートとTPMがうまくいってないらしいです。

## うまくいけ

ということで、UEFI上でセキュアブートとTPMを有効にしていきます。

・AdvancedからAMD fTPM configurationでTPMを有効にします。

・SecurityからSecure Bootを有効にします。

## もう一度

できたのでもう一度PC正常性チェックツールを動かすと、

「「この PC で Windows 11 を実行できます」」

勝ちました。

## Insider Preview

Insider PreviewでWindows 11をインストールするには、まずチャネルをDev チャネルにしないと出てきません。

それから少し待ちます。

![Windows 11]({{site.url}}\assets\images\windows11hello.png)

はいできました。


## まとめ

***正式リリースを待とう！！***

以上です。PeeNuでした。
