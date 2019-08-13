---
title: remoteAction 列挙型
description: リモートアクション Intune がサポートしています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ac112c970fd05f7c697402d3cb3a14782890c7fe
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372126"
---
# <a name="remoteaction-enum-type"></a>remoteAction 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

リモートアクション Intune がサポートしています。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|.0|ユーザーが不明なアクションを開始します。|
|factoryReset|1-d|ユーザーがデバイスを出荷時にリセットするアクションを開始します。 |
|removeCompanyData|pbm-2|ユーザーがデバイスから会社のデータを削除するアクションを開始します。 |
|resetPasscode|1/3|ユーザーが、iOS デバイスのパスコードを削除するアクションを開始するか、Android/Windows デバイスのパスコードをリセットします。 |
|remoteLock|2/4|ユーザーがデバイスをリモートロックするアクションを開始します。|
|enableLostMode|5|ユーザーが、監視対象 iOS デバイスで失われたモードを有効にするアクションを開始します。|
|disableLostMode|シックス|ユーザーが、監視対象 iOS デバイスで失われたモードを無効にするアクションを開始します。|
|locateDevice|7|ユーザーが、監視対象 iOS デバイスを検索するアクションを開始します。|
|rebootNow|8 |ユーザーが Windows デバイスを再起動するアクションを開始します。|
|recoverPasscode|9 |ユーザーが windows phone デバイスでのパスポートの pin をリセットするアクションを開始します。|
|cleanWindowsDevice|10 |ユーザーが windows デバイスをクリーンアップするアクションを開始します。|
|logoutSharedAppleDeviceActiveUser|#|ユーザーが、共有 apple デバイスの現在のユーザーをログアウトするアクションを開始します。|
|quickScan|個|ユーザーがデバイスでクイックスキャンを実行するアクションを開始します。|
|fullScan|スリー|ユーザーがデバイスでフルスキャンを実行するアクションを開始します。|
|windowsDefenderUpdateSignatures|第|ユーザーがデバイスでマルウェア署名を更新するアクションを開始します。|
|factoryResetKeepEnrollmentData|約|ユーザーが、登録データを保持する操作リモートワイプデバイスを開始します。|
|updateDeviceAccount|16|ユーザーがデバイス上のアカウントを更新するアクションを開始します。|
|自動再展開|インチ|ユーザーがデバイスを自動化して再展開するアクションを開始する|
|シャット|個|ユーザーがデバイスをシャットダウンするアクションを開始します。|
|rotateFileVaultKey|1280|ユーザーが mac で FileVaultKey を回転するアクションを開始します。|
|getFileVaultKey|21|ユーザーが mac で FileVaultKey を取得するアクションを開始します。|
|setDeviceName|×|ユーザーがデバイスのデバイス名を設定するアクションを開始します。|



