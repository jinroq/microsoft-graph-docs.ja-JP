---
title: ポリシー リソースの種類
description: Azure AD ポリシーを表します。 ポリシーは、アプリケーション、サービス ・ プリンシパル、グループ、または組織に割り当てられている全体に適用することができますカスタム ルールです。 現在だけがポリシーの 1 つのタイプがあります。
localization_priority: Normal
ms.openlocfilehash: bd946da13fc36925e284ad2af29585b37d0a9a3a
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576200"
---
# <a name="policy-resource-type"></a>ポリシー リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Azure AD ポリシーを表します。 ポリシーは、アプリケーション、サービス ・ プリンシパル、グループ、または組織に割り当てられている全体に適用することができますカスタム ルールです。 現在だけがポリシーの 1 つのタイプがあります。

- トークンの有効期間ポリシー]-[アプリケーションとサービス ・ プリンシパルに発行されたトークンの有効期間を指定します。

このポリシーはさらに以下で詳しく説明します。

## <a name="methods"></a>メソッド
| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
| [ポリシーを取得します。](../api/policy-get.md) |ポリシー|ユーザー オブジェクトのプロパティと関係を読み取ります。|
|[ポリシーを作成します。](../api/policy-post.md)|ポリシー|新しいポリシー オブジェクトを作成します。|
|[ポリシーを更新します。](../api/policy-update.md)|なし|ポリシー オブジェクトを更新します。|
|[ポリシーを削除します。](../api/policy-delete.md)|なし|ポリシー オブジェクトを削除します。|
|[ポリシーを割り当てる](../api/policy-assign.md)|なし|サービス主体のアプリケーションにポリシーを割り当てます。|
|[リスト ポリシー](../api/policy-list.md)|ポリシー コレクション|組織内のすべてのポリシー オブジェクトを取得します。|
|[リストが割り当てられているポリシー](../api/policy-list-assigned.md)|ポリシー コレクション|アプリケーションまたはサービス ・ プリンシパルに割り当てられているすべてのポリシー オブジェクトを取得します。|

### <a name="common-properties"></a>共通プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|definition|String コレクション|特定のポリシーの文字列バージョンです。 以下を参照してください。 必須。|
|displayName|String|ポリシーに独自の名前です。 必須です。|
|IsOrganizationDefault|Boolean|場合に true の場合、このポリシーをアクティブに設定します。 同一のポリシーの種類の多くのポリシーが存在することができますが、組織の既定値として、1 つだけをアクティブにすることができます。 オプション、既定値では、false を指定します。|
|type|String|ポリシーの種類を指定します。 現在"TokenLifetimePolicy"をする必要があります。 必須です。|

#### <a name="common-relationships"></a>共通関係
|リレーションシップ|型|説明|
|:-------------|:-----------|:-----------|
|appliesTo|[directoryObject](../resources/directoryobject.md) コレクション|アプリケーション、サービス ・ プリンシパル、グループ、または組織ポリシーを適用します。|

## <a name="token-lifetime-policy"></a>トークンの有効期間のポリシー
さまざまな目的で発行されたトークンの有効期間を指定します。 このようなポリシーは、アプリケーションとサービス ・ プリンシパルに[割り当てられている](../api/policy-assign.md)ができます。 4 種類のトークンの有効期間を構成することがあります。 ブラウザー経由の認証時に ID とセッション トークンのペアを取得し、クライアントからの認証中に/更新のアクセス トークンのペアが得られます。

- **アクセス トークン**には、id、およびアプリケーションと同様に保護されたリソースにアクセスするクライアントによって使用されるユーザー アカウントに関連付けられている権限についての情報が含まれています。
- **トークンの更新**は、アクセス トークンと Azure の AD によって保護されたリソースにアクセスするクライアントに対してユーザーを認証するときです。 失効していないまたは (下) MaxInactiveTime より多くの未使用のまま、中には、現在のアクセス トークンの有効期限が切れたときに、新しい/更新のアクセス トークンのペアを取得するのには使用できます。
- **ID のトークン**は、アクセス トークンと同様に動作しますが、ブラウザー経由で取得しました。
- **セッション トークン**をブラウザーから取得したのですが、更新のトークンと同様に動作します。

## <a name="properties"></a>プロパティ
以下のプロパティは、トークンの有効期間ポリシーを表す JSON オブジェクトを形成します。 この JSON オブジェクトする必要があります**エスケープの見積を文字列に変換**」の定義」の一般的なポリシーのプロパティに挿入します。 例を次に示します。

>注: これらのプロパティのすべての時間は、"dd.hh:mm:ss"の形式で指定します。

>注:「日」で表されるプロパティの最大値は、コンセンサスを表します日数の 1 秒です。 として 1 日の最大値を指定するたとえば、"23: 59:59"です。

| プロパティ     | 型   |説明| 最小値 | 最大値 | 既定値|
|:---------------|:--------|:----------|:--------|:--------|:----|
|AccessTokenLifetime|String|どのくらいの期間**アクセスと ID のトークンの両方**有効と見なされますを制御します。|10 分|1 日|1 時間|
|MaxInactiveTime|String|古い更新トークンは、クライアントが使用できなくなりますリソースにアクセスする新しいアクセス/更新トークンのペアを取得する前に制御します。|10 分|90 日間|14 日間|
|MaxAgeSingleFactor|String|コントロールがどのくらいの時間を取得する新しいアクセスの更新トークンのペア、認証された後正常に 1 つの要因だけで更新トークンを使用するユーザーが続行できます。 一元的は、多元的な認証よりも安全性が低いと見なされる、ため、MultiFactorRefreshTokenMaxAge よりも等しいか小さい値にこのポリシーを設定することをお勧めします。|10 分|無効にするまで|365 日または失効するまで|
|MaxAgeMultiFactor|String|コントロールがどのくらいの時間を取得する新しいアクセスの更新トークンのペア、認証された後正常に複数の要素を持つ更新トークンを使用するユーザーが続行できます。|10 分|無効にするまで|365 日または失効するまで|
|MaxAgeSessionSingleFactor|String|コントロールがどのくらいの時間、ユーザーは、セッション トークンを使用して、最後に、正常に認証された 1 つの要因だけで新しい ID とセッションのトークンを取得するには続行できます。 一元的は、多元的な認証よりも安全性が低いと見なされる、ためには、このポリシーが、MultiFactorSessionTokenMaxAge よりも等しいまたはより低い値に設定されているをお勧め|10 分|無効にするまで|365 または無効にするまで|
|MaxAgeSessionMultiFactor|String|コントロールがどのくらいの時間、ユーザーは、セッション トークンを使用して複数の要因で正常に認証されて、最後に新しい ID とセッションのトークンを取得するのには続行できます。|10 分|無効にするまで|365 または無効にするまで|
|バージョン|整数|1 の値を設定します。 必須です。|なし|なし|なし|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.policy"
}-->

```json
{
  "definition":["{\"TokenLifetimePolicy\":{\"Version\":1,\"AccessTokenLifetime\":\"8:00:00\",\"MaxInactiveTime\":\"20:00:00\",}}"],
  "displayName":"Test Policy",
  "isOrganizationDefault":false,
  "type":"TokenLifetimePolicy",
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/policy.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
