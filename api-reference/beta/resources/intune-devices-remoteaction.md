---
title: remoteaction 列挙型
description: リモートアクション Intune がサポートしています。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4d7835ac9ecc1c9e7df7724032a97d31d7d99069
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521216"
---
# <a name="remoteaction-enum-type"></a>remoteaction 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

リモートアクション Intune がサポートしています。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|ユーザーが不明なアクションを開始します。|
|factoryReset|1 |ユーザーがデバイスを出荷時にリセットするアクションを開始します。 |
|removecompanydata|2 |ユーザーがデバイスから会社のデータを削除するアクションを開始します。 |
|resetPasscode|3 |ユーザーが、iOS デバイスのパスコードを削除するアクションを開始するか、Android/Windows デバイスのパスコードをリセットします。 |
|remoteLock|4 |ユーザーがデバイスをリモートロックするアクションを開始します。|
|enableLostMode|5 |ユーザーが、監視対象 iOS デバイスで失われたモードを有効にするアクションを開始します。|
|disableLostMode|6 |ユーザーが、監視対象 iOS デバイスで失われたモードを無効にするアクションを開始します。|
|locateDevice|7 |ユーザーが、監視対象 iOS デバイスを検索するアクションを開始します。|
|rebootNow|8 |ユーザーが Windows デバイスを再起動するアクションを開始します。|
|recoverPasscode|9 |ユーザーが windows phone デバイスでのパスポートの pin をリセットするアクションを開始します。|
|cleanWindowsDevice|10  |ユーザーが windows デバイスをクリーンアップするアクションを開始します。|
|logoutSharedAppleDeviceActiveUser|11 |ユーザーが、共有 apple デバイスの現在のユーザーをログアウトするアクションを開始します。|
|quickScan|12 |ユーザーがデバイスでクイックスキャンを実行するアクションを開始します。|
|fullScan|13 |ユーザーがデバイスでフルスキャンを実行するアクションを開始します。|
|windowsDefenderUpdateSignatures|14 |ユーザーがデバイスでマルウェア署名を更新するアクションを開始します。|
|factoryResetKeepEnrollmentData|15 |ユーザーが、登録データを保持する操作リモートワイプデバイスを開始します。|
|updatedeviceaccount|16 |ユーザーがデバイス上のアカウントを更新するアクションを開始します。|
|自動再展開|17 |ユーザーがデバイスを自動化して再展開するアクションを開始する|
|シャット|18 |ユーザーがデバイスをシャットダウンするアクションを開始します。|





