---
title: ドメイン リソースの種類
description: テナントに関連付けられているドメインを表します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d19909679447e050ea639ee0fcb4cd31288efc0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518640"
---
# <a name="domain-resource-type"></a>ドメイン リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナントに関連付けられているドメインを表します。

ドメイン操作を使用して、テナントにドメインを関連付け、ドメインの所有権を確認し、サポートされているサービスを構成します。ドメイン操作によって Office 365 などのサービスのドメインの関連付けを自動化するレジストラーを有効にします。たとえば、ドメインのサインアップの一部として、レジストラーは電子メール、Web サイト、認証などのバニティ ドメインを有効化することができます。

ドメインをテナントに関連付ける方法：

1. ドメインをテナントに[関連付ける](../api/domain-post-domains.md)。

2. ドメインの検証レコードを[取得する](../api/domain-list-verificationdnsrecords.md)。ドメイン レジストラーまたは DNS サーバー構成を使用して、検証レコードの詳細情報をドメインのゾーン ファイルに追加します。

3. ドメインの所有権を[検証する](../api/domain-verify.md)。ドメインを確認し、*isVerified* プロパティを *true* に設定します。

4. ドメインと共に使用する、サポートされているサービスを[指定する](../api/domain-update.md)。

5. ドメイン向けのサービスを有効にするのに必要なレコードの一覧を取得して、サポートされているサービスを[構成する](../api/domain-list-serviceconfigurationrecords.md)。ドメイン レジストラーまたは DNS サーバー構成を使用して、構成レコードの詳細情報をドメインのゾーン ファイルに追加します。

## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型 |説明|
|:---------------|:--------|:----------|
|[Get domain](../api/domain-get.md) | [domain](domain.md) | ドメイン オブジェクトのプロパティとリレーションシップを読み取ります。|
|[Create domain](../api/domain-post-domains.md) | [domain](domain.md) | テナントにドメインを追加します。 |
|[List domainNameReference](../api/domain-list-domainnamereferences.md) |[directoryObject](directoryobject.md) コレクション| ドメインへの参照付きのディレクトリ オブジェクトの一覧を取得します。|
|[List serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md) |[domainDnsRecord](domaindnsrecord.md) collection|  ドメイン構成のためドメインの DNS レコードの一覧を取得します。|
|[List verificationDnsRecords](../api/domain-list-verificationdnsrecords.md) |[domainDnsRecord](domaindnsrecord.md) collection|  ドメイン検証のためドメインの DNS レコードの一覧を取得します。|
|[Update domain](../api/domain-update.md) | [domain](domain.md) |ドメインを更新します|
|[Delete domain](../api/domain-delete.md) | なし |ドメインを削除します。|
|[ForceDelete ドメイン](../api/domain-forcedelete.md)|なし|非同期操作を使用してドメインを削除します。|
|[Verify domain](../api/domain-verify.md)|[domain](domain.md)|ドメインの所有権を検証します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型 | 説明 |
|:---------------|:--------|:----------|
|authenticationType|String| ドメインに対して構成されている認証の種類を示します。値は、*Managed* または *Federated* のいずれかです。<br> *Managed* の場合、Azure AD がユーザー認証を実行するクラウド管理のドメインを表します。<br>*Federated* の場合、Active Directory フェデレーション サービスを経由したテナントのオンプレミスの Active Directory のように、認証が ID プロバイダーとフェデレーションを行うことを表します。null 許容ではありません |
|availabilityStatus|String| [確認](../api/domain-verify.md)操作を使用する場合を除き、このプロパティは常に null です。[確認](../api/domain-verify.md)操作を使用する場合、応答で**ドメイン** エンティティが返されます。応答内の、**ドメイン** エンティティの **availabilityStatus** プロパティは、*AvailableImmediately* または *EmailVerifiedDomainTakeoverScheduled* のいずれかです。|
|id|String| ドメインの完全修飾名です。キー、不変、Null 許容ではない、一意 |
|isAdminManaged|ブール値| ドメインの DNS レコードの管理が Office 365 に委任されている場合、プロパティの値は false です。それ以外の場合、値は true です。null 許容ではありません |
|isDefault|ブール型| ユーザーの作成に使用する既定のドメインの場合は true です。会社ごとに 1 つだけの既定のドメインがあります。null 許容ではありません |
|isInitial|ブール値| Microsoft Online Services (companyname.onmicrosoft.com) によって作成された初期ドメインがある場合は true です。会社ごとに 1 つだけの初期ドメインがあります。null 許容ではありません |
|isRoot|ブール値| ドメインが検証済みのルート ドメインである場合は true です。それ以外に、ドメインがサブドメインまたは未確認である場合は false です。null 許容ではありません |
|isVerified|Boolean| そのドメインが、ドメイン所有権の確認を完了している場合は true です。null 許容ではありません |
|supportedServices|String collection| ドメインに割り当てられている機能です。<br><br>0、1 または次の値を含めることができます。*Email*、*Sharepoint*、*EmailInternalRelayOnly*、*OfficeCommunicationsOnline*、*SharePointDefaultDomain*、*FullRedelegation*、*SharePointPublic*、*OrgIdAuthentication*、*Yammer*、*Intune*<br><br> Graph API を使用して追加または削除できる値は次のとおりです。*Email*、*OfficeCommunicationsOnline*、*Yammer*<br>null 許容ではありません|
|state|[domainState](domainstate.md)| ドメインのためにスケジュールされている非同期操作の状態です。 |

## <a name="relationships"></a>リレーションシップ

検証レコードやサービス構成のレコードなど、ディレクトリ内のドメインと他のオブジェクト間のリレーションシップは、ナビゲーション プロパティを介して公開されます。要求でこれらのナビゲーション プロパティを対象にすれば、そのリレーションシップを読み取ることができます。

| リレーションシップ | 型 |説明|
|:---------------|:--------|:----------|
|domainNameReferences|[directoryObject](directoryobject.md) collection| 読み取り専用、Null 許容型|
|serviceConfigurationRecords|[domainDnsRecord](domaindnsrecord.md) collection| ドメインを Microsoft Online Services で使用する前に、顧客がそのドメインの DNS ゾーン ファイルに追加する DNS レコードです。<br>読み取り専用、Null 許容型 |
|verificationDnsRecords|[domainDnsRecord](domaindnsrecord.md) collection| 顧客が Azure AD のドメイン所有権の確認を完了する前に、顧客がそのドメインの DNS ゾーン ファイルに追加する DNS レコード。<br>読み取り専用、Null 許容型|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domain"
}-->

```json
{
  "authenticationType": "String",
  "availabilityStatus": "String",
  "id": "String (identifier)",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "isVerified": true,
  "state": {"@odata.type": "microsoft.graph.domainState"},
  "supportedServices": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/domain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
