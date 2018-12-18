---
title: educationFileSynchronizationVerificationMessage リソースの種類
description: CSV ベースの学校のデータのプロファイルの同期を開始する要求への応答としてクライアントに返されるエラーを表します。 リソースの検証エラーが含まれます。 ユーザーは Azure Active Directory (AD の Azure) との同期を要求を再起動する前にソース データを修正する必要があります。
author: mmast-msft
ms.openlocfilehash: f2826f779aac3ba41146b6677f3d1e0364be92a1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336065"
---
# <a name="educationfilesynchronizationverificationmessage-resource-type"></a>educationFileSynchronizationVerificationMessage リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

CSV ベースの学校のデータのプロファイルの[同期の開始](../api/educationsynchronizationprofile-start.md)を要求への応答としてクライアントに返されるエラーを表します。 リソースの検証エラーが含まれます。 ユーザーは Azure Active Directory (AD の Azure) との同期を要求を再起動する前にソース データを修正する必要があります。

## <a name="properties"></a>Properties

| プロパティ | 種類 | 説明 |
|:-|:-|:-|
| **type** | string | メッセージの種類です。 可能な値は、`error`、`warning`、`information` です。 | 
| **filename** | string | エラーを含むソース ファイルです。 |
| **description** | string | メッセージの種類に関する詳細な情報。 |

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