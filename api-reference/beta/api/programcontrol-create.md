---
title: ProgramControl を作成する
description: Azure AD access レビュー機能で、新しい programControl オブジェクトを作成します。  これにより、アクセスレビューがプログラムにリンクされます。
localization_priority: Normal
ms.openlocfilehash: dafaf94d00ca44159d474078f8dcce3b8de3e670
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35875344"
---
# <a name="create-programcontrol"></a>ProgramControl を作成する

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
|委任 (職場または学校のアカウント)     | ProgramControl.ReadWrite.All  |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            |  ProgramControl.ReadWrite.All  |

また、サインインしているユーザーは、 **Programcontrol**を作成することを許可するディレクトリロールにある必要があります。 

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
要求本文で、 [Programcontrol](../resources/programcontrol.md)オブジェクトの JSON 表記を指定します。

次の表に、プログラムコントロールの作成時に必要なプロパティを示します。

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
| `programId`              |`String`                | このコントロールが一部になるプログラムの programId。                             |
| `controlId`              |`String`                | コントロールの controlId (特にアクセスレビューの識別子)。                                                |
| `controlTypeId`          |`String`                | ProgramControlType には、プログラムコントロールの種類を指定します。たとえば、ゲストアクセスレビューにリンクしているコントロールがあります。 |

## <a name="response"></a>応答
成功した場合、このメソッド`201, Created`は応答コードと、応答本文で[programcontrol](../resources/programcontrol.md)オブジェクトを返します。


## <a name="example"></a>例
##### <a name="request"></a>要求
要求本文で、 [Programcontrol](../resources/programcontrol.md)オブジェクトの JSON 表記を指定します。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
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
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-programcontrol-from-programcontrols-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-programcontrol-from-programcontrols-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-programcontrol-from-programcontrols-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-programcontrol-from-programcontrols-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


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
|[ProgramControlTypes のリスト](../api/programcontroltype-list.md) | [Programcontroltype](../resources/programcontroltype.md)コレクション| プログラムコントロールの種類を一覧表示します。 |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
