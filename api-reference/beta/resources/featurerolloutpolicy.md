---
title: featureRolloutPolicy リソースの種類
description: ディレクトリオブジェクトに関連付けられている機能ロールアウトポリシーを表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 50d54ae046ef5a0283f5eb2e474fd0faab781687
ms.sourcegitcommit: bbed891d16995b4a8ce866169dddb96abdc28776
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/02/2019
ms.locfileid: "36062164"
---
# <a name="featurerolloutpolicy-resource-type"></a>featureRolloutPolicy リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ディレクトリオブジェクトに関連付けられている機能ロールアウトポリシーを表します。 機能ロールアウトポリシーを作成すると、テナント管理者は、組織全体に対して機能を有効にする前に、特定のグループを使用して Azure AD の機能を試験的に実行できます。 これにより、影響が最小限に抑えられ、管理者が認証関連機能を徐々にテストおよびロールアウトできるようになります。

機能のロールアウトには、次の制限があります。

- 各機能では、最大10個のグループがサポートされています。
- **AppliesTo**フィールドは、グループのみをサポートします。
- 動的グループとネストされたグループはサポートされていません。

このロールアウトポリシーを使用して、現在 suported に展開されている各機能の前提条件は次のとおりです。

### <a name="passthrough-authentication"></a>パススルー認証

* [認証](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-pta)エージェントを実行する Windows Server 2012 R2 以降を実行しているサーバーを特定します。サーバーがドメインに参加しており、Active Directory を使用して選択したユーザーを認証できること、および送信ポート/Url で Azure AD と通信できることを確認してください。
* サーバーに Microsoft Azure AD Connect 認証エージェントを[ダウンロード](https://aka.ms/getauthagent)& インストールします。
* 高可用性を有効にするには、[ここ](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-pta-quick-start#step-4-ensure-high-availability)に記載されているように、他のサーバーに追加の認証エージェントをインストールします。
* [スマートロックアウト](https://docs.microsoft.com/en-us/azure/active-directory/authentication/howto-password-smart-lockout)設定が適切に構成されていることを確認します。 これは、ユーザーのオンプレミスの Active Directory アカウントが不正な俳優によってロックアウトされないようにするためです。

### <a name="seamlesssso"></a>SeamlessSso

* [次](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/tshoot-connect-sso#manual-reset-of-the-feature)の手順に従って、AD フォレストの[SeamlessSso](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/how-to-connect-sso)を有効にします。

### <a name="passwordhashsync"></a>PasswordHashSync

* Azure AD Connect の [オプション機能] ページで [PasswordHashSync](https://docs.microsoft.com/en-us/azure/active-directory/hybrid/whatis-phs) を有効にします。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
| [リスト featureRolloutPolicies](../api/directory-list-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | FeatureRolloutPolicy オブジェクトのリストを取得します。 |
| [FeatureRolloutPolicy を取得する](../api/featurerolloutpolicy-get.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Featurerolloutpolicy オブジェクトのプロパティとリレーションシップを取得します。 ||
| [FeatureRolloutPolicy を作成する](../api/directory-post-featurerolloutpolicies.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | 新しい featureRolloutPolicy オブジェクトを作成します。
| [FeatureRolloutPolicy の更新](../api/featurerolloutpolicy-update.md) | [featureRolloutPolicy](featurerolloutpolicy.md) | Featurerolloutpolicy オブジェクトのプロパティを更新します。 |
| [FeatureRolloutPolicy の削除](../api/featurerolloutpolicy-delete.md) | None | FeatureRolloutPolicy オブジェクトを削除します。 |
| [AppliesTo を割り当てる](../api/featurerolloutpolicy-post-appliesto.md) | [directoryObject](directoryobject.md) | 機能のロールアウトに directoryObject を割り当てます。 |
| [AppliesTo の削除](../api/featurerolloutpolicy-delete-appliesto.md) | None | 機能ロールアウトから directoryObject を削除します。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|description|String|この機能ロールアウトポリシーの説明。|
|displayName|String|この機能ロールアウトポリシーの表示名。|
|特徴|stagedFeatureName| 使用可能な値は、`passthroughAuthentication`、`seamlessSso`、`passwordHashSync`、`unknownFutureValue` です。|
|id|String| 読み取り専用です。|
|isAppliedToOrganization|Boolean|この機能ロールアウトポリシーを組織全体に適用する必要があるかどうかを示します。|
|isEnabled|Boolean|機能ロールアウトが有効になっているかどうかを示します。|

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型        | 説明 |
|:-------------|:------------|:------------|
|appliesTo|[directoryObject](directoryobject.md) collection| Null 許容型。 機能が有効になっている directoryObjects のリストを指定します。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.featureRolloutPolicy",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "feature": "string",
  "id": "String (identifier)",
  "isAppliedToOrganization": false,
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "featureRolloutPolicy resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
