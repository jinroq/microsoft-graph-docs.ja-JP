---
title: deviceComplianceActionType 列挙型
description: 列挙型の操作をスケジュールします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1856847cb8a8ecf48ee6d13067bd24515326d89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973210"
---
# <a name="devicecomplianceactiontype-enum-type"></a>deviceComplianceActionType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

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
|remoteLock|10|リモートでデバイスをロックします。|





