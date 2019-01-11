---
title: デバッギングを作成します。
description: Azure AD のレビュー機能にアクセス、デバッギング オブジェクトを新規作成します。  アクセス確認をプログラムにリンクします。
localization_priority: Normal
ms.openlocfilehash: 4dfbb76244a41867b8a57faa42f63dc728f59136
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851535"
---
# <a name="create-programcontrol"></a>デバッギングを作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、新しい[デバッギング](../resources/programcontrol.md)オブジェクトを作成します。  アクセス確認をプログラムにリンクします。

この要求を行う前に呼び出し元には以前

 - [プログラムを作成](program-create.md)または[プログラムを取得する](program-list.md)の値を設定する`programId`、要求に含める
 - [アクセス確認を作成](accessreview-create.md)または[、アクセス確認を取得する](accessreview-get.md)の値を設定する`controlId`、要求に含めると
 - [コントロールの種類のプログラムの一覧を取得](programcontroltype-list.md)の値を設定する`controlTypeId`要求に含める。


## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | `ProgramControl.ReadWrite.All`.  サインインしているユーザーは、ディレクトリの役割を可能にして、デバッギングを作成する必要があります。 |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 種類        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー\{トークン\}。 必須。 |

## <a name="request-body"></a>要求本文
要求の本文には、[デバッギング](../resources/programcontrol.md)オブジェクトの JSON の形式を指定します。

プログラムのコントロールを作成するときに必要なプロパティを次の表に示します。

| プロパティ     | 種類        | 説明 |
|:-------------|:------------|:------------|
| `programId`              |`String`                | プログラムの programId コントロールしようの一部になります。                             |
| `controlId`              |`String`                | コントロールの処理、特にアクセスの id を確認します。                                                |
| `controlTypeId`          |`String`                | ProgramControlType は、プログラムの制御の種類を識別 - たとえば、ゲスト アクセスへのリンク コントロールを確認します。 |

## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、`201, Created`応答コードおよび応答の本文の[デバッギング](../resources/programcontrol.md)オブジェクトです。


## <a name="example"></a>例
##### <a name="request"></a>要求
要求の本文には、[デバッギング](../resources/programcontrol.md)オブジェクトの JSON の形式を指定します。

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
|[リスト programControlTypes](../api/programcontroltype-list.md) | [programControlType](../resources/programcontroltype.md)コレクション| プログラムのコントロールの種類を一覧表示します。 |


<!-- {
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
