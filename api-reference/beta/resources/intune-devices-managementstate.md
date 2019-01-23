---
title: managementState 列挙型
description: Microsoft Intune でのデバイスの状態を管理します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a8d0801949125f3b0cceb865ac1f8546195112e3
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420018"
---
# <a name="managementstate-enum-type"></a>managementState 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Microsoft Intune でのデバイスの状態を管理します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|管理|0|管理対象デバイスは、します。|
|retirePending|1|削除コマンドは、デバイスと管理から unenrolling の処理中に発生しています。|
|retireFailed|2|破棄コマンドがデバイスに失敗しました。|
|wipePending|3|ワイプ コマンドは、デバイスと管理から unenrolling の処理中に発生しています。|
|wipeFailed|4|デバイス ワイプ コマンドが失敗しました。|
|問題があります。|5|デバイスが正常な状態ではありません。|
|deletePending|6|削除コマンドは、デバイスで発生しています。 |
|retireIssued|7|デバイスの削除コマンドが発行されました|
|wipeIssued|8|デバイス ワイプ コマンドがに対して発行されました|
|wipeCanceled|9|このデバイスのワイプ コマンドがキャンセルされました|
|retireCanceled|10|このデバイスの削除コマンドがキャンセルされました|
|発見|11|デバイスが検出されたが、完全に登録されています。|




