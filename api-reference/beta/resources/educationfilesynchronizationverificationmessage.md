---
title: educationFileSynchronizationVerificationMessage リソースの種類
description: CSV ベースの学校データプロファイルの同期を開始する要求に対する応答としてクライアントに返されるエラーを表します。 リソースには、検証結果のエラーが含まれています。 azure Active Directory (azure AD) と同期するには、要求を再起動する前に、ソースデータを修正する必要があります。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 26f96c83ce14539011664b446265328f714ed402
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32507132"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>educationFileSynchronizationVerificationMessage リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

CSV ベースの学校データプロファイルの[同期を開始](../api/educationsynchronizationprofile-start.md)する要求に対する応答としてクライアントに返されるエラーを表します。 リソースには、検証結果のエラーが含まれています。 azure Active Directory (azure AD) と同期するには、要求を再起動する前に、ソースデータを修正する必要があります。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **type** | string | メッセージの種類。 使用可能な値は、`error`、`warning`、`information` です。 | 
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfilesynchronizationverificationmessage.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
