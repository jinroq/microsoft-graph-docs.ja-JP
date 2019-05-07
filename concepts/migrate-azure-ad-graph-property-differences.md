---
title: Azure AD Graph と Microsoft Graph のプロパティの相違点
description: アプリを移行するために、Azure AD Graph リソース (エンティティ) と Microsoft Graph のプロパティの相違点について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e2f8ba237cd86ab2361c98f5b51afaa77d2b7f50
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33630217"
---
# <a name="property-differences-between-azure-ad-graph-and-microsoft-graph"></a>Azure AD Graph と Microsoft Graph のプロパティの相違点

この記事は、*手順 1:* [アプリを移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の API の相違点を確認します。

一般的に、Azure AD Graph API を Microsoft Graph と比較する最善の方法は、各サービスの基になるメタデータを比較することです (特にリソースの説明)。

- [Azure AD Graph のメタデータ](https://graph.windows.net/microsoft.com/$metadata?api-version=1.6)
- [Microsoft Graph beta メタデータ](https://graph.microsoft.com/beta /$metadata)
- [Microsoft Graph version 1.0 のメタデータ](https://graph.microsoft.comv/1.0/$metadata)

ここでは、リソース間のプロパティの違いが強調表示されています。 プロパティがこの一覧に表示されていない場合は、既に v2.0[バージョン](/graph/api/overview?view=graph-rest-1.0)の Microsoft Graph で使用できます。これは、Azure AD Graph とまったく同じ名前です。

ユーザーとグループが頻繁に使用されるため、これらのリソースが最初に表示されます。  その他のリソースはアルファベット順に表示されます。

## <a name="user-property-differences"></a>ユーザープロパティの違い

|Azure AD Graph <br>(v 1.6) プロパティ |Microsoft Graph<br>プロパティ|Comments|
|---|---|---|
| **appRoleAssignments** | ベータ**承認の Leassignments** <br> v 1.0-_まだ使用できません_ | |
| **/テキスト** | ベータ版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_| |
| **deletedTimestamp**| ベータ- **deletedDateTime** <br> v 1.0- **deletedDateTime** | |
| **dirSyncEnabled** | ベータ&nbsp; - &nbsp;版**onPremisesSyncEnabled** <br> v 1.0- **onPremisesSyncEnabled** | |
| **facsimileTelephoneNumber** | β- **Fax 番号** <br> v 1.0- **Fax 番号** | |
| **immutableId** | ベータ&nbsp; - &nbsp;版**onPremisesImmutableId** <br> v 1.0- **onPremisesImmutableId**  | |
| **漏洩** | ベータ版_は使用できません_ <br> v2.0 1.0-_使用_不可 | Microsoft Graph [id 保護](/graph/api/resources/identityprotection-root?view=graph-rest-beta)API は、より高度な機能を提供します。 |
| **lastDirSyncDateTime** | ベータ&nbsp; - &nbsp;版**onPremisesLastSyncDateTime** <br> v 1.0- **onPremisesLastSyncDateTime** | |
| **mobile** | ベータ- **mobilePhone** <br> v 1.0- **mobilePhone** | |
| **oAuth2PermissionGrants** | ベータ- **oAuth2PermissionGrants** <br> v 1.0-_まだ使用できません_ ||
| **プロビジョニングエラー** | ベータ&nbsp; - &nbsp;版**onPremisesProvisioningErrors** <br> v 1.0- **onPremisesProvisioningErrors** | |
| **refreshTokensValidFromDateTime** | ベータ&nbsp;-&nbsp;版**signinSessionsValidFromDateTime**<br>version 1.0&nbsp;-&nbsp;_はまだ利用できません_ | |
| **signinNames** | ベータ版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | |
| **電話番号** | ベータ- **businessPhones** <br> v 1.0- **businessPhones** | |
| **thumbnailPhoto** | ベータ-**写真**、写真 <br> v 1.0-**写真**、写真 | Azure AD のサムネイル写真は、Microsoft Graph からは使用できません。  代わりに、 [PHOTO API](/graph/api/resources/profilephoto?view=graph-rest-1.0)を使用してください。 |
| **userIdentities** | ベータ版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | |
| **userState** | ベータ- **Externaluserstate** <br> v 1.0- **Externaluserstate** | |
| **userStateChangedOn** | ベータ&nbsp;-&nbsp;版**externalUserStateChangeDateTime**<br>v 1.0&nbsp;-&nbsp;**externalUserStateChangeDateTime** | |

## <a name="group-property-differences"></a>グループプロパティの違い

|Azure AD Graph <br>(v 1.6) プロパティ |Microsoft Graph<br> プロパティ|Comments|
|---|---|---|
| **dirSyncEnabled** | ベータ&nbsp; - &nbsp;版**onPremisesSyncEnabled** <br> v 1.0- **onPremisesSyncEnabled** | |
| **immutableId** | ベータ&nbsp; - &nbsp;版**onPremisesImmutableId** <br> v 1.0- **onPremisesImmutableId** | |
| **lastDirSyncDateTime** | ベータ&nbsp;-&nbsp;版**onPremisesLastSyncDateTime**<br>v 1.0- **onPremisesLastSyncDateTime** | |
| **onPremisesDomainName** | ベータ版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | 計画済みですが、まだ使用できません。 |
| **onPremisesNetBiosName** | ベータ版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | 計画済みですが、まだ使用できません。 |
| **onPremisesSamAccountName** | ベータ版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | 計画済みですが、まだ使用できません。 |
| **プロビジョニングエラー** | ベータ&nbsp;-&nbsp;版**onPremisesProvisioningErrors**<br> v 1.0- **onPremisesProvisioningErrors** | |

## <a name="application-property-differences"></a>アプリケーションプロパティの違い

|Azure AD Graph <br>(v 1.6) プロパティ |Microsoft Graph<br> プロパティ|Comments|
|---|---|---|
| **acceptMappedClaims**  | &nbsp; -ベータ&nbsp; **api/acceptMappedClaims** <br> v 1.0-_まだ使用できません_ | acceptMappedClaims が新しい api リソースの一部になりました。 |
| **アドイン** | ベータ版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_  | |
| **applicationTemplateId** | ベータ版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | |
| **Availabletoothertenants から** | ベータ&nbsp; - &nbsp;版**orgRestrictions** <br> v 1.0-_まだ使用できません_ | |
| **errorUrl**| ベータ&nbsp; - &nbsp;版_は使用できません_ <br> v2.0 1.0-_使用_不可 | このプロパティは推奨されていません。|
| **HomePage**| ベータ&nbsp; - &nbsp;版**web/ホームページ** <br> v 1.0-_まだ使用できません_ | ホームページが新しい web リソースの一部になっています。|
| **Information Alurl**| ベータ&nbsp; - &nbsp;版**情報** <br> v 1.0-_まだ使用できません_ | |
| **knownClientApplications**| &nbsp;-ベータ&nbsp;**api/knownclientapplications** <br> v 1.0-_まだ使用できません_ | knownClientApplications は新しい api リソースの一部になりました。 |
| **logoutUrl**| ベータ&nbsp; - &nbsp;版**web/ログインアウト url** <br> v 1.0-_まだ使用できません_ | logoutUrl が web リソースの一部になりました。 |
| **logoUrl**| &nbsp; -ベータ&nbsp;**情報/logoUrl** <br> v 1.0-_まだ使用できません_ | logoUrl が新しい info リソースの一部になりました。 |
| **Mainlogo から logo**| ベータ&nbsp; - &nbsp;版_は使用できません_ <br> v2.0 1.0-_使用_不可 | このプロパティは推奨されていません。|
| **oauth2AllowIdTokenImplicitFlow** | ベータ&nbsp;-&nbsp;版**web/implicitGrantSettings/enableidtokenissuance**<br>v 1.0-_まだ使用できません_ | 名前が変更され、新しい implicitGrantSettings リソースの一部になっています。 |
| **oauth2AllowImplicitFlow**| ベータ&nbsp;-&nbsp;版**web/oauth2AllowImplicitFlow**<br>v 1.0-_まだ使用できません_ | oauth2AllowImplicitFlow が新しい web リソースの一部になりました。 |
| **oauth2AllowUrlPathMatching**| ベータ&nbsp; - &nbsp;版_は使用できません_ <br> v2.0 1.0-_使用_不可 | このプロパティは推奨されていません。|
| **oauth2Permissions**| &nbsp;-ベータ&nbsp;**api/oauth2PermissionScopes**<br> v 1.0-_まだ使用できません_ | 名前が変更され、新しい api リソースの一部になりました。 |
| **oauth2RequirePostResponse**| ベータ&nbsp; - &nbsp;版_は使用できません_ <br> v2.0 1.0-_使用_不可 | このプロパティは推奨されていません。|
| **publicClient**| &nbsp; - β &nbsp; **isfallbackpublicclient** <br> v 1.0-_まだ使用できません_ | このプロパティには新しい意味があります。これには、redirectUris のようなパブリッククライアントの設定が含まれています。 アプリが公開されているか、または機密クライアントであるかを判別し、isFallbackPublicClient プロパティを使用して自動的に決定できない1つの特殊なケースを処理するようになりました。|
| **recordConsentConditions**| ベータ&nbsp; - &nbsp;版_は使用できません_ <br> v2.0 1.0-_使用_不可 | このプロパティは推奨されていません。|
| **replyUrls**| ベータ&nbsp;-&nbsp;版の**web/redirecturis**<br> v 1.0-_まだ使用できません_ | 名前が変更されているだけでなく、redirectUris が新しい web リソースの一部になっています。 | |
| **samlMetadataUrl**| ベータ版_はまだ利用できません_  <br> v 1.0-_まだ使用できません_  | |
| **extensionProperties**| &nbsp; -β &nbsp; **extensionproperties** <br> v 1.0-_まだ使用できません_ | このプロパティは推奨されていません。 |
| **serviceEndpoints**|  ベータ版_はまだ利用できません_  <br> v 1.0-_まだ使用できません_  | |

## <a name="approleassignment-differences"></a>承認の Leassignment の違い

|Azure AD Graph <br>(v 1.6) プロパティ |Microsoft Graph<br> プロパティ|Comments|
|---|---|---|
| **creationTimestamp** | ベータ&nbsp; - &nbsp;版の**タイムスタンプ** <br> v 1.0-_まだ使用できません_ | これは、"いいね!" という名前に変更されます。|
| **id** | &nbsp; -ベータ&nbsp;の**承認 leid** <br> v 1.0-_まだ使用できません_ | |

## <a name="contact-property-differences"></a>連絡先プロパティの違い

Azure AD Graph 連絡先リソースは、Microsoft Graph の orgContact に名前が変更されました。  プロパティの相違点は次のとおりです。

|Azure AD Graph <br>(v 1.6) プロパティ |Microsoft Graph<br> プロパティ|Comments|
|---|---|---|
| **city** | &nbsp;-ベータ&nbsp;**住所 (市町村)** <br> v 1.0-_まだ使用できません_  | City プロパティは、addresses リソースコレクションの一部です。 |
| **country** | &nbsp;-ベータ&nbsp;**** アドレス&nbsp;**(countryOrRegion)**<br> v 1.0-_まだ使用できません_  | CountryOrRegion プロパティは、addresses リソースコレクションの一部です。 |
| **dirSyncEnabled** | ベータ&nbsp; - &nbsp;版**onPremisesSyncEnabled** <br> v 1.0-_まだ使用できません_  | |
| **facsimileTelephoneNumber** | ベータ&nbsp;-&nbsp;版**電話****** (businessfax)&nbsp; <br> v 1.0-_まだ使用できません_ | これで、携帯電話、business、および businessFax をサポートする phone コレクションの一部になりました。 |
| **physicalDeliveryOfficeName** | &nbsp; -ベータ&nbsp;**オフィスの場所** <br> v 1.0- **Officelocation** | |
| **postalCode** | &nbsp;-ベータ&nbsp;**** 住所&nbsp;**(郵便番号)**<br> v 1.0-_まだ使用できません_  | "郵便番号" プロパティは、addresses リソースコレクションの一部です。 |
| **プロビジョニングエラー** | ベータ&nbsp;-&nbsp;版**onPremisesProvisioningErrors**<br> v 1.0-_まだ使用できません_  | |
| **sipProxyAddress** |  &nbsp; -ベータ&nbsp; **imaddresses**<br> v 1.0-_まだ使用できません_  | |
| **state** | &nbsp; -ベータ&nbsp; **** アドレス&nbsp;**(都道府県)**<br> v 1.0-_まだ使用できません_  | State プロパティは、addresses リソースコレクションの一部です。 |
| **streetAddress** | &nbsp; -ベータ&nbsp; **** 住所&nbsp;**(番地)**<br> v 1.0-_まだ使用できません_  | ストリートプロパティは、addresses リソースコレクションの一部です。 |
| **電話番号** | ベータ&nbsp;-&nbsp;版**電話****** (business)&nbsp; <br> v 1.0-_まだ使用できません_ | これで、携帯電話、business、および businessFax をサポートする phone コレクションの一部になりました。 |
| **thumbnailPhoto** | ベータ&nbsp; - &nbsp;_版&nbsp;は&nbsp;まだ利用できません_&nbsp;<br> v 1.0-_まだ使用できません_ | |

## <a name="contract-property-differences"></a>Contract プロパティの違い

|Azure AD Graph <br>(v 1.6) プロパティ |Microsoft Graph<br> プロパティ|Comments|
|---|---|---|
| **customerContextId** | ベータ&nbsp; - &nbsp;版**customerId** <br> version 1.0- **customerId**  |  |

## <a name="device-property-differences"></a>デバイスプロパティの違い

|Azure AD Graph <br>(v 1.6) プロパティ |Microsoft Graph<br> プロパティ|Comments|
|---|---|---|
| **approximateLastLogonTimestamp** | ベータ&nbsp;-&nbsp;版**approximateLastSignInDateTime** <br> v 1.0- **approximateLastSignInDateTime** |  |
| **complianceExpiryTime** | ベータ&nbsp;-&nbsp;版**complianceExpirationDateTime** <br> v 1.0- **complianceExpirationDateTime** |  |
| **deviceObjectVersion** |  &nbsp;-ベータ&nbsp;**デバイスバージョン** <br> v 1.0- **Deviceversion** |  |
| **deviceOSType** | ベータ&nbsp;-&nbsp;版**operatingSystem** <br> v 1.0- **operatingSystem** |  |
| **deviceOSVersion** | ベータ&nbsp;-&nbsp;版**operatingSystemVersion** <br> v 1.0- **operatingSystemVersion** |  |
| **devicePhysicalIds** | ベータ&nbsp;-&nbsp;版**physicalIds** <br> v 1.0- **physicalIds** |  |
| **deviceTrustType** | &nbsp;-ベータ&nbsp;の**trusttype** <br> v 1.0- **Trusttype** |  |
| **dirSyncEnabled** |  ベータ&nbsp;-&nbsp;版**onPremisesSyncEnabled** <br> v 1.0- **onPremisesSyncEnabled** |  |
| **lastDirSyncTime** |  ベータ&nbsp;-&nbsp;版**onPremisesLastSyncDateTime** <br> v 1.0- **onPremisesLastSyncDateTime** |  |

## <a name="directoryobjectreference-property-differences"></a>DirectoryObjectReference プロパティの違い

Azure AD Graph directoryObjectReference リソースは、Microsoft Graph の directoryObjectPartnerReference に名前が変更されました。  プロパティの相違点は次のとおりです。

|Azure AD Graph <br>(v 1.6) プロパティ |Microsoft Graph<br> プロパティ|Comments|
|---|---|---|
| **externalContextId** | &nbsp;-ベータ&nbsp;**externalpartnertenantid** <br> v 1.0- **Externalpartnertenantid** |  |

## <a name="domain-property-differences"></a>ドメインプロパティの違い

|Azure AD Graph <br>(v 1.6) プロパティ |Microsoft Graph<br> プロパティ|Comments|
|---|---|---|
| **name** | &nbsp;-ベータ&nbsp;**id** <br> v 1.0- **id** | Microsoft Graph では、一意識別子 (id) にドメイン名が含まれています。プロパティ`name`が存在しません。 |
| **forceDeleteState** |  &nbsp;-ベータ&nbsp;**状態** <br> v 1.0-**状態** | Azure AD Graph には、forceDelete と domain 状態の個別のプロパティがあります。  Microsoft Graph では、すべてのドメインの状態は state プロパティによって処理されます。 |
| **isDefaultForCloudRedirections** | ベータ&nbsp;-&nbsp;_版&nbsp;は&nbsp;まだ利用できません_&nbsp;<br> v 1.0-_まだ使用できません_ | |

## <a name="oauth2permissionsgrant-property-differences"></a>OAuth2PermissionsGrant プロパティの違い

|Azure AD Graph <br>(v 1.6) プロパティ |Microsoft Graph<br> プロパティ|Comments|
|---|---|---|
| **expiryTime** | ベータ&nbsp;-&nbsp;版**expiryTime** <br> version 1.0&nbsp;-&nbsp;_は&nbsp;まだ&nbsp;利用できません_ | このプロパティは使用されないため、Microsoft Graph では削除される可能性があります。 |
| **startTime** | &nbsp;-β&nbsp;**startTime** <br> version 1.0&nbsp;-&nbsp;_は&nbsp;まだ&nbsp;利用できません_  | このプロパティは使用されないため、Microsoft Graph では削除される可能性があります。 |

## <a name="policy-property-differences"></a>ポリシープロパティの違い

現時点では、Microsoft Graph のポリシーリソース (プレビューでのみ使用可能) は Azure AD Graph によく似ています。  ただし、汎用ポリシーリソースの種類ではなく、名前付きポリシーの種類 (tokenIssuancePolicy、tokenLifetimePolicy など) が存在するように変更されます。

## <a name="serviceendpoint-property-differences"></a>ServiceEndpoint プロパティの違い

Azure AD Graph ServiceEndpoint リソースは、Microsoft Graph のエンドポイントに名前が変更されました。

|Azure AD Graph <br>(v 1.6) プロパティ |Microsoft Graph<br> プロパティ|Comments|
|---|---|---|
| **能力** | &nbsp;-ベータ&nbsp;**機能**<br> v 1.0-_まだ使用できません_ | |
| **serviceId** | &nbsp;-ベータ&nbsp;**providerId**<br> v 1.0-_まだ使用できません_ | |
| **serviceName** | &nbsp;-β&nbsp;**providerName**<br> v 1.0-_まだ使用できません_ | |
| **resourceId** | &nbsp;-ベータ&nbsp;**providerresourceid**<br> v 1.0-_まだ使用できません_ | |
| **uri** | ベータ&nbsp;-&nbsp;版**uri**<br> v 1.0-_まだ使用できません_ | |

## <a name="serviceprincipal-property-differences"></a>ServicePrincipal プロパティの違い

|Azure AD Graph <br>(v 1.6) プロパティ |Microsoft Graph<br> プロパティ|Comments|
|---|---|---|
| **applicationTemplateId** | ベータ版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | |
| **appOwnerTenantId** | ベータ&nbsp;-&nbsp;版**appOwnerOrganizationId** <br> v 1.0-_まだ使用できません_ | |
| **Information Alurl**| ベータ&nbsp;-&nbsp;版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | |
| **preferredSingleSignOnMode** | ベータ&nbsp;-&nbsp;版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | |
| **preferredTokenSigningKeyEndDateTime** | ベータ&nbsp;-&nbsp;版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | |
| **samlSingleSignOnSettings** | ベータ&nbsp;-&nbsp;版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | |
| **servicePrincipalType** | ベータ&nbsp;-&nbsp;版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | |
| **signInAudience** | ベータ&nbsp;-&nbsp;版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | |
| **tokenEncryptionKeyId Id** | ベータ&nbsp;-&nbsp;版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | |
| **serviceEndpoints** | ベータ&nbsp;-&nbsp;版_はまだ利用できません_ <br> v 1.0-_まだ使用できません_ | |

## <a name="tenantdetails-property-differences"></a>TenantDetails プロパティの違い

Azure AD Graph TenantDetails リソースは、Microsoft Graph の組織に名前が変更されました。  プロパティの相違点は次のとおりです。

|Azure AD Graph <br>(v 1.6) プロパティ |Microsoft Graph<br> プロパティ|Comments|
|---|---|---|
| **companyLastDirSyncTime** | ベータ&nbsp;-&nbsp;版**onPremisesLastSyncDateTime** <br>v 1.0- **onPremisesLastSyncDateTime** |  |
| **dirSyncEnabled** | ベータ&nbsp;-&nbsp;版**onPremisesSyncEnabled** <br> v 1.0- **onPremisesSyncEnabled** |  |
| **Soningerrors をプロビジョニングする** | ベータ&nbsp;-&nbsp;_版&nbsp;は&nbsp;まだ利用できません_<br> v 1.0-_まだ使用できません_ | |
| **電話番号** | ベータ&nbsp;-&nbsp;版**businessPhones** <br> v 1.0- **businessPhones** |  |

## <a name="trustedcasforpasswordlessauth-property-differences"></a>Trustedcasforpasswordauthentication プロパティの違い

Azure AD Graph Trustedcasforpasswordを含む Auth リソースは、Microsoft Graph の Certificateベース Authconfiguration に変更されました。  プロパティの違いはありません。

## <a name="next-steps"></a>次のステップ

- Azure AD Graph と Microsoft Graph の[方法の違い](migrate-azure-ad-graph-method-differences.md)について説明します。
- [Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。
- [Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。
