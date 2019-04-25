---
title: プログラムを作成する
description: Azure AD access レビュー機能で、新しいプログラムオブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: a6e9ab300cf44a2f3973c468679af7fa48262680
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538540"
---
# <a name="create-program"></a>プログラムを作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、新しい[プログラム](../resources/program.md)オブジェクトを作成します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | `ProgramControl.ReadWrite.All`.  サインインしているユーザーは、プログラムを作成することを許可するディレクトリロールにある必要があります。 |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー \{トークン\}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。

次の表に、プログラムの作成時に必要なプロパティを示します。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  プログラムの名前を指定します。                   |
| `description`               |`String`                              |  プログラムの説明。           |


## <a name="response"></a>応答
成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[プログラム](../resources/program.md)オブジェクトを返します。

## <a name="example"></a>例
##### <a name="request"></a>要求
要求本文で、[プログラム](../resources/program.md)オブジェクトの JSON 表記を指定します。

<!-- {
  "blockType": "request",
  "name": "create_program_from_programs"
}-->
```http
POST https://graph.microsoft.com/beta/programs
Content-type: application/json

{
    "displayName": "testprogram3",
    "description": "test description"
}
```

##### <a name="response"></a>応答
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3",
    "description": "test description"
}
```

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[プログラムの一覧表示](program-list.md) | [プログラム](../resources/program.md)コレクション|  すべてのプログラムのコレクションを取得します。|
|[プログラムの programcontrols を一覧表示する](program-listcontrols.md) |     [programcontrol](../resources/programcontrol.md)コレクション|    プログラムのコントロールのコレクションを取得します。|
|[プログラムの更新](program-update.md) |  [アプリケーション](../resources/program.md)| プログラムを更新します。|
|[programcontrol を作成する](programcontrol-create.md) |        [programcontrol](../resources/programcontrol.md)    |   プログラムに programcontrol を追加します。|

<!--
{
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
