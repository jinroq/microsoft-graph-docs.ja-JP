---
title: educationSynchronizationError リソースの種類
description: 学校データ プロファイルの検証との同期中にエラーを表します。検証や Azure Active Directory (AD の Azure) との同期に失敗したすべてのエントリに対して一意のエラーが生成されます。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 2808ba0fd633fcdcbbaa32ce63162ac1cd4531ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944727"
---
# <a name="educationsynchronizationerror-resource-type"></a>educationSynchronizationError リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

学校データ プロファイルの検証との同期中にエラーを表します。検証や Azure Active Directory (AD の Azure) との同期に失敗したすべてのエントリに対して一意のエラーが生成されます。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-|:-|:-|
| [同期エラーが発生をします。](../api/educationsynchronizationerrors-get.md) | **educationSynchronizationError**コレクション| プロファイルに関連付けられている同期エラーの一覧を返します。 |

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **示した** | 文字列 |  (学校、セクション、学生、教師) は、同期エンティティを表します。       |
| **errorCode** | 文字列 |  このエラーのエラー コードを表します。         |
| **エラー メッセージ** | 文字列 |  エラーの説明が含まれています。        |
| **joiningValue** | 文字列 |  エントリの一意の識別子です。         |
| **recordedDateTime** | DateTimeOffset | このエラーの発生時刻。         |
| **reportableIdentifier** | 文字列 | このエラーのエントリの識別子です。       |

## <a name="json-representation"></a>JSON 表記
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "#microsoft.graph.educationSynchronizationError"
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
