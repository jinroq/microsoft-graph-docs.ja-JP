---
title: deviceComplianceActionType 列挙型
description: 列挙型の操作をスケジュールします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cd0db68a21fff79ddbab924e8a1d9bd2ff2e542d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425744"
---
# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

列挙型の操作をスケジュールします。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|noAction|0|操作は必要ありません。|
|通知|1|通知を送信します。|
|ブロック|2|AAD でデバイスをブロックします。|
|退職|3|デバイスを破棄します。|
|ワイプ|4|デバイスをワイプします。|
|removeResourceAccessProfiles|5|デバイスからリソースのアクセス ・ プロファイルを削除します。|
|pushNotification|9|デバイスにプッシュ通知を送信します。|
|remoteLock|10|リモートでデバイスをロックします。|




