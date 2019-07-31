---
title: TrustFrameworkPolicy の作成
description: この操作により、Azure AD B2C テナントに新しい trustFrameworkPolicy オブジェクトが作成されます。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac3e1546e72e91988ef5339ad201fab7f3f2224d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990569"
---
# <a name="create-trustframeworkpolicy"></a>TrustFrameworkPolicy の作成

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。

新しい[Trustframeworkpolicy](../resources/trustframeworkpolicy.md)オブジェクトを作成します。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。

|アクセス許可の種類      | アクセス許可 (特権の小さいものから大きいものへ)              |
|:--------------------|:---------------------------------------------------------|
|委任 (職場または学校のアカウント)|Policy.ReadWrite.TrustFramework|
|委任 (個人用 Microsoft アカウント)| サポートされていません。|
|アプリケーション|サポートされていません。|

職場または学校のアカウントは、テナントのグローバル管理者のものである必要があります。

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->
```http
POST /trustFramework/policies
```

## <a name="request-headers"></a>要求ヘッダー

|名前|説明|
|:---------------|:----------|
|Authorization|ベアラー {トークン}。必須。|
|Content-Type|アプリケーション/xml。 必須です。|

## <a name="request-body"></a>要求本文

要求本文で、 [Trustframeworkpolicy](../resources/trustframeworkpolicy.md)オブジェクトの XML 表現を指定します。 コンテンツ タイプは `application/xml` でなければなりません。

## <a name="response"></a>応答

成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[trustframeworkpolicy](../resources/trustframeworkpolicy.md)オブジェクトを返します。 失敗した場合、`4xx` エラーが詳細情報とともに返されます。

## <a name="example"></a>例

次の例では、 **Trustframeworkpolicy**を作成します。

##### <a name="request"></a>要求

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "name": "create_trustframeworkpolicy_from_trustframeworkpolicy"
}-->
```http
POST https://graph.microsoft.com/beta/trustFramework/policies
Content-Type: application/xml

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```

##### <a name="response"></a>応答

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
} -->
```http
HTTP/1.1 201 Created
Content-Type: application/xml
Location: /trustFramework/policies/B2C_1A_SocialAndLocalAccounts_Base/

<TrustFrameworkPolicy xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns="http://schemas.microsoft.com/online/cpim/schemas/2013/06" PolicySchemaVersion="0.3.0.0" TenantId="tenantName.onmicrosoft.com" PolicyId="B2C_1A_SocialAndLocalAccounts_Base" PublicPolicyUri="http://tenantName.onmicrosoft.com/B2C_1A_Test">
    <!---PolicyContent-->
</TrustFrameworkPolicy>
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create trustFrameworkPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
