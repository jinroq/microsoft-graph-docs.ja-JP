---
title: SecureScoreControlProfiles を更新します。
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: afbfcd1889c55dd53241ff8d796bb3ab492b2acf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066470"
---
# <a name="update-securescorecontrolprofiles"></a>SecureScoreControlProfiles を更新します。

 > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

**担当者**や**tenantNote**などのさまざまなプロパティを変更するのには統合されたソリューション内で編集可能な**secureScoreControlProfiles**プロパティを更新します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント) |   SecurityEvents.ReadWrite.All。  |
|委任 (個人用 Microsoft アカウント) |  サポートされていません。  |
|アプリケーション | SecurityEvents.ReadWrite.All。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
PATCH /security/secureScoreControlProfiles/{id}
```

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 説明|
|:-----------|:-----------|
| Authorization  | Bearer {code}。必須。|
|Prefer | 返す = 表現します。 |

## <a name="request-body"></a>要求本文

要求の本文には、更新される関連フィールドの値の JSON の形式を指定します。 SecureScoreControlProfile に更新可能なフィールドを次の表に一覧します。 要求の本文に含まれていない既存のプロパティの値は変更されません。 最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。

| プロパティ   | 型 |説明|
|:---------------|:--------|:----------|
|担当者|String|アナリストのコントロールの名前は、選別、導入、または修復用に割り当てられます。|
|tenantNote|String|(顧客管理) のコントロールのアナリストのコメントです。|
|controlStateUpdates| String|アナリストは、コントロールの設定を優先します。 可能な値は、`ignore`、`thirdParty`、`reviewed` です。|


## <a name="response"></a>応答

成功した場合、このメソッドは `204 No Content` 応答コードを返します。

省略可能な要求ヘッダーが使用され、メソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[secureScoreControlProfiles](../resources/securescorecontrolprofiles.md)オブジェクトです。

## <a name="example"></a>例

### <a name="request"></a>要求

要求の例を次に示します。
<!-- {
  "blockType": "request",
  "name": "securescorecontrolprofiles_update"
}-->

```http
PATCH https://graph.microsoft.com/beta/security/secureScoreControlProfiles/AdminMFA
Content-type: application/json

{
  "assignedTo": "assignedTo-value",
  "controlStateUpdates": "controlStateUpdates-value",
  "tenantNote": "tenantNote-value"
}
```

### <a name="response"></a>応答

次は、正常な応答の例です。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.secureScoreControlProfiles"
} -->

```http
HTTP/1.1 204 No Content
```




<!-- {
  "type": "#page.annotation",
  "description": "Update secureScoreControlProfiles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
