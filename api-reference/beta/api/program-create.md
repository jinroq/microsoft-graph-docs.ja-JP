---
title: プログラムを作成します。
description: Azure AD のレビュー機能にアクセス、新しいプログラム オブジェクトを作成します。
localization_priority: Normal
ms.openlocfilehash: a6e9ab300cf44a2f3973c468679af7fa48262680
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521300"
---
# <a name="create-program"></a>プログラムを作成します。

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、新しい[プログラム](../resources/program.md)オブジェクトを作成します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | `ProgramControl.ReadWrite.All`.  サインインしているユーザーは、プログラムを作成することを許可するディレクトリの役割でもあります。 |
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
| Authorization | string | ベアラー トークン 必須です。 |

## <a name="request-body"></a>要求本文
要求の本文には、[プログラム](../resources/program.md)オブジェクトの JSON 表現を指定します。

プログラムを作成するときに必要なプロパティを次の表に示します。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  プログラムの名前です。                   |
| `description`               |`String`                              |  プログラムの説明です。           |


## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、 `201, Created` 、応答の本体で応答コードと[プログラム](../resources/program.md)のオブジェクトです。

## <a name="example"></a>例
##### <a name="request"></a>要求
要求の本文には、[プログラム](../resources/program.md)オブジェクトの JSON 表現を指定します。

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
|[プログラムを一覧表示](program-list.md) | [プログラム](../resources/program.md)のコレクション|  すべてのプログラムのコレクションを取得します。|
|[プログラムのリスト programControls](program-listcontrols.md) |     [デバッギング](../resources/programcontrol.md)コレクション|    プログラムのコントロールのコレクションを取得します。|
|[更新プログラム](program-update.md) |  [プログラム](../resources/program.md)| プログラムを更新します。|
|[デバッギングを作成します。](programcontrol-create.md) |        [デバッギング](../resources/programcontrol.md)    |   デバッギングをプログラムに追加します。|

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
