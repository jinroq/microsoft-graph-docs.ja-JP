---
title: Certificateベース Authconfiguration リソースの種類
description: 証明機関のコレクションを表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 76178d8d70225a8cf861f5ff5e1cdaf7f0f69f60
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667663"
---
# <a name="certificatebasedauthconfiguration-resource-type"></a>Certificateベース Authconfiguration リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

証明書ベースの認証を使用すると、Exchange Online アカウントを次のように接続する際に、Windows、Android、または iOS デバイス上のクライアント証明書を使用して Azure Active Directory による認証を行うことができます。

- Outlook や Word などの Microsoft モバイルアプリケーション
- Exchange ActiveSync (EAS) クライアント

この機能を構成すると、ユーザー名とパスワードの組み合わせを、モバイルデバイス上の特定のメールおよび Microsoft Office アプリケーションに入力する必要がなくなります。

証明書ベースの認証構成は、証明機関のコレクションによって提供されます。 証明機関は、信頼できる証明書チェーンを確立するために使用されます。これにより、クライアント証明書を使用して Azure Active Directory によってクライアントを認証できます。

[Azure Active Directory での証明書ベースの認証の](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-certificate-based-authentication-get-started)詳細について説明します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [Certificateベース Authconfiguration の一覧表示](../api/certificatebasedauthconfiguration-list.md) | [Certificateベース Authconfiguration](certificatebasedauthconfiguration.md) | **Certificateベース Authconfiguration**コレクションのプロパティを一覧表示します。 |
| [Certificateベース Authconfiguration の取得](../api/certificatebasedauthconfiguration-get.md) | [Certificateベース Authconfiguration](certificatebasedauthconfiguration.md) | **Certificateベース Authconfiguration**オブジェクトのプロパティを読み取ります。 |
| [Certificateベース Authconfiguration の作成](../api/certificatebasedauthconfiguration-post-certificatebasedauthconfiguration.md) | [Certificateベース Authconfiguration](certificatebasedauthconfiguration.md) | 新しい**Certificateベース Authconfiguration**オブジェクトを作成します。 |
| [Certificateベース Authconfiguration の削除](../api/certificatebasedauthconfiguration-delete.md) | None | **Certificateベース Authconfiguration**オブジェクトを削除します。 |

>[!NOTE]
>Cerの更新はサポートされていません。 Cerな設定を変更するには、まず、を削除してから、新しい cerの設定を作成します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|certificateAuthorities|[Certificateauthority](certificateauthority.md)コレクション|信頼された証明書チェーンを作成する証明機関のコレクション。|
|id|String|証明書ベースの認証構成の一意の識別子。 読み取り専用です。|

## <a name="relationships"></a>関係

なし

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateBasedAuthConfiguration",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "certificateAuthorities": {"@odata.type": "collection(microsoft.graph.certificateAuthority)"},
  "id": "String (identifier)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateBasedAuthConfiguration resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
