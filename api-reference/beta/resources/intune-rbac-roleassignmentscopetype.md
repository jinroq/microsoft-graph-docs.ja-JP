---
title: roleAssignmentScopeType 列挙型
description: 役割の割り当てのスコープの種類を指定します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 738579fbd8bcda9ac438ada2f7746e020396d225
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871541"
---
# <a name="roleassignmentscopetype-enum-type"></a>roleAssignmentScopeType 列挙型

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

役割の割り当てのスコープの種類を指定します。
## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|resourceScope|0|指定された ResourceScopes への割り当てを許可します。|
|しています。|1|Intune のすべてのデバイスへの割り当てを許可します。|
|allLicensedUsers|2|Intune にライセンスのすべてのユーザーへの割り当てを許可します。|
|allDevicesAndLicensedUsers|3|Intune デバイスおよびライセンスを受けたユーザーのすべての割り当てを許可します。|





