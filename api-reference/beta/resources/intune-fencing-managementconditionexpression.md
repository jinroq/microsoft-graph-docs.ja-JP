---
title: managementconditionexpression リソースの種類
description: 管理条件式は、評価時にブール値を生成する式です。つまり、true または false のいずれかで、管理条件ステートメントがアクティブ化/非アクティブ化されたことを示します。 管理条件式は、式の変数とブール値の式の演算子の組み合わせで構成できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b102fe5d23a3a6dddadbf569ac9b15817a5947e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568746"
---
# <a name="managementconditionexpression-resource-type"></a>managementconditionexpression リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

管理条件式は、評価時にブール値を生成する式です。つまり、true または false のいずれかで、管理条件ステートメントがアクティブ化/非アクティブ化されたことを示します。 管理条件式は、式の変数とブール値の式の演算子の組み合わせで構成できます。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpression"
}
```





