---
title: deviceComplianceActionType 列挙型
description: 列挙型の操作をスケジュールします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 92e43378f119a5e1a10604babb5ad23b2dfddf3b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851437"
---
# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 列挙型

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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



