---
title: ポリシーの削除
description: ポリシーを削除します。
localization_priority: Normal
ms.openlocfilehash: e4e5f5372e2904e1f74bc25224e3d2b1ce7ba154
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538731"
---
# <a name="delete-policy"></a>ポリシーの削除

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[ポリシー](../resources/policy.md)を削除します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

```http
DELETE /policies/{id}
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:---------------|:--------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。 失敗した場合...

## <a name="example"></a>例
次の例では、ポリシーを削除します。

##### <a name="request"></a>要求
以下は、要求の例です。

```http
DELETE https://graph.microsoft.com/beta/policies/{id}
```

##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

```http
HTTP/1.1 204 No Content
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/policy-delete.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
