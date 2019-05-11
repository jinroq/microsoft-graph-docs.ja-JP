---
title: roleAssignmentScopeType 列挙型
description: 役割の割り当てのスコープの種類を指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: faf0b7ea9cabde19746d4741f2a22583930aa31e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940002"
---
# <a name="roleassignmentscopetype-enum-type"></a>roleAssignmentScopeType 列挙型

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

役割の割り当てのスコープの種類を指定します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|resourceScope|.0|指定した ResourceScopes への割り当てを許可します。|
|allDevices|1-d|すべての Intune デバイスへの割り当てを許可します。|
|allLicensedUsers|pbm-2|Intune にライセンスされたすべてのユーザーへの割り当てを許可します。|
|allDevicesAndLicensedUsers|1/3|すべての Intune デバイスおよびライセンスされたユーザーへの割り当てを許可します。|




