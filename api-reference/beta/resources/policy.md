---
title: ポリシーリソースの種類
description: Azure AD ポリシーを表します。 ポリシーは、割り当てられているアプリケーション、サービスプリンシパル、グループ、または組織全体に適用できるカスタムルールです。 現時点では、使用可能なポリシーの種類は1つだけです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4a97caf82a53900ac4ba1e81cebddda114336597
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965812"
---
# <a name="policy-resource-type"></a>ポリシーリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD ポリシーを表します。 ポリシーは、割り当てられているアプリケーション、サービスプリンシパル、グループ、または組織全体に適用できるカスタムルールです。 現時点では、使用可能なポリシーの種類は1つだけです。

- トークン有効期間ポリシー-アプリケーションおよびサービスプリンシパルに対して発行されるトークンの有効期間を指定します。

このポリシーについては、後で詳しく説明します。

## <a name="methods"></a>メソッド
| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
| [ポリシーを取得する](../api/policy-get.md) |ポリシー|ユーザー オブジェクトのプロパティと関係を読み取ります。|
|[ポリシーを作成する](../api/policy-post.md)|ポリシー|新しいポリシーオブジェクトを作成します。|
|[ポリシーを更新する](../api/policy-update.md)|None|ポリシーオブジェクトを更新します。|
|[ポリシーを削除する](../api/policy-delete.md)|None|ポリシーオブジェクトを削除します。|
|[ポリシーの割り当て](../api/policy-assign.md)|None|アプリケーションのサービスプリンシパルにポリシーを割り当てます。|
|[ポリシーを一覧表示する](../api/policy-list.md)|ポリシーのコレクション|組織内のすべてのポリシーオブジェクトを取得します。|
|[割り当てられているポリシーを一覧表示する](../api/policy-list-assigned.md)|ポリシーのコレクション|アプリケーションまたはサービスプリンシパルに割り当てられているすべてのポリシーオブジェクトを取得します。|

##  <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|definition|文字列コレクション|特定のポリシーの文字列バージョン。 以下を参照してください。 必須。|
|displayName|文字列|ポリシーのカスタム名。 必須です。|
|Is組織既定|Boolean|True に設定されている場合は、このポリシーを有効にします。 同じポリシーの種類に対して複数のポリシーを設定できますが、組織の既定値としてライセンス認証を行うことができるのは1つだけです。 省略可能。既定値は false です。|
|type|String|ポリシーの種類を指定します。 現在、"TokenLifetimePolicy" である必要があります。 必須です。|
|alternativeIdentifer|String| |
|keyCredentials| [keyCredential](keycredential.md) コレクション| |

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.policy",
  "keyProperty": "id",
  "baseType":"microsoft.graph.directoryObject",  
  "openType": true
}-->
```json
{
  "alternativeIdentifer": "String",
  "definition": ["String"],
  "displayName": "String",
  "isOrganizationDefault": "Boolean",
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "type": "String"
}
```

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:-------------|:-----------|:-----------|
|appliesTo|[directoryObject](../resources/directoryobject.md) collection|ポリシーが適用されるアプリケーション、サービスプリンシパル、グループ、または組織。|

### <a name="token-lifetime-policy"></a>トークンの有効期間ポリシー
さまざまな目的に対して発行されるトークンの有効期間を指定します。 この種のポリシーは、アプリケーションおよびサービスプリンシパルに[割り当てる](../api/policy-assign.md)ことができます。 有効期間を構成できるトークンには4つの種類があります。 アクセス/更新トークンのペアはクライアントを介して認証時に取得されますが、ID/セッショントークンのペアはブラウザーを介して認証時に取得されます。

- **アクセストークン**には、アプリケーションなどの保護されたリソースにアクセスするためにクライアントによって使用されるユーザーアカウントに関連付けられている id と権限に関する情報が含まれています。
- ユーザーが保護されたリソースにアクセスするためにクライアントを使用して Azure AD に対して認証を行う場合、**更新トークン**はアクセストークンと共に取得されます。 MaxInactiveTime (以下を参照) よりも多くの場合、取り消されていないか、または使用されていないため、現在のアクセストークンの有効期限が切れたときに新しいアクセス/更新トークンのペアを取得するために使用できます。
- **ID トークン**はアクセストークンと同様に動作しますが、ブラウザーから取得されます。
- **セッショントークン**は、更新トークンと同じように動作しますが、ブラウザーで取得されます。

#### <a name="properties-of-a-token-lifetime-policy"></a>トークンの有効期間ポリシーのプロパティ
以下のプロパティは、トークンの有効期間ポリシーを表す JSON オブジェクトを形成します。 この JSON オブジェクトは、"definition" 共通ポリシープロパティに挿入されるように**引用符がエスケープされた文字列に変換**する必要があります。 JSON 形式での例を次に示します。

<!-- {
  "blockType": "ignored"
}-->
``` json
"definition": [
    "{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"
  ]
```

>注: これらのプロパティのすべての期間は、"dd. hh: mm: ss" という形式で指定されています。

>注: "days" で示されるプロパティの最大値は、指定された日数の1秒短くなります。 たとえば、1日の最大値が "23:59:59" として指定されているとします。

| プロパティ     | 型   |説明| 最小値 | 最大値 | 既定値|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|String|**アクセストークンと ID トークンの両方**が有効と見なされる期間を制御します。|10 分|1 日|1 hour|
|MaxInactiveTime|String|古い更新トークンが、リソースにアクセスするために新しいアクセス/更新トークンのペアを取得するために使用できなくなる前に、更新トークンがどのように使用されるかを制御します。|10 分|90 日間|14 日|
|MaxAgeSingleFactor|String|ユーザーが更新トークンを使用して、最後に認証に成功した後に新しいアクセス/更新トークンのペアを取得するために、1つの要素のみで継続できる期間を制御します。 単一要素は多要素認証より安全ではないと考えられるため、このポリシーは、MultiFactorRefreshTokenMaxAge と同等またはそれより小さい値に設定することをお勧めします。|10 分|失効まで|365日または失効まで|
|MaxAgeMultiFactor|String|ユーザーが定期的に更新トークンを使用して、複数の要素で最後に認証された後に新しいアクセス/更新トークンのペアを取得する時間を制御します。|10 分|失効まで|365日または失効まで|
|MaxAgeSessionSingleFactor|String|ユーザーがセッショントークンを引き続き使用して、1つの要素のみで前回認証に成功した後に新しい ID/セッショントークンを取得できる期間を制御します。 単一要素は多要素認証より安全ではないと考えられるため、このポリシーは、MultiFactorSessionTokenMaxAge と同等またはそれより小さい値に設定することをお勧めします。|10 分|失効まで|365または無効|
|MaxAgeSessionMultiFactor|String|ユーザーが引き続きセッショントークンを使用して、複数の要素で最後に認証された後に新しい ID/セッショントークンを取得できる期間を制御します。|10 分|失効まで|365または無効|
|バージョン|整数|値を1に設定します。 必須です。|なし|なし|None|


