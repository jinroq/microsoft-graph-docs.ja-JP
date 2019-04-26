---
title: trustframeworkpolicy
description: Azure AD B2C 信頼フレームワークポリシーは、カスタムポリシーと呼ばれます。 これは、テナントの trustframeworkpolicy オブジェクトで利用可能な操作を示します。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 3160ce5ec75c0b65def8aed44ad89032cd293dee
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345464"
---
# <a name="trustframeworkpolicy-resource-type"></a>trustframeworkpolicy リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。

[Azure Active Directory B2C](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview)の[信頼フレームワーク](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-reference-trustframeworks-defined-ief-custom)ポリシー ([カスタムポリシー](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)とも呼ばれます) を表します。 信頼フレームワークポリシーにより、ユーザー手順を完全に制御できるようになります。 次の場合に使用します。

* サインアップおよびサインインの完全なエクスペリエンスをカスタマイズします。
* 任意の SAML、Open id Connect、または OAuth2 id プロバイダーとのフェデレーションを行います。
* REST エンドポイントを呼び出すことで、他のシステムまたはユーザーのデータストアと統合します。
* クレームを変換し、証明書利用者アプリケーションに発行されたトークンをカスタマイズします。

詳細については、「 [Azure Active Directory B2C のカスタムポリシー](https://docs.microsoft.com/en-us/azure/active-directory-b2c/active-directory-b2c-overview-custom)」を参照してください。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[trustframeworkpolicy の作成](../api/trustframework-post-trustframeworkpolicy.md)|trustframeworkpolicy|新しい trustframeworkpolicy を作成します。|
|[trustframeworkpolicy の取得](../api/trustframeworkpolicy-get.md) |trustframeworkpolicy|既存の trustframeworkpolicy のプロパティを読み取ります。|
|[trustframeworkpolicies を一覧表示する](../api/trustframework-list-trustframeworkpolicies.md)|trustframeworkpolicy コレクション|テナントで構成されているすべての trustframeworkpolicies を一覧表示します。|
|[trustframeworkpolicy を更新または作成する](../api/trustframework-put-trustframeworkpolicy.md)|なし|既存の trustframeworkpolicy を更新します。|
|[trustframeworkpolicy の削除](../api/trustframeworkpolicy-delete.md)|なし|既存の trustframeworkpolicy を削除します。|

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

- [trustframeworkpolicy](https://docs.microsoft.com/en-us/azure/active-directory-b2c/trustframeworkpolicy)スキーマ要素に関する情報を示します。  
- [trustframeworkpolicy .xsd](https://github.com/Azure-Samples/active-directory-b2c-custom-policy-starterpack/blob/master/TrustFrameworkPolicy_0.3.0.0.xsd)
