---
title: roleAssignmentScopeType 列挙型
description: 役割の割り当てのスコープの種類を指定します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b815cf7eb396aa82f49df792ceee0612678077c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419892"
---
# <a name="roleassignmentscopetype-enum-type"></a>roleAssignmentScopeType 列挙型

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

役割の割り当てのスコープの種類を指定します。

## <a name="members"></a>メンバー
|メンバー|値|説明|
|:---|:---|:---|
|resourceScope|0|指定された ResourceScopes への割り当てを許可します。|
|しています。|1|Intune のすべてのデバイスへの割り当てを許可します。|
|allLicensedUsers|2|Intune にライセンスのすべてのユーザーへの割り当てを許可します。|
|allDevicesAndLicensedUsers|3|Intune デバイスおよびライセンスを受けたユーザーのすべての割り当てを許可します。|




