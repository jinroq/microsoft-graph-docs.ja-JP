---
title: trustFrameworkPolicy
description: Azure AD B2C 信頼フレームワークポリシーは、カスタムポリシーと呼ばれます。 これは、テナントの trustFrameworkPolicy オブジェクトで利用可能な操作を示します。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: f573b331b587db50019e71468ec98d0e746e3963
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964187"
---
# <a name="trustframeworkpolicy-resource-type"></a>trustFrameworkPolicy リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。

[Azure Active DIRECTORY B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview)の[信頼フレームワーク](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom)ポリシー ([カスタムポリシー](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)とも呼ばれます) を表します。 信頼フレームワークポリシーにより、ユーザー手順を完全に制御できるようになります。 次の場合に使用します。

* サインアップおよびサインインの完全なエクスペリエンスをカスタマイズします。
* 任意の SAML、Open ID Connect、または OAuth2 id プロバイダーとのフェデレーションを行います。
* REST エンドポイントを呼び出すことで、他のシステムまたはユーザーのデータストアと統合します。
* クレームを変換し、証明書利用者アプリケーションに発行されたトークンをカスタマイズします。

詳細については、「 [Azure Active DIRECTORY B2C のカスタムポリシー](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)」を参照してください。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[TrustFrameworkPolicy の作成](../api/trustframework-post-trustframeworkpolicy.md)|trustFrameworkPolicy|新しい trustFrameworkPolicy を作成します。|
|[TrustFrameworkPolicy の取得](../api/trustframeworkpolicy-get.md) |trustFrameworkPolicy|既存の trustFrameworkPolicy のプロパティを読み取ります。|
|[TrustFrameworkPolicies を一覧表示する](../api/trustframework-list-trustframeworkpolicies.md)|trustFrameworkPolicy コレクション|テナントで構成されているすべての trustFrameworkPolicies を一覧表示します。|
|[TrustFrameworkPolicy を更新または作成する](../api/trustframework-put-trustframeworkpolicy.md)|None|既存の trustFrameworkPolicy を更新します。|
|[TrustFrameworkPolicy の削除](../api/trustframeworkpolicy-delete.md)|None|既存の trustFrameworkPolicy を削除します。|

## <a name="properties"></a>プロパティ

|プロパティ|型|説明|
|:---------------|:--------|:----------|
|id|String|ポリシーの ID。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType":"microsoft.graph.entity",
  "keyProperty":"id",
  "isMediaEntity":true,
  "@odata.type": "microsoft.graph.trustFrameworkPolicy"
}-->
```json
{
   "id": "B2C_1A_Test"
}
```

## <a name="see-also"></a>関連項目

- [Trustframeworkpolicy](https://docs.microsoft.com/en-us/azure/active-directory-b2c/trustframeworkpolicy)スキーマ要素に関する情報を示します。  
- [trustFrameworkPolicy .xsd](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)
