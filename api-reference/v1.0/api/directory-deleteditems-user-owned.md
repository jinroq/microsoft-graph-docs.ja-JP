---
title: Permissions
description: '指定されたユーザーによって所有されている、最近削除したアイテムの一覧を取得します。  '
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 2c4dfb7300d75ec066cf7c76c582d7bc4014e27a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27890084"
---
# <a name="list-deleted-items-owned-by-a-user"></a>**ユーザーによって所有されている削除済みのアイテムを一覧表示します。**

指定されたユーザーによって所有されている、最近削除したアイテムの一覧を取得します。  

現在、削除されたリスト アイテムの機能はユーザーによって所有されているリソースを[グループ化](../resources/group.md)します。

これは、改ページ調整がサポートされていないこと、サービスの操作です。  API が ID で並べ替えて、ユーザーが所有する最大 1,000 の削除されたオブジェクトを返します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)」を参照してください。

| アクセス許可の種類 | アクセス許可 (特権の小さいものから大きいものへ) |
| --- | --- |
| 委任 (職場または学校のアカウント) | Group.Read.All、Group.ReadWrite.All |
| 委任 (個人用 Microsoft アカウント) |  サポートされていません。 |
| アプリケーション | Group.Read.All、Group.ReadWrite.All  |

## <a name="http-request"></a>HTTP 要求

``` http
POST /directory/deletedItems/getUserOwnedObjects
```

## <a name="request-headers"></a>要求ヘッダー

| 名前          | 説明               |
| ------------- | ------------------------- |
| Authorization | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

```json
{
  "userId":"{id}",
  "type":"Group"
}
```

要求の本体には、次のパラメーターが必要です。

| Parameter    | Type |説明|
|:---------------|:--------|:----------|
|userId|String|所有者の ID です。|
|type|String|返される所有しているオブジェクトの種類`Group`は、現在サポートされている値だけです。|


## <a name="response"></a>応答

成功した要求を返す`200 OK`応答コードです。応答オブジェクトには、[ディレクトリ (削除済みアイテム)](../resources/directory.md)のプロパティが含まれています。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。

``` http
POST https://graph.microsoft.com/v1.0/directory/deletedItems/getUserOwnedObjects
Content-type: application/json
```

``` json
{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a>応答

以下は、応答の例です。 注: この応答オブジェクトを簡潔にするためにあります。 サポートされているすべてのプロパティは、実際の呼び出しから返されます。

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": 2018-04-01T12:39:16Z,
              "classification": null,
              "createdDateTime": "2017-03-22T12:39:16Z",
              "description": null,
              "displayName": "Test",
              "groupTypes": [
                  "Unified"
              ],
              "mail": "Test@contoso.com",
              "mailEnabled": true,
              "mailNickname": "Test",
              "membershipRule": null,
              "membershipRuleProcessingState": null,
              "preferredDataLocation": null,
              "preferredLanguage": null,
              "proxyAddresses": [
                  "SMTP:Test@contoso.com"
              ],
              "renewedDateTime": "2017-09-22T22:30:39Z",
              "securityEnabled": false,
              "theme": null,
              "visibility": "Public"
          } 
        ]
 }
```


