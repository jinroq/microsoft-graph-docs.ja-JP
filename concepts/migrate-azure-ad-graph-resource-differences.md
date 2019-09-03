---
title: Azure AD Graph と Microsoft Graph のリソースの種類の違い
description: アプリを移行するために、Azure AD Graph のリソースと Microsoft Graph のリソースの違いについて説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 23a27e80027e6c862c32648bb452770cf3e27b5c
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667598"
---
# <a name="resource-type-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD Graph と Microsoft Graph のリソースの種類の違い

この記事は、*手順 1:* [アプリを移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の API の相違点を確認します。

Azure AD Graph から Microsoft Graph にアプリを移行するときは、リソースによって名前と種類が異なることに注意してください。  たとえば、Azure AD Graph アプリが**Tenantinfo**リソースを使用している場合は、代わりに[組織](/graph/api/resources/organization?view=graph-rest-1.0)を参照するようにコードを更新する必要があります。

次の表に、Azure AD Graph と Microsoft Graph のリソースの違いを示します。  名前が異なるリソースが表示されているか、使用できません。また、Microsoft Graph のベータ版では使用できても、v2.0 バージョンでは利用できないリソースも強調表示されています。

この一覧にリソースが表示されていない場合は、Azure AD Graph と同じ名前で、既に Microsoft Graph の v1.0[バージョン](/graph/api/overview?view=graph-rest-1.0)で使用できます。

> **メモ**: Azure AD graph のリソースの種類の名前は Pascal 形式ですが、Microsoft Graph では camel 形式になっています。

|Azure AD Graph <br>(v2.0) リソース |Microsoft Graph<br>リソース|Comments|
|---|---|---|
| [AddIn](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference)       | ベータ版_はまだ利用できません_<br>v 1.0-_まだ使用できません_ ||
| [Application](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ-[アプリケーション](/graph/api/resources/application?view=graph-rest-beta)<br>v 1.0-_まだ使用できません_ ||
| [AppRole](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ[承認 le](/graph/api/resources/approle?view=graph-rest-beta)<br>v 1.0-_まだ使用できません_ | |
| [AppRoleAssignment](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp;-ベータ&nbsp;[承認 leassignment](/graph/api/resources/approleassignment?view=graph-rest-beta)<br>v 1.0-_まだ使用できません_ | |
| [CertificateAuthorityInformation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ&nbsp;-&nbsp;版の[certificateauthority](/graph/api/resources/certificateauthority?view=graph-rest-beta)<br>version 1.0&nbsp;-&nbsp;_はまだ利用できません_ | |
| [Contact](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ版の[連絡先](/graph/api/resources/orgContact?view=graph-rest-beta)<br>v 1.0-_まだ使用できません_ | |
| [DirectoryLinkChange](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ-_新&nbsp;手法_ <br>v2.0 1.0-_新しい&nbsp;方法_ | デルタクエリは、このリソースを必要としないメカニズムで、リレーションシップの変更の検出をサポートします。 「 [AZURE AD graph と Microsoft Graph の機能の違い」を](migrate-azure-ad-graph-feature-differences.md)参照してください。 |
| [KeyCredential](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference)| β- [Keycredential](/graph/api/resources/keyCredential?view=graph-rest-beta)<br>v 1.0-_まだ使用できません_ | |
| [KeyValue](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ- [keyValue](/graph/api/resources/keyValue?view=graph-rest-beta) <br> v 1.0-_まだ使用できません_ ||
| [OAuth2Permission](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ- [Permissionscope](/graph/api/resources/permissionScope?view=graph-rest-beta) <br> v 1.0-_まだ使用できません_ ||
| [OAuth2PermissionGrant](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ&nbsp;-&nbsp;版[oAuth2PermissionGrant](/graph/api/resources/oAuth2PermissionGrant?view=graph-rest-beta) <br> v 1.0-_まだ使用できません_ ||
| [任意の Claim](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ版の要求 <br> v 1.0-_まだ使用できません_ | |
| [任意のクレーム](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ版のクレーム<br> v 1.0-_まだ使用できません_ ||
| [ParentalControlSettings](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ- [Parentalcontrolsettings](/graph/api/resources/parentalcontrolsettings?view=graph-rest-beta) <br> v 1.0-_まだ使用できません_ ||
| [PasswordCredential](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ- [Passwordcredential](/graph/api/resources/passwordCredential?view=graph-rest-beta) <br> v 1.0-_まだ使用できません_ ||
| [PasswordProfile](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ- [Passwordprofile](/graph/api/resources/passwordProfile?view=graph-rest-beta) <br> v 1.0-PasswordProfile ||
| [ポリシー](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ-[ポリシー](/graph/api/resources/parentalcontrolsettings?view=graph-rest-beta) _(変更する対象)_ <br> v 1.0-_まだ使用できません_ | 各ポリシーには、一意の種類の名前と構造があります。|
| [プロビジョニングエラー](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ&nbsp;-&nbsp;版_は使用できません_ <br> version 1.0&nbsp;-&nbsp;_は使用できません_ | このリソースは推奨されていません。  ただし、AD Connect 関連のプロビジョニングエラーを説明する新しいリソースは、 [onPremisesProvisioningError](/graph/api/resources/onPremisesProvisioningError?view=graph-rest-v1.0)にあります。 |
| [RequiredResourceAccess](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ版の[Resourceaccess](/graph/api/resources/requiredResourceAccess?view=graph-rest-beta) <br> v 1.0-_まだ使用できません_ | |
| [ResourceAccess](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ- [Resourceaccess](/graph/api/resources/resourceAccess?view=graph-rest-beta) <br> v 1.0-_まだ使用できません_ | |
| [ServiceEndpoint](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ[エンドポイント](/graph/api/resources/endpoint?view=graph-rest-beta) <br> v1.0-エンドポイント_はまだ利用できません_ | [エンドポイント](/graph/api/resources/endpoint?view=graph-rest-beta)は、[グループ](/graph/api/resources/group?view=graph-rest-beta)リソースの一部としてのみ使用できます。|
| [ServicePrincipal](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ- [Serviceprincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) <br> v 1.0-_まだ使用できません_ | |
| [SignInName](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | ユーザーアカウントへのサインインに使用されているがまだ使用**** できない識別子の新しいモデル。 Azure AD B2C シナリオをサポートします。 |
| [TenantDetail](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ-[組織](/graph/api/resources/organization?view=graph-rest-beta) <br> v 1.0-[組織](/graph/api/resources/organization?view=graph-rest-v1.0) | |
| [TrustedCasForPasswordAuth](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | &nbsp;-ベータ&nbsp;の[certificateベース authconfiguration](/graph/api/resources/certificatebasedcuthconfiguration?view=graph-rest-beta) <br> v 1.0-_まだ使用できません_ | |
| [UserIdentity](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/entity-and-complex-type-reference) | ベータ版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ |  ユーザーアカウントへのサインインに使用されているがまだ使用**** できない識別子の新しいモデル。 Azure AD B2C シナリオをサポートします。 |

## <a name="next-steps"></a>次のステップ

- Azure AD Graph と Microsoft Graph の[エンティティプロパティの違い](migrate-azure-ad-graph-property-differences.md)について説明します。
- [Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。
- [Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。
