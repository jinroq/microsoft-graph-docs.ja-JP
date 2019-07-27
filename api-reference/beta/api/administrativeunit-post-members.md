---
title: メンバーを追加する
description: この API を使用して、管理単位にメンバー (ユーザーまたはグループ) を追加します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a86fc2eaccb318164b91b8101577b4e3ffd64fbe
ms.sourcegitcommit: 27e8ddb53b699f70b676c9648db8f06bb8d831a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/27/2019
ms.locfileid: "35918014"
---
# <a name="add-a-member"></a>メンバーを追加する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

この API を使用して、管理単位にメンバー (ユーザーまたはグループ) を追加します。

`NOTE: Currently it's only possible to add one member at a time to an administrative unit.`

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。


|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | AdministrativeUnit。すべての Directory.accessasuser.all について    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | AdministrativeUnit |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /administrativeUnits/{id}/members/$ref
```
## <a name="request-headers"></a>要求ヘッダー
| 名前      |説明|
|:----------|:----------|
| Authorization  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、追加する[ユーザー](../resources/user.md)、[グループ](../resources/group.md)、または[directoryobject](../resources/directoryobject.md)の JSON 表記を指定します。

## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。

```http
POST https://graph.microsoft.com/beta/administrativeUnits/{id}/members/$ref
Content-type: application/json
Content-length: 109

{
  "@odata.id":"https://graph.microsoft.com/beta/groups/{id}"
}

```
要求本文で、追加する[ユーザー](../resources/user.md)または[グループ](../resources/group.md)オブジェクト`id`の JSON 表記を指定します。

##### <a name="response"></a>応答
以下は、応答の例です。
 
```http
HTTP/1.1 204 No Content
```
