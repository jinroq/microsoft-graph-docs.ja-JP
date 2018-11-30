---
title: educationFileSynchronizationVerificationMessage リソースの種類
description: CSV ベースの学校のデータのプロファイルの同期を開始する要求への応答としてクライアントに返されるエラーを表します。 リソースの検証エラーが含まれます。 ユーザーは Azure Active Directory (AD の Azure) との同期を要求を再起動する前にソース データを修正する必要があります。
ms.openlocfilehash: cf685e0619c5600340df68ba86ecaef11a8a435d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066861"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>educationFileSynchronizationVerificationMessage リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

CSV ベースの学校のデータのプロファイルの[同期の開始](../api/educationsynchronizationprofile-start.md)を要求への応答としてクライアントに返されるエラーを表します。 リソースの検証エラーが含まれます。 ユーザーは Azure Active Directory (AD の Azure) との同期を要求を再起動する前にソース データを修正する必要があります。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:-|:-|:-|
| **type** | string | メッセージの種類です。 可能な値は、`error`、`warning`、`information` です。 | 
| filename | 文字列 | エラーを含むソース ファイルです。 |
| **description** | 文字列 | メッセージの種類に関する詳細な情報。 |

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