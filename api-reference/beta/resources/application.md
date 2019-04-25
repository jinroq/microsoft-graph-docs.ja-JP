---
title: アプリケーション リソースの種類
description: 'これはアプリケーションを表すものです。 Azure Active Directory (Azure AD) に認証をアウトソースするすべてのアプリケーションは、ディレクトリに登録する必要があります。 アプリケーションの登録では、アプリケーションに関する情報 (場所の URL、認証後に返信を送信する URL、アプリケーションを識別する URI など) を Azure AD に通知する必要があります。 詳細については、Azure AD でのアプリケーションの登録の基本を参照してください。 directoryObject から継承します。 '
localization_priority: Priority
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 694f6b12dd8fe1fd59f12cafebd47c842a4077cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548204"
---
# <a name="application-resource-type"></a>アプリケーション リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

これはアプリケーションを表すものです。 Azure Active Directory (Azure AD) に認証をアウトソースするすべてのアプリケーションは、ディレクトリに登録する必要があります。 アプリケーションの登録では、アプリケーションに関する情報 (場所の URL、認証後に返信を送信する URL、アプリケーションを識別する URI など) を Azure AD に通知する必要があります。 詳細については、[Azure AD でのアプリケーションの登録の基本](https://azure.microsoft.com/documentation/articles/active-directory-authentication-scenarios/#basics-of-registering-an-application-in-azure-ad)を参照してください。 [directoryObject](directoryobject.md) から継承します。 

> **注:** アプリケーション リソースの種類に対する変更は、現在開発中です。 詳細については、「[Microsoft Graph に関する既知の問題](/graph/known-issues#application-and-serviceprincipal-api-changes)」を参照してください。

このリソースは以下をサポートしています。

- [デルタ](../api/application-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[アプリケーションを取得する](../api/application-get.md) | application |アプリケーション オブジェクトのプロパティと関係を読み取ります。|
|[アプリケーションを作成する](../api/application-post-applications.md) | application | 新しいアプリケーションを作成 (登録) します。|
|[アプリケーションを一覧表示する](../api/application-list.md) | application | 組織内のアプリケーションの一覧を取得します。 |
|[アプリケーションを更新する](../api/application-update.md) | application |アプリケーション オブジェクトを更新します。 |
|[アプリケーションを削除する](../api/application-delete.md) | なし |アプリケーション オブジェクトを削除します。 |
|[割り当てられているポリシーを一覧表示する](../api/policy-list-assigned.md)| [policy](policy.md) コレクション| このオブジェクトに割り当てられているすべてのポリシーを取得します。|
|[所有者を作成する](../api/application-post-owners.md) |[directoryObject](directoryobject.md)| 所有者のコレクションに投稿して、新しい所有者を作成します。|
|[所有者を一覧表示する](../api/application-list-owners.md) |[directoryObject](directoryobject.md) コレクション| 所有者オブジェクトのコレクションを取得します。|
|[デルタ](../api/application-delta.md)|application コレクション| アプリケーションに対する増分の変更を取得します。 |
|[通話の作成](../api/application-post-calls.md)|[call](call.md)|通話のコレクションに投稿して新しい通話を作成します。|
|[オンライン会議を作成する](../api/application-post-onlinemeetings.md)|[onlineMeeting](onlinemeeting.md)|onlineMeetings コレクションに投稿して、新しいオンライン会議を作成します。|

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|api|[api](api.md)| API アプリケーションの設定を指定します。 |
|appId| String | Azure AD によってアプリケーションに割り当てられる、アプリケーションの一意の識別子です。 null 許容型ではありません。 読み取り専用です。 |
|appRoles|[appRole](approle.md) コレクション|アプリケーションで宣言できるアプリケーション ロールのコレクションです。 これらのロールは、ユーザー、グループ、サービス プリンシパルなどに割り当てることができます。 null 許容型ではありません。|
|createdDateTime|DateTimeOffset| アプリケーションが登録された日付と時刻です。 |
|deletedDateTime|DateTimeOffset| アプリケーションが削除された日付と時刻です。 |
|displayName|String|アプリケーションの表示名。 |
|id|String|アプリケーションの一意の識別子です。 [directoryObject](directoryobject.md) から継承されます。 キー。 null 許容ではありません。 読み取り専用です。 |
|identifierUris|String コレクション| アプリケーションを識別する URI です。 詳細については、「[Azure Active Directory のアプリケーション オブジェクトとサービス プリンシパル オブジェクト](https://azure.microsoft.com/documentation/articles/active-directory-application-objects/)」を参照してください。 複数値プロパティのフィルター式には *any* 演算子が必要です。 null 許容型ではありません。 |
|info|[informationalUrl](informationalurl.md)| アプリケーションの基本的なプロファイル情報です。 |
|isFallbackPublicClient|Boolean| モバイル デバイスで実行されているインストール済みアプリなど、フォールバック アプリの種類をパブリック クライアントとして指定します。 既定値は *false* です。つまりフォールバック アプリの種類は Web アプリなどの機密性の高いクライアントです。 Azure AD がクライアント アプリの種類を特定できないシナリオ (例: リダイレクト URI を指定せずに構成されている [ROPC](https://tools.ietf.org/html/rfc6749#section-4.3) フロー) もあります。 そのような場合、Azure AD では、このプロパティの値に基づいてアプリの種類を解釈します。|
|keyCredentials|[keyCredential](keycredential.md) コレクション|アプリケーションに関連付けられているキー資格情報のコレクションです。null 許容型ではありません。 |
|logo|Stream|アプリケーションのメイン ロゴです。 null 許容型ではありません。 |
|optionalClaims|optionalClaims| 将来使用するために予約されています。 |
|orgRestrictions|String コレクション| 将来使用するために予約されています。 |
|parentalControlSettings|[parentalControlSettings](parentalcontrolsettings.md) |アプリケーションにおける、保護者による制限設定を指定します。|
|passwordCredentials|[passwordCredential](passwordcredential.md) コレクション|アプリケーションに関連付けられているパスワード資格情報のコレクションです。 null 許容型ではありません。|
|publicClient|[publicClient](publicclient.md)| デスクトップやモバイル デバイスなど、インストールされているクライアントの設定を指定します。 |
|publisherDomain| String | アプリケーションの確認済み発行元のドメインです。 読み取り専用です。|
|requiredResourceAccess|[requiredResourceAccess](requiredresourceaccess.md) コレクション|このアプリケーションがアクセスする必要があるリソース、およびそのリソースで必要な OAuth アクセス許可の範囲とアプリケーション ロールのセットを指定します。 必要なリソースへのアクセスに対するこの事前構成によって、同意エクスペリエンスが促進されます。 null 許容型ではありません。|
|signInAudience | String | 現在のアプリケーションでサポートされている Microsoft アカウントを指定します。 サポートされている値は次のとおりです。<ul><li>**AzureADMyOrg**: 組織の Azure AD テナント (つまり、シングル テナント) で Microsoft の職場または学校アカウントを持つユーザー</li><li>**AzureADMultipleOrgs**: 組織の Azure AD テナント (つまり、マルチ テナント) で Microsoft の職場または学校アカウントを持つユーザー</li> <li>**AzureADandPersonalMicrosoftAccount**: 個人の Microsoft アカウントを持つユーザー、または組織の Azure AD テナントで職場または学校のアカウントを持つユーザー</li></ul> | `AzureADandPersonalMicrosoftAccount` |
|tags|String コレクション| アプリケーションを分類および識別するために使用できるカスタム文字列です。 |
|web|[web](web.md)| Web アプリケーションの設定を指定します。 |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型 | 説明 |
|:---------------|:--------|:----------|
|calls           |[call](call.md) コレクション                  |読み取り専用です。 Null 許容型。|
|connectorGroup|[connectorGroup](connectorgroup.md)| アプリケーションが Azure AD アプリケーション プロキシで使用している connectorGroup です。 Null 許容型です。|
|createdOnBehalfOf|[directoryObject](directoryobject.md)| 読み取り専用です。|
|onlineMeetings  |[onlineMeeting](onlinemeeting.md) コレクション|読み取り専用。Null 許容型です。|
|owners|[directoryObject](directoryobject.md) コレクション|アプリケーションの所有者であるディレクトリ オブジェクトです。 所有者は、このオブジェクトの変更を許可されている管理者以外のユーザーです。 バージョン 2013-11-08 以降が必要です。 読み取り専用です。 Null 許容型です。|
|policy|[policy](policy.md) コレクション|このアプリケーションに割り当てられているポリシーです。|

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
<!--
{
  "type": "#page.annotation",
  "description": "application resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/application.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
