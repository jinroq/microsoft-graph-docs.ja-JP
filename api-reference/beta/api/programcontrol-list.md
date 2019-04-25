---
title: programcontrols のリスト
description: Azure AD access レビュー機能で、すべての programcontrol オブジェクトを、テナント内のすべてのプログラムで一覧表示します。
localization_priority: Normal
ms.openlocfilehash: 52361e3878445d4f739fd0cd33817d5b254ddc03
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546429"
---
# <a name="list-programcontrols"></a>programcontrols のリスト

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、すべての[programcontrol](../resources/programcontrol.md)オブジェクトを、テナント内のすべてのプログラムで一覧表示します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | `ProgramControl.Read.All`, `ProgramControl.ReadWrite.All`.  サインインしているユーザーは、プログラムを読み取ることができるようにする必要があります。 |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
GET /programControls
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー \{トークン\}。必須。 |

## <a name="request-body"></a>要求本文
要求本文を指定する必要はありません。

## <a name="response"></a>応答
成功した場合、このメソッド`200, OK`は応答コードと、応答本文で[programcontrol](../resources/programcontrol.md)オブジェクトの配列を返します。

## <a name="example"></a>例
##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "get_programControl"
}-->
```http
GET https://graph.microsoft.com/beta/programControls
```

##### <a name="response"></a>応答
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl",
    "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{

    "value": [
        {
            "id": "f6abf8ef-a05e-4788-adc9-5af909c400af",
            "controlId": "bc81d51d-be53-4606-a8c2-f90a2beb5f40",
            "programId": "673a7379-9c38-4f01-bd9d-4fda7260b807",
            "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
            "displayName": "guest user review",
            "status": "Completed",
            "createdDateTime": "2017-09-20T20:18:05.1318394Z"
        }
    ]
}

```

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[プログラムの programcontrols を一覧表示する](program-listcontrols.md) |     [programcontrol](../resources/programcontrol.md)コレクション|    プログラムのコントロールのコレクションを取得します。|


<!--
{
  "type": "#page.annotation",
  "description": "List programControls",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
