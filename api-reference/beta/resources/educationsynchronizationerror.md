---
title: educationSynchronizationError リソースの種類
description: 学校データ プロファイルの検証との同期中にエラーを表します。検証や Azure Active Directory (AD の Azure) との同期に失敗したすべてのエントリに対して一意のエラーが生成されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 397ac305fcacd789174c05ea36ab026826227475
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425814"
---
# <a name="educationsynchronizationerror-resource-type"></a>educationSynchronizationError リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

学校データ プロファイルの検証との同期中にエラーを表します。検証や Azure Active Directory (AD の Azure) との同期に失敗したすべてのエントリに対して一意のエラーが生成されます。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-|:-|:-|
| [同期エラーが発生をします。](../api/educationsynchronizationerrors-get.md) | **educationSynchronizationError**コレクション| プロファイルに関連付けられている同期エラーの一覧を返します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **示した** | string |  (学校、セクション、学生、教師) は、同期エンティティを表します。       |
| **errorCode** | string |  このエラーのエラー コードを表します。         |
| **エラー メッセージ** | string |  エラーの説明が含まれています。        |
| **joiningValue** | string |  エントリの一意の識別子です。         |
| **recordedDateTime** | DateTimeOffset | このエラーの発生時刻。         |
| **reportableIdentifier** | string | このエラーのエントリの識別子です。       |

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
