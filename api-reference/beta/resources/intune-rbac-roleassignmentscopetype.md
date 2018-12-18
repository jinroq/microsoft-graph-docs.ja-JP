---
title: roleAssignmentScopeType 列挙型
description: 役割の割り当てのスコープの種類を指定します。
author: tfitzmac
ms.openlocfilehash: 0a3286b3b7bc583323204ca39ff85e01869ddbe7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343128"
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





