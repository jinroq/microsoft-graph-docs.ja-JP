---
title: 'グループ: checkMemberGroups'
description: 指定したグループ一覧内のメンバーシップを確認します。 リストからそのグループを返します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 1815f187a25eaddbd3b1757fde5e7e4e9c74f650
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329649"
---
# <a name="group-checkmembergroups"></a>グループ: checkMemberGroups

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

指定したグループ一覧内のメンバーシップを確認します。指定したグループがダイレクト メンバーシップまたは推移性メンバーシップを持つグループを一覧から返します。

要求ごとに、最大 20 のグループを確認できます。この関数は、Office 365 と Azure AD でプロビジョニングされた他の種類のグループをサポートしています。Office 365 グループにはグループを含めることはできませんのでご注意ください。そのため、Office 365 グループのメンバーシップは常にダイレクト メンバーシップです。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)                                                 |
| :------------------------------------- | :------------------------------------------------------------------------------------------ |
| 委任 (職場または学校のアカウント)     | ~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。                                                                              |
| アプリケーション                            | ~~Group.Read.All~~、Directory.Read.All、Directory.ReadWrite.All                             |

> **注:** 現在この API には、`Directory.Read.All` 以上のアクセス許可が必要です。 `Group.Read.All`のアクセス許可を使用すると、エラーが返されます。 これは既知のバグです。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
POST /groups/{id}/checkMemberGroups
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 型   | 説明               |
| :------------ | :----- | :------------------------ |
| Authorization | string | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。

| パラメーター | 型   | 説明           |
| :-------- | :----- | :-------------------- |
| groupIds  | String collection | グループ ID の配列 |

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で文字列コレクション オブジェクトを返します。

## <a name="example"></a>例

以下は、この API を呼び出す方法の例です。

##### <a name="request"></a>要求

以下は、要求の例です。

<!-- {
  "blockType": "request",
  "name": "group_checkmembergroups"
}-->

```http
POST https://graph.microsoft.com/beta/groups/{id}/checkMemberGroups
Content-type: application/json
Content-length: 44

{
  "groupIds": [
    "groupIds-value"
  ]
}
```

##### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "value": [
    "string-value"
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!--
{
  "type": "#page.annotation",
  "description": "group: checkMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
