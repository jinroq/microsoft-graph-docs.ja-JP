---
title: 更新プログラム
description: Azure AD のレビュー機能にアクセス、既存のプログラム オブジェクトを更新します。
localization_priority: Normal
ms.openlocfilehash: a9abe10a2a672984d14f1da821b7ae6244cbdf39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840335"
---
# <a name="update-program"></a>更新プログラム

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

機能では、Azure AD[アクセスの確認](../resources/accessreviews-root.md)、既存の[プログラム](../resources/program.md)オブジェクトを更新します。
## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)     | `ProgramControl.ReadWrite.All`.  サインインしているユーザーは、プログラムを更新することを許可するディレクトリの役割でもあります。 |
|委任 (個人用 Microsoft アカウント) | サポートされていません。 |
|アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a>要求ヘッダー
| 名前         | 種類        | 説明 |
|:-------------|:------------|:------------|
| Authorization | string | ベアラー\{トークン\}。 必須。 |

## <a name="request-body"></a>要求本文
要求の本文には、[プログラム](../resources/program.md)オブジェクトの JSON 表現を指定します。

プログラムを更新するときに指定できるプロパティを次の表に示します。

| プロパティ     | 種類        | 説明 |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  プログラムの名前です。                   |
| `description`               |`String`                              |  プログラムの説明です。           |


## <a name="response"></a>応答
かどうかは成功すると、このメソッドが返されます、 `204, Accepted` 、応答の本体で応答コードと[プログラム](../resources/program.md)のオブジェクトです。

## <a name="example"></a>例
##### <a name="request"></a>要求
要求の本文には、[プログラム](../resources/program.md)オブジェクトのパラメーターを変更するのに JSON 形式を指定します。

<!-- {
  "blockType": "request",
  "name": "update_program"
}-->
```http
PATCH https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
Content-type: application/json

{
    "displayName": "testprogram3 new name"
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
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3 new name",
    "description": "test description"
}
```

## <a name="see-also"></a>関連項目

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[プログラムのリスト programControls](program-listcontrols.md) |     [デバッギング](../resources/programcontrol.md)コレクション|    プログラムのコントロールのコレクションを取得します。|
|[デバッギングを作成します。](programcontrol-create.md) |        [デバッギング](../resources/programcontrol.md)    |   デバッギングをプログラムに追加します。|

<!-- {
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
