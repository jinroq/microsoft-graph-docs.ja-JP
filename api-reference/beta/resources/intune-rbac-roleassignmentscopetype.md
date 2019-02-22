---
title: roleAssignmentScopeType 列挙型
description: 役割の割り当てのスコープの種類を指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6089021851e3d953fce4874b11e343b4747adf40
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150695"
---
# <a name="roleassignmentscopetype-enum-type"></a>roleAssignmentScopeType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

役割の割り当てのスコープの種類を指定します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|resourcescope|.0|指定した ResourceScopes への割り当てを許可します。|
|alldevices|1-d|すべての Intune デバイスへの割り当てを許可します。|
|allLicensedUsers|pbm-2|Intune にライセンスされたすべてのユーザーへの割り当てを許可します。|
|allDevicesAndLicensedUsers|1/3|すべての Intune デバイスおよびライセンスされたユーザーへの割り当てを許可します。|




