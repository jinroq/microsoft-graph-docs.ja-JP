---
title: ディレクトリの設定を作成します。
description: DirectorySettingTemplates で利用可能なテンプレートに基づいて、新しい設定を作成するのにには、この API を使用します。 テナント レベルまたはオブジェクト レベルでこれらの設定ができます (現在のグループに対してのみ)。 テンプレートで定義されているすべての設定の作成の要求に settingValues を入力してください。 グループに固有の設定のみの設定を制御するグループのメンバーは、ゲスト ユーザーを招待できるかどうかを設定できます。 ゲスト ユーザーをグループに追加することが一般的に使用できるとは、この動作が適用されます。
ms.openlocfilehash: 40e90f66c43032deea8ee866b13508fd73c0f17f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068905"
---
# <a name="create-a-directory-setting"></a>ディレクトリの設定を作成します。

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

DirectorySettingTemplates で利用可能なテンプレートに基づいて、新しい設定を作成するのにには、この API を使用します。 テナント レベルまたはオブジェクト レベルでこれらの設定ができます (現在のグループに対してのみ)。 テンプレートで定義されているすべての設定の作成の要求に settingValues を入力してください。 グループに固有の設定のみの設定を制御するグループのメンバーは、ゲスト ユーザーを招待できるかどうかを設定できます。 ゲスト ユーザーをグループに追加することが一般的に使用できるとは、この動作が適用されます。

> **注**: この API の/beta バージョンは、のみのグループに適用されます。 この API の/v1.0 バージョン*を作成する groupSettings*の名前は。

テンプレートとベータ版でサポートしているプロパティのリストは、 [directorySettingTemplate クエリ](https://developer.microsoft.com/graph/graph-explorer?request=directorySettingTemplates&version=beta)を使用します。 ( [GroupSettingTemplates](https://developer.microsoft.com/graph/graph-explorer?request=groupSettingTemplates&version=v1.0)を呼び出す v1.0 のエンドポイントに対して)。


## <a name="permissions"></a>アクセス許可
この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) | Directory.ReadWrite.All、Directory.AccessAsUser.All    |
|委任 (個人用 Microsoft アカウント) | サポートされていません。    |
|アプリケーション | Directory.ReadWrite.All |

## <a name="http-request"></a>HTTP 要求
<!-- { "blockType": "ignored" } -->
```http
POST /settings
POST /groups/{id}/settings
```
## <a name="request-headers"></a>要求ヘッダー
| 名前       | 説明|
|:---------------|:----------|
| Authorization  | ベアラー {トークン}。必須。|

## <a name="request-body"></a>要求本文
要求の本文には、 [directorySetting](../resources/directorysetting.md)オブジェクトの JSON 表現を指定します。  ただし、設定の表示名が設定に基づいて参照設定テンプレート名を。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[directorySetting](../resources/directorysetting.md)のオブジェクトです。

## <a name="example"></a>例
##### <a name="request"></a>要求
以下は、要求の例です。
<!-- {
  "blockType": "request",
  "name": "create_directorysetting_from_settings"
}-->
```http
POST https://graph.microsoft.com/beta/settings
Content-type: application/json
Content-length: 222

{
  "templateId": "templateId-value",
  "values": [
    {
      "name": "name-value",
      "value": "value-value"
    }
  ]
}
```
要求の本文には、 [directorySetting](../resources/directorysetting.md)オブジェクトの JSON 表現を指定します。
##### <a name="response"></a>応答
以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directorySetting"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 244

{
    "@odata.context": "https://graph.microsoft.com/stagingbeta/$metadata#settings/$entity",
    "id": "id-value",
    "displayName": "displayName-value",
    "templateId": "templateId-value",
    "values": [
      {
        "name": "name-value",
        "value": "value-value"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directorySetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->