---
title: CalendarGroup を更新する
description: calendargroup オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 14254395e69054e3ba6f1a9141746c4e71360eb0
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35443722"
---
# <a name="update-calendargroup"></a>CalendarGroup を更新する

calendargroup オブジェクトのプロパティを更新します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
| :------------------------------------- | :------------------------------------------ |
| 委任 (職場または学校のアカウント)     | Calendars.ReadWrite                         |
| 委任 (個人用 Microsoft アカウント) | Calendars.ReadWrite                         |
| アプリケーション                            | Calendars.ReadWrite                         |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。

```http
PATCH /me/calendarGroups/{id}
PATCH /users/{id | userPrincipalName}/calendarGroups/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー        | 値                       |
| :------------ | :-------------------------- |
| Authorization | ベアラー {トークン}。必須。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>要求本文

要求本文で、更新する関連フィールドの値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。

| プロパティ | 型   | 説明     |
| :------- | :----- | :-------------- |
| name     | String | グループの名前。 |

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された[予定表グループ](../resources/calendargroup.md) オブジェクトを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_calendargroup"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/me/calendarGroups/{id}
Content-type: application/json
Content-length: 30

{
  "name": "name-value"
}
```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-calendargroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-calendargroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-calendargroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendarGroup"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 110

{
  "name": "name-value",
  "classId": "11b0131d-43c8-4bbb-b2c8-e80f9a50834a",
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Update calendargroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
