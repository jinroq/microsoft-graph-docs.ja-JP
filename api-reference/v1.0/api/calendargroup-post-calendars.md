---
title: 予定表を作成する
description: この API を使って、ユーザー用の予定表グループに新しい予定表を作成します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 791615d7b934536a27d4a8d1ea88be42a4ca2d79
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928452"
---
# <a name="create-calendar"></a>予定表を作成する

この API を使って、[ユーザー](../resources/user.md)用の予定表グループに新しい予定表を作成します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
| :------------------------------------- | :------------------------------------------ |
| 委任 (職場または学校のアカウント)     | Calendars.ReadWrite                         |
| 委任 (個人用 Microsoft アカウント) | Calendars.ReadWrite                         |
| アプリケーション                            | Calendars.ReadWrite                         |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

ユーザーの既定 [calendarGroup](../resources/calendargroup.md)。

```http
POST /me/calendarGroup/calendars
POST /users/{id | userPrincipalName}/calendarGroup/calendars
```

ユーザーの任意の [calendarGroup](../resources/calendargroup.md)。

```http
POST /me/calendarGroups/{id}/calendars
POST /users/{id | userPrincipalName}/calendarGroups/{id}/calendars
```

## <a name="request-headers"></a>要求ヘッダー

| ヘッダー        | 値                       |
| :------------ | :-------------------------- |
| Authorization | ベアラー {トークン}。必須。   |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>要求本文

要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。

## <a name="response"></a>応答

成功した場合、このメソッドは応答本文で `201 Created` 応答コードと [予定表](../resources/calendar.md)オブジェクトを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。

<!-- {
  "blockType": "request",
  "name": "create_calendar_from_calendargroup"
}-->

```http
POST https://graph.microsoft.com/v1.0/me/calendarGroups/{id}/calendars
Content-type: application/json
Content-length: 78

{
  "name": "name-value",
  "color": {
  }
}
```

要求本文で、[予定表](../resources/calendar.md) オブジェクトの JSON 表記を指定します。

##### <a name="response"></a>応答

以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.calendar"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 98

{
  "name": "name-value",
  "color": {
  },
  "changeKey": "changeKey-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->

<!-- {
  "type": "#page.annotation",
  "description": "Create Calendar",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
