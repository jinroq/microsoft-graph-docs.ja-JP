---
title: リスト privilegedOperationEvents
description: フィルター ' の式です。
ms.openlocfilehash: c18e00086ae92610cdc05e31d9f04ecf7e5d5c48
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072053"
---
# <a name="list-privilegedoperationevents"></a>リスト privilegedOperationEvents

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

ロールの操作の権限を持つ Id 管理によって生成される監査イベントを表す[privilegedOperationEvent](../resources/privilegedoperationevent.md)オブジェクトの一覧を取得します。 監査イベントの詳細については、 [privilegedOperationEvent](../resources/privilegedoperationevent.md)を参照してください。 クエリの結果をフィルターするには、標準の OData を使用して、``$filter``式です。


## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

リクエスターは、次のロールのいずれかを持つ必要があります:_ロールの権限を持つ管理者_、_グローバル管理者_、_セキュリティ管理者_、または_セキュリティのリーダー_です。

 

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedOperationEvents
```
## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター
このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。

## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文内の[privilegedOperationEvent](../resources/privilegedoperationevent.md)オブジェクトのコレクションです。

テナントの PIM を登録する必要があることに注意してください。 それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。
## <a name="examples"></a>例

### <a name="get-audit-events-for-role-assignment-operations"></a>ロールの割り当ての操作の監査イベントを取得します。
##### <a name="request"></a>要求
次の使用例は、ロールの割り当て操作の監査イベントを取得する要求を示しています。 この例では、``requestType``の値は、 ``Assign``。

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/beta/privilegedOperationEvents?$filter=requestType%20eq%20'Assign'
```
##### <a name="response"></a>応答
次の例は応答を示しています。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
    "value": [
        {
            "id": "201707240003469369",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f80",
            "userName": "admin1",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "9360feb5-f418-4baa-8175-e2a00bac4301",
            "roleName": "Directory Writers",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-24T18:32:38.7589078Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Assign",
            "additionalInformation": null,
            "referenceKey": null,
            "referenceSystem": null
        },
        {
            "id": "201707240003469372",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f80",
            "userName": "admin",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-24T18:33:00.7607701Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Assign",
            "additionalInformation": null,
            "referenceKey": null,
            "referenceSystem": null
        }
    ]
}
```
### <a name="get-audit-events-for-the-operations-of-self-role-activation-and-makepermanent"></a>自己の役割のアクティブ化および makePermanent の操作の監査イベントを取得します。
##### <a name="request"></a>要求
次の例では、自己の役割のアクティブ化および makePermanent の操作の監査イベントを取得する要求を示します。 この例では、``requestType``の値は、 ``Activate``。

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/beta/privilegedOperationEvents?$filter=requestType%20eq%20'Activate'
```
##### <a name="response"></a>応答
次の例は応答を示しています。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
    "value": [
        {
            "id": "201707240003469811",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "userName": "admin1",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "44367163-eba1-44c3-98af-f5787879f96a",
            "roleName": "CRM Service Administrator",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-24T23:34:41.9661094Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin1",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Activate",
            "additionalInformation": "Make permanent admin",
            "referenceKey": null,
            "referenceSystem": null
        },
        {
            "id": "201707240003469814",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "userName": "admin1",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "2017-07-25T00:37:07.3402169Z",
            "creationDateTime": "2017-07-24T23:37:08.0052112Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin1",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Activate",
            "additionalInformation": "self activate",
            "referenceKey": "",
            "referenceSystem": ""
        }
    ]
}
```

### <a name="get-audit-events-for-role-assignment-deactivation"></a>ロール割り当ての非アクティブ化のイベントの監査を取得します。
##### <a name="request"></a>要求
ロール割り当ての非アクティブ化のイベントの監査を取得する要求の例を次に示します。 この例では、``requestType``の値は、 ``Deactivate``。

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/beta/privilegedOperationEvents?$filter=requestType%20eq%20'Deactivate'
```
##### <a name="response"></a>応答
次の例は応答を示しています。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
    "value": [
        {
            "id": "201707240003469375",
            "userId": "2cf9eef8-bc67-4aa4-bb65-75cc9e5c3f80",
            "userName": "admin1",
            "userMail": "admin1@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-24T18:33:28.3408971Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin1",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Deactivate",
            "additionalInformation": "Make eligible admin",
            "referenceKey": null,
            "referenceSystem": null
        }
    ]
}
```
### <a name="get-audit-events-created-in-a-time-range"></a>時間の範囲で作成される監査イベントを取得します。
##### <a name="request"></a>要求 
時間の範囲で作成された監査イベントを取得する要求の例を次に示します。

<!-- { "blockType": "request" } -->
```http
GET https://graph.microsoft.com/beta/privilegedOperationEvents?$filter=(creationDateTime%20ge%202017-06-25T07:00:00Z)%20and%20(creationDateTime%20le%202017-07-25T17:30:17Z)&$count=true&$orderby=creationDateTime%20desc
```
##### <a name="response"></a>応答
次の例は応答を示しています。 注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。 実際の呼び出しではすべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedOperationEvent",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 547

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#privilegedOperationEvents",
    "@odata.count": 2,
    "value": [
        {
            "id": "201707250003471056",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "userName": "admin",
            "userMail": "admin@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "2017-07-25T17:38:49.5640383Z",
            "creationDateTime": "2017-07-25T16:38:50.3681771Z",
            "requestorId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "requestorName": "admin",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Activate",
            "additionalInformation": "activate test",
            "referenceKey": "",
            "referenceSystem": ""
        },
        {
            "id": "201707250003469896",
            "userId": "0f693614-c255-4cf5-92fa-74e770c656d8",
            "userName": "admin",
            "userMail": "admin@contoso.onmicrosoft.com",
            "roleId": "95e79109-95c0-4d8e-aee3-d01accf2d47b",
            "roleName": "Guest Inviter",
            "expirationDateTime": "0001-01-01T00:00:00Z",
            "creationDateTime": "2017-07-25T00:37:08.6172407Z",
            "requestorId": "6b61baec-bb80-4a8a-b8bd-fa5ba1f12386",
            "requestorName": "Azure AD PIM",
            "tenantId": "ef73ae8b-cc96-4325-9bd1-dc82594b0b40",
            "requestType": "Deactivate",
            "additionalInformation": "Expired",
            "referenceKey": "",
            "referenceSystem": ""
        }
    ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedOperationEvents",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
