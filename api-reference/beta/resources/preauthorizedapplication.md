---
title: preAuthorizedApplication リソースの種類
description: アプリケーションおよび暗黙の同意を要求されたアクセス許可を表します。 管理者がアプリケーションに同意を提供する必要があります。 preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意するものは必要ありません。 PreAuthorizedApplications に記載されているアクセス許可では、ユーザーの同意は必要ありません。 ただし、preAuthorizedApplications に記載されていない追加の要求されたアクセス許可は、ユーザーの同意を必要とします。
ms.openlocfilehash: d299aefcac541407e0e42d0b0933e903afa3e84d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074094"
---
# <a name="preauthorizedapplication-resource-type"></a>preAuthorizedApplication リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

アプリケーションおよび暗黙の同意を要求されたアクセス許可を表します。 管理者がアプリケーションに同意を提供する必要があります。 preAuthorizedApplications では、ユーザーが要求されたアクセス許可に同意するものは必要ありません。 PreAuthorizedApplications に記載されているアクセス許可では、ユーザーの同意は必要ありません。 ただし、preAuthorizedApplications に記載されていない追加の要求されたアクセス許可は、ユーザーの同意を必要とします。

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|appId|文字列型 (String)| アプリケーションの一意の識別子です。 |
|permissionIds|String コレクション| [PublishedPermissionScope](permissionscope.md)または[エンティティ](approle.md)は、アプリケーションのいずれかの一意の識別子が必要です。 |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->