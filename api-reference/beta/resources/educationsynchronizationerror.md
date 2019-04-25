---
title: educationSynchronizationError リソースの種類
description: school data profile validation または sync の間に発生したエラーを表します。azure Active Directory (azure AD) との検証や同期を失敗したすべてのエントリに対して一意のエラーが生成されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 5c937e95441132e4633b0f5e48a75b0597b8f08d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542966"
---
# <a name="educationsynchronizationerror-resource-type"></a>educationSynchronizationError リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

school data profile validation または sync の間に発生したエラーを表します。azure Active Directory (azure AD) との検証や同期を失敗したすべてのエントリに対して一意のエラーが生成されます。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-|:-|:-|
| [同期エラーを取得する](../api/educationsynchronizationerrors-get.md) | **educationSynchronizationError**コレクション| プロファイルに関連付けられている同期エラーのリストを返します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **entrytype** | string |  同期エンティティ (school、section、student、教師) を表します。       |
| **errorCode** | string |  このエラーのエラーコードを表します。         |
| **errorMessage** | string |  エラーの説明を格納します。        |
| **joiningvalue** | string |  エントリの一意識別子。         |
| **recordedDateTime** | DateTimeOffset | このエラーが発生した時刻。         |
| **reportableidentifier** | string | このエラーエントリの識別子。       |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSynchronizationError"
}-->

```json
{
    "entryType": "String",
    "errorCode": "String",
    "errorMessage": "String",
    "joiningValue": "String",
    "recordedDateTime": "DateTimeOffset",
    "reportableIdentifier": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationerror.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
