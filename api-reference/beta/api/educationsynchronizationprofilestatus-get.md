---
title: educationSynchronizationProfile の状態を取得する
description: テナント内の特定の学校データ同期プロファイルの状態を取得します。 応答は、同期の状態を示します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: e3806102480fc6d8bbb408fab31724b78205ab59
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33324414"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a>educationSynchronizationProfile の状態を取得する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)の状態を取得します。 応答は、同期の状態を示します。

## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類 | アクセス許可 (特権の小さいものから大きいものへ) |
|:-----------|:----------|
| 委任 (職場または学校のアカウント) | EduAdministration、EduAdministration |
|委任 (個人 Microsoft アカウント|サポートされていません。|
|アプリケーション| EduAdministration、EduAdministration のいずれかを取得します。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a>要求ヘッダー
| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。  |

## <a name="request-body"></a>要求本文
このメソッドには、要求本文を指定しません。
## <a name="response"></a>応答
成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md)オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a>応答
応答の例を次に示します。 

>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
}
```
