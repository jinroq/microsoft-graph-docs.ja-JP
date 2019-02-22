---
title: androidpermissionaction リソースの種類
description: android アプリのアクセス許可と android のアクションとの間のマッピングは、そのアクセス許可が要求されたときに行われる必要があります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e00bb351f2eff093dee21cb393ba622bc5e29ea9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30161573"
---
# <a name="androidpermissionaction-resource-type"></a>androidpermissionaction リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

android アプリのアクセス許可と android のアクションとの間のマッピングは、そのアクセス許可が要求されたときに行われる必要があります。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|アクセス許可|String|android のアクセス許可文字列。公式の android ドキュメントで定義されています。  例 ' READ_CONTACTS '。|
|action|[androidpermissionactiontype](../resources/intune-apps-androidpermissionactiontype.md)|Android のアクセス許可アクションの種類。 可能な値は、`prompt`、`autoGrant`、`autoDeny` です。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidPermissionAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidPermissionAction",
  "permission": "String",
  "action": "String"
}
```




