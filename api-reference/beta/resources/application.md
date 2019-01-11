---
title: アプリケーション リソースの種類
description: 'アプリケーションを表します。 Azure Active Directory (AD の Azure) への認証をアウトソースするすべてのアプリケーションは、ディレクトリに登録してください。 Azure AD を示す URL は、場所、アプリケーション、および詳細を識別する URI の認証の後に応答を送信する URL を含む、アプリケーションに関するアプリケーションの登録が含まれます。 詳細については、基本のアプリケーションを登録する Azure AD で参照してください。 directoryObject から継承します。 '
localization_priority: Priority
ms.openlocfilehash: b64de5670ccb9deebbabe32bb691d15b5a621f30
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805671"
---
# <a name="application-resource-type"></a>アプリケーション リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

アプリケーションを表します。 Azure Active Directory (AD の Azure) への認証をアウトソースするすべてのアプリケーションは、ディレクトリに登録してください。 Azure AD を示す URL は、場所、アプリケーション、および詳細を識別する URI の認証の後に応答を送信する URL を含む、アプリケーションに関するアプリケーションの登録が含まれます。 詳細については、[基本のアプリケーションを登録する Azure AD で](https://azure.microsoft.com/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad)参照してください。 [directoryObject](directoryobject.md) から継承します。 

> **注:** アプリケーション リソースの種類への変更は、現在開発中です。 詳細については、[既知の問題を Microsoft Graph を使用して](/graph/known-issues#application-and-serviceprincipal-api-changes)参照してください。

このリソースは以下をサポートしています。

- [デルタ](../api/application-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[アプリケーションを取得します。](../api/application-get.md) | application |アプリケーション オブジェクトのプロパティと関係を参照してください。|
|[アプリケーションを作成します。](../api/application-post-applications.md) | application | (レジスタ) を作成する新しいアプリケーションです。|
|[アプリケーション一覧](../api/application-list.md) | application | 組織内のアプリケーションの一覧を取得します。 |
|[アプリケーションを更新します。](../api/application-update.md) | application |アプリケーション オブジェクトを更新します。 |
|[アプリケーションを削除します。](../api/application-delete.md) | なし |アプリケーション オブジェクトを削除します。 |
|[リストが割り当てられているポリシー](../api/policy-list-assigned.md)| [ポリシー](policy.md)コレクション| このオブジェクトに割り当てられているすべてのポリシーを取得します。|
|[所有者を作成します。](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| 所有者のコレクションへの投稿には、新しい所有者を作成します。|
|[所有者を一覧表示する](../api/application-list-owners.md) |[directoryObject](directoryobject.md) コレクション| 所有者オブジェクトのコレクションを取得します。|
|[delta](../api/application-delta.md)|アプリケーション コレクション| アプリケーションの増分の変更を取得します。 |
|[呼び出しを作成します。](../api/application-post-calls.md)|[呼び出し](call.md)|呼び出しのコレクションへの投稿には、新しい呼び出しを作成します。|
|[オンライン会議を作成します。](../api/application-post-onlinemeetings.md)|[onlineMeeting](onlinemeeting.md)|OnlineMeetings コレクションへの投稿には、新しいオンライン ミーティングを作成します。|

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:---------------|:--------|:----------|
|api|[api](api.md)| API アプリケーションの設定を指定します。 |
|appId| 文字列型 (String) | Azure AD でアプリケーションに割り当てられているアプリケーションの一意の識別子です。 null 許容ではありません。 読み取り専用です。 |
|appRoles|[エンティティ](approle.md)のコレクション|アプリケーションが宣言されているアプリケーション ロールのコレクションです。 これらのロールは、ユーザー、グループ、またはサービス ・ プリンシパルを指定できます。 null 許容ではありません。|
|createdDateTime|DateTimeOffset| 日付と時刻、アプリケーションが登録されています。 |
|deletedDateTime|DateTimeOffset| 日付と時刻、アプリケーションが削除されました。 |
|displayName|String|アプリケーションの表示名です。 |
|id|String|アプリケーションの一意の識別子です。 [directoryObject](directoryobject.md) から継承されます。 キー。 null 許容ではありません。 読み取り専用です。 |
|identifierUris|String コレクション| アプリケーションを識別する Uri。 詳細情報は、「[アプリケーションのオブジェクトおよびオブジェクトのサービス プリンシパル](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/)です。 *Any*演算子は、複数値を持つプロパティのフィルター式に必要です。 null 許容ではありません。 |
|情報|[informationalUrl](informationalurl.md)| アプリケーションの基本的なプロファイル情報です。 |
|isFallbackPublicClient|ブール型| パブリック クライアント モバイル デバイスで実行されているインストール済みのアプリケーションとして、代替のアプリケーションの種類を指定します。 既定値は*false*フォールバックのアプリケーションの種類は、web アプリケーションなどの機密性の高いクライアントです。 Azure AD がクライアント アプリケーションの種類 (例: リダイレクト URI を指定することがなく構成されている[ROPC](https://tools.ietf.org/html/rfc6749#section-4.3)フロー) を判断できない特定のシナリオがあります。 このような場合に、Azure AD がこのプロパティの値に基づいてアプリケーションの種類を解釈します。|
|keyCredentials|[keyCredential](keycredential.md)コレクション|しないアプリケーションに関連付けられているキーの資格情報のコレクション null 許容型です。 |
|logo|Stream|アプリケーションのメインのロゴです。 null 許容ではありません。 |
|optionalClaims|optionalClaims| 将来の使用のために予約されています。 |
|orgRestrictions|String コレクション| 将来の使用のために予約されています。 |
|parentalControlSettings|[parentalControlSettings](parentalcontrolsettings.md) |アプリケーションの視聴制限の設定を指定します。|
|passwordCredentials|[passwordCredential](passwordcredential.md)コレクション|アプリケーションに関連付けられているパスワード資格情報のコレクションです。 null 許容ではありません。|
|publicClient|[publicClient](publicclient.md)| デスクトップやモバイル デバイスなどのインストールされているクライアントの設定を指定します。 |
|publisherDomain| String | アプリケーションの確認された発行元のドメイン。 読み取り専用です。|
|requiredResourceAccess|[requiredResourceAccess](requiredresourceaccess.md)コレクション|このアプリケーションへのアクセスと、OAuth アクセス許可のスコープおよび各リソースの下に必要なアプリケーション ロールのセットを必要とするリソースを指定します。 必要なリソースへのアクセスのこの前の構成では、同意の経験をドライブします。 null 許容ではありません。|
|signInAudience | String | 現在のアプリケーションのサポートはどのような Microsoft アカウントを指定します。 サポートされている値は次のとおりです。<ul><li>**AzureADMyOrg**: microsoft のユーザーまたは組織の Azure AD テナント (つまり単一のテナント) でアカウントの学校</li><li>**AzureADMultipleOrgs**: microsoft ユーザーは、作業や、学校でどのような組織の Azure AD テナント (マルチ テナント型など) のアカウント</li> <li>**AzureADandPersonalMicrosoftAccount**: Microsoft の個人アカウントでは、またはどのような組織の Azure AD テナントで、職場、学校のアカウントを持つユーザー</li></ul> | `AzureADandPersonalMicrosoftAccount` |
|タグの前に追加されるマークアップ|String コレクション| 分類し、アプリケーションの識別に使用できるカスタム文字列。 |
|web|[web](web.md)| Web アプリケーションの設定を指定します。 |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型 | 説明 |
|:---------------|:--------|:----------|
|呼び出し           |コレクションの[呼び出し](call.md)                  |読み取り専用。Null 許容型。|
|connectorGroup|[connectorGroup](connectorgroup.md)| ConnectorGroup アプリケーションは、Azure AD アプリケーション プロキシを使用しています。 Null 許容型。|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| 読み取り専用です。|
|onlineMeetings  |[onlineMeeting](onlinemeeting.md)コレクション|読み取り専用。Null 許容型。|
|owners|[directoryObject](directoryobject.md) コレクション|ディレクトリ オブジェクト、アプリケーションの所有者であります。 所有者は、このオブジェクトを変更するのには許可されている管理者以外のユーザーのセットです。 2013-11-08 のバージョンが必要ですまたはそれ以降です。 読み取り専用です。 Null 許容型。|
|役割|[ポリシー](policy.md)コレクション|このアプリケーションに割り当てられているポリシーです。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "createdOnBehalfOf",
    "owners"
  ],
  "@odata.type": "microsoft.graph.application"
}-->

```json
{
  "api": {"@odata.type": "microsoft.graph.apiApplication"},
  "appId": "String",
  "appRoles": [{"@odata.type": "microsoft.graph.appRole"}],
  "createdDateTime": "String (timestamp)",
  "deletedDateTime": "String (timestamp)",
  "displayName": "String",
  "id": "String (identifier)",
  "identifierUris": ["String"],
  "info": {"@odata.type": "microsoft.graph.informationalUrl"},
  "isFallbackPublicClient": true,
  "keyCredentials": [{"@odata.type": "microsoft.graph.keyCredential"}],
  "logo": "Stream",
  "optionalClaims": [{"@odata.type": "microsoft.graph.optionalClaims"}],
  "orgRestrictions": ["Guid"],
  "parentalControlSettings": [{"@odata.type": "microsoft.graph.parentalControlSettings"}],
  "passwordCredentials": [{"@odata.type": "microsoft.graph.passwordCredential"}],
  "preAuthorizedApplications": [{"@odata.type": "microsoft.graph.preAuthorizedApplication"}],
  "publicClient": {"@odata.type": "microsoft.graph.publicClientApplication"},
  "publisherDomain": "String",
  "requiredResourceAccess": [{"@odata.type": "microsoft.graph.requiredResourceAccess"}],
  "signInAudience": "String",
  "tags": ["String"],
  "web": {"@odata.type": "microsoft.graph.webApplication"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
