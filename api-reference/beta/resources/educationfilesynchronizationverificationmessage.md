---
title: educationFileSynchronizationVerificationMessage リソースの種類
description: CSV ベースの学校データプロファイルの同期を開始する要求に対する応答としてクライアントに返されるエラーを表します。 リソースには、検証結果のエラーが含まれています。 azure Active Directory (azure AD) と同期するには、要求を再起動する前に、ソースデータを修正する必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: bbf38f15fbe14112ef254c625a8747e57eb1cae4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340523"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>educationFileSynchronizationVerificationMessage リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

CSV ベースの学校データプロファイルの[同期を開始](../api/educationsynchronizationprofile-start.md)する要求に対する応答としてクライアントに返されるエラーを表します。 リソースには、検証結果のエラーが含まれています。 azure Active Directory (azure AD) と同期するには、要求を再起動する前に、ソースデータを修正する必要があります。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **type** | string | メッセージの種類。 可能な値は、`error`、`warning`、`information` です。 | 
| **filename** | string | エラーを含むソースファイル。 |
| **説明** | string | メッセージの種類に関する詳細情報。 |

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileSynchronizationVerificationMessage"
}-->

```json
{
    "type": "String",
    "fileName": "String",
    "description": "String"
}
```
