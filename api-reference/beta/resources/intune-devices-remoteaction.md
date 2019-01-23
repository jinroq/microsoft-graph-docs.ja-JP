---
title: remoteAction 列挙型
description: リモート操作 Intune をサポートしています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3177ea43599cd155e11af1786636111a8578d29b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405542"
---
# <a name="remoteaction-enum-type"></a>remoteAction 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

リモート操作 Intune をサポートしています。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|不明|0|ユーザーは、不明なアクションを開始します。|
|factoryReset|1|工場出荷時の動作を開始するユーザーは、デバイスをリセットします。 |
|removeCompanyData|2|ユーザーは、デバイスから企業データを削除するアクションを開始します。 |
|resetPasscode|3|ユーザーが、iOS デバイスのパスコードを削除するか、アプリのパスコードをリセットする操作を開始すると Windows のデバイスです。 |
|remoteLock|4|ユーザーは、デバイスをリモート ロック操作を開始します。|
|enableLostMode|5|ユーザーは、コールを管理する iOS デバイス上で失われたモードを有効にする操作を開始します。|
|disableLostMode|6|ユーザーは、コールを管理する iOS デバイス上で失われたモードを無効にする操作を開始します。|
|locateDevice|7|ユーザーは、コールを管理する iOS デバイスを検索する操作を開始します。|
|rebootNow|8|ユーザーは、Windows のデバイスを再起動する操作を開始します。|
|recoverPasscode|9|ユーザーは、windows の電話デバイスでの作業の passport の pin をリセットするのにはアクションを開始します。|
|cleanWindowsDevice|10|ユーザーは、windows のデバイスをクリーンアップする処理を開始します。|
|logoutSharedAppleDeviceActiveUser|11|ユーザーは、共有の apple デバイス上の現在のユーザーをログアウトする操作を開始します。|
|quickScan|12|ユーザーは、デバイス上のクイック スキャンを実行するアクションを開始します。|
|fullScan|13|ユーザーは、デバイスの完全なスキャンを実行するアクションを開始します。|
|windowsDefenderUpdateSignatures|14|ユーザーは、デバイス上のマルウェアの署名を更新する操作を開始します。|
|factoryResetKeepEnrollmentData|15|ユーザーは、登録データを保持することで、デバイスを操作リモート ワイプを開始します。|
|updateDeviceAccount|16|ユーザーは、デバイス上のアカウントを更新する操作を開始します。|
|automaticRedeployment|17|ユーザーが automatice デバイスを再配置する操作を開始します。|
|シャット ダウン|18|ユーザーは、デバイスをシャット ダウンする操作を開始します。|




