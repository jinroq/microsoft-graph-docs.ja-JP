---
title: アクセス許可
description: '指定したユーザーが所有している最近削除されたアイテムのリストを取得します。  '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 81afb6e3da6cd9ffb795c4e867c23177a24a5ed2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33325995"
---
# <a name="list-deleted-items-owned-by-a-user"></a>**ユーザーが所有する削除済みアイテムを一覧表示する**

指定したユーザーが所有している最近削除されたアイテムのリストを取得します。  

現時点では、削除済みアイテムのリスト機能は、ユーザーが所有する[グループ](../resources/group.md)リソースに対してのみサポートされています。

これは、サービスのアクションであり、改ページ処理をサポートしていないことを意味します。  API は、ユーザーが所有する最大1000の削除済みオブジェクトを ID で並べ替えて返します。

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

要求本文には、次のパラメーターが必要です。

| パラメーター    | 型 |説明|
|:---------------|:--------|:----------|
|userId|String|所有者の ID。|
|type|String|取得する、所有されているオブジェクトの種類。`group`は現在、サポートされている唯一の値です。|


## <a name="response"></a>応答

成功した`200 OK`要求は応答コードを返します。response オブジェクトには、[ディレクトリ (削除済みアイテム)](../resources/directory.md)のプロパティが含まれています。

## <a name="example"></a>例

##### <a name="request"></a>要求

以下は、要求の例です。

``` http
POST https://graph.microsoft.com/beta/directory/deletedItems/getUserOwnedObjects
Content-type: application/json

{
  "userId":"55ac777c-109e-4022-b58c-470c8fcb6892",
  "type":"group"
}
```

###### <a name="response"></a>応答

以下は、応答の例です。 注: この応答オブジェクトは、簡潔にするために切り詰められている場合があります。 サポートされているすべてのプロパティは、実際の呼び出しから返されます。

``` http
HTTP/1.1 200
Content-type: application/json
Content-length: 1249

{
"value": [
          {
              "@odata.type": "#microsoft.graph.group",
              "id": "bfa7033a-7367-4644-85f5-95aaf385cbd7",
              "deletedDateTime": "2018-04-01T12:39:16Z",
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


