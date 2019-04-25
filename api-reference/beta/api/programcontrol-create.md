---
title: programcontrol を作成する
description: Azure AD access レビュー機能で、新しい programcontrol オブジェクトを作成します。  これにより、アクセスレビューがプログラムにリンクされます。
localization_priority: Normal
ms.openlocfilehash: 89e31994ea91dba68e2f4563c64eeab53dd4db93
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546440"
---
# <a name="create-programcontrol"></a>programcontrol を作成する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD [access レビュー](../resources/accessreviews-root.md)機能で、新しい[programcontrol](../resources/programcontrol.md)オブジェクトを作成します。  これにより、アクセスレビューがプログラムにリンクされます。

この要求を行う前に、発信者が以前に

 - の`programId`値を要求に含めるには、[プログラムを作成](program-create.md)するか、[プログラムを取得](program-list.md)しました。
 - の`controlId`値を要求に含めるために、[アクセスレビューを作成](accessreview-create.md)するか、[アクセスレビューを取得](accessreview-get.md)しました。
 - の`controlTypeId`値を要求に含めるために、[プログラムコントロールの種類の一覧を取得](programcontroltype-list.md)しました。


## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | `ProgramControl.ReadWrite.All`.  また、サインインしているユーザーは、programcontrol を作成できるようにするために、ディレクトリロールにある必要があります。 |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 型        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー \{トークン\}。必須。 |

## <a name="request-body"></a>要求本文
要求本文で、 [programcontrol](../resources/programcontrol.md)オブジェクトの JSON 表記を指定します。

次の表に、プログラムコントロールの作成時に必要なプロパティを示します。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
| `programId`              |`String`                | このコントロールが一部になるプログラムの programid。                             |
| `controlId`              |`String`                | コントロールの controlId (特にアクセスレビューの識別子)。                                                |
| `controlTypeId`          |`String`                | programcontroltype には、プログラムコントロールの種類を指定します。たとえば、ゲストアクセスレビューにリンクしているコントロールがあります。 |

## <a name="response"></a>応答
成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[programcontrol](../resources/programcontrol.md)オブジェクトを返します。


## <a name="example"></a>例
##### <a name="request"></a>要求
要求本文で、 [programcontrol](../resources/programcontrol.md)オブジェクトの JSON 表記を指定します。

<!-- {
  "blockType": "request",
  "name": "create_programControl_from_programControls"
}-->
```http
POST https://graph.microsoft.com/beta/programControls
Content-type: application/json

{
    "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
}
```

##### <a name="response"></a>応答
>**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "63b2302c-7e62-43b7-aefb-063ba5bdb853",
  "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
  "displayName": "test",
  "status": "Active",
  "createdDateTime": "2018-05-18T20:26:05.2976279Z"
}
```

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[programcontroltypes のリスト](../api/programcontroltype-list.md) | [programcontroltype](../resources/programcontroltype.md)コレクション| プログラムコントロールの種類を一覧表示します。 |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
