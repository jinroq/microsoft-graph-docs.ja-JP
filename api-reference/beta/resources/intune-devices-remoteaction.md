---
title: remoteaction 列挙型
description: リモートアクション Intune がサポートしています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d7835ac9ecc1c9e7df7724032a97d31d7d99069
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31799441"
---
# <a name="remoteaction-enum-type"></a>remoteaction 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

リモートアクション Intune がサポートしています。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|ユーザーが不明なアクションを開始します。|
|factoryReset|1-d|ユーザーがデバイスを出荷時にリセットするアクションを開始します。 |
|removecompanydata|pbm-2|ユーザーがデバイスから会社のデータを削除するアクションを開始します。 |
|resetPasscode|1/3|ユーザーが、iOS デバイスのパスコードを削除するアクションを開始するか、Android/Windows デバイスのパスコードをリセットします。 |
|remoteLock|2/4|ユーザーがデバイスをリモートロックするアクションを開始します。|
|enableLostMode|5|ユーザーが、監視対象 iOS デバイスで失われたモードを有効にするアクションを開始します。|
|disableLostMode|シックス|ユーザーが、監視対象 iOS デバイスで失われたモードを無効にするアクションを開始します。|
|locateDevice|7|ユーザーが、監視対象 iOS デバイスを検索するアクションを開始します。|
|rebootNow|~|ユーザーが Windows デバイスを再起動するアクションを開始します。|
|recoverPasscode|i-9|ユーザーが windows phone デバイスでのパスポートの pin をリセットするアクションを開始します。|
|cleanWindowsDevice|個|ユーザーが windows デバイスをクリーンアップするアクションを開始します。|
|logoutSharedAppleDeviceActiveUser|#|ユーザーが、共有 apple デバイスの現在のユーザーをログアウトするアクションを開始します。|
|quickScan|個|ユーザーがデバイスでクイックスキャンを実行するアクションを開始します。|
|fullScan|スリー|ユーザーがデバイスでフルスキャンを実行するアクションを開始します。|
|windowsDefenderUpdateSignatures|第|ユーザーがデバイスでマルウェア署名を更新するアクションを開始します。|
|factoryResetKeepEnrollmentData|約|ユーザーが、登録データを保持する操作リモートワイプデバイスを開始します。|
|updatedeviceaccount|16|ユーザーがデバイス上のアカウントを更新するアクションを開始します。|
|自動再展開|インチ|ユーザーがデバイスを自動化して再展開するアクションを開始する|
|シャット|個|ユーザーがデバイスをシャットダウンするアクションを開始します。|





