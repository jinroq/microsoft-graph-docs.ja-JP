---
title: educationFileSynchronizationVerificationMessage リソースの種類
description: CSV ベースの学校データプロファイルの同期を開始する要求に対する応答としてクライアントに返されるエラーを表します。 リソースには、検証結果のエラーが含まれています。 Azure Active Directory (Azure AD) と同期するには、要求を再起動する前に、ソースデータを修正する必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: cf462873226ff4238f95ffc4798b6eb662666f3d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006410"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>educationFileSynchronizationVerificationMessage リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

CSV ベースの学校データプロファイルの[同期を開始](../api/educationsynchronizationprofile-start.md)する要求に対する応答としてクライアントに返されるエラーを表します。 リソースには、検証結果のエラーが含まれています。 Azure Active Directory (Azure AD) と同期するには、要求を再起動する前に、ソースデータを修正する必要があります。

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
