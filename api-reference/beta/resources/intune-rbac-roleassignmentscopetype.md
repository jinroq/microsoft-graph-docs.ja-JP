---
title: roleAssignmentScopeType 列挙型
description: 役割の割り当てのスコープの種類を指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d9659c4eaa1f4080ef5dd07a5e69f76a7a14d50
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573054"
---
# <a name="roleassignmentscopetype-enum-type"></a>roleAssignmentScopeType 列挙型

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

役割の割り当てのスコープの種類を指定します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|resourcescope|.0|指定した ResourceScopes への割り当てを許可します。|
|alldevices|1 |すべての Intune デバイスへの割り当てを許可します。|
|allLicensedUsers|2 |Intune にライセンスされたすべてのユーザーへの割り当てを許可します。|
|allDevicesAndLicensedUsers|3 |すべての Intune デバイスおよびライセンスされたユーザーへの割り当てを許可します。|





