---
title: educationSynchronizationError リソースの種類
description: School data profile validation または sync の間に発生したエラーを表します。Azure Active Directory (Azure AD) との検証や同期を失敗したすべてのエントリに対して一意のエラーが生成されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 11e5be9893c6a50615774e0d2a8e4d51c9576da6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972412"
---
# <a name="educationsynchronizationerror-resource-type"></a>educationSynchronizationError リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

School data profile validation または sync の間に発生したエラーを表します。Azure Active Directory (Azure AD) との検証や同期を失敗したすべてのエントリに対して一意のエラーが生成されます。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-|:-|:-|
| [同期エラーを取得する](../api/educationsynchronizationerrors-get.md) | **educationSynchronizationError**コレクション| プロファイルに関連付けられている同期エラーのリストを返します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **entryType** | string |  同期エンティティ (school、section、student、教師) を表します。       |
| **errorCode** | string |  このエラーのエラーコードを表します。         |
| **errorMessage** | string |  エラーの説明を格納します。        |
| **joiningValue** | string |  エントリの一意識別子。         |
| **recordedDateTime** | DateTimeOffset | このエラーが発生した時刻。         |
| **reportableIdentifier** | string | このエラーエントリの識別子。       |

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
