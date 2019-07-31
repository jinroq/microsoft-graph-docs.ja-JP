---
title: ドメインリソースの種類
description: テナントに関連付けられているドメインを表します。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e6390b72a7292a9529c11c6200d4c61dcc5355c1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973824"
---
# <a name="domain-resource-type"></a>ドメインリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

テナントに関連付けられているドメインを表します。

ドメインの操作を使用して、ドメインをテナントに関連付け、ドメインの所有権を確認し、サポートされているサービスを構成します。  ドメイン操作によって Office 365 などのサービスのドメインの関連付けを自動化するレジストラーを有効にします。 たとえば、ドメインのサインアップの一環として、レジストラーは、電子メール、web サイト、認証などのバニティドメインを有効にすることができます。

ドメインをテナントに関連付けるには、次のようにします。

1. ドメインをテナントに[関連付け](../api/domain-post-domains.md)ます。

2. ドメイン検証レコードを[取得](../api/domain-list-verificationdnsrecords.md)します。 ドメインレジストラーまたは DNS サーバー構成を使用して、ドメインのゾーンファイルに検証レコードの詳細を追加します。

3. ドメインの所有権[を確認](../api/domain-verify.md)します。 これにより、ドメインが確認さ** れ、isverified プロパティが*true*に設定されます。

4. ドメインでの使用を計画しているサービスを[示し](../api/domain-update.md)ます。

5. ドメインのサービスを有効にするために必要なレコードの一覧を取得して、サポートされているサービスを[構成](../api/domain-list-serviceconfigurationrecords.md)します。 ドメインレジストラーまたは DNS サーバー構成を使用して、ドメインのゾーンファイルに構成レコードの詳細を追加します。

## <a name="methods"></a>メソッド

| メソッド   | 戻り値の型 |説明|
|:---------------|:--------|:----------|
|[ドメインを取得する](../api/domain-get.md) | [domain](domain.md) | ドメインオブジェクトのプロパティとリレーションシップを読み取ります。|
|[ドメインを作成する](../api/domain-post-domains.md) | [domain](domain.md) | テナントにドメインを追加します。 |
|[リスト domainNameReference](../api/domain-list-domainnamereferences.md) |[directoryObject](directoryobject.md) collection| ドメインへの参照を使用して、ディレクトリオブジェクトの一覧を取得します。|
|[リスト serviceConfigurationRecords](../api/domain-list-serviceconfigurationrecords.md) |[Domaindnsrecord](domaindnsrecord.md)コレクション|  ドメイン構成のドメイン DNS レコードの一覧を取得します。|
|[リスト verificationDnsRecords](../api/domain-list-verificationdnsrecords.md) |[Domaindnsrecord](domaindnsrecord.md)コレクション|  ドメイン検証のドメイン DNS レコードの一覧を取得します。|
|[ドメインを更新する](../api/domain-update.md) | [domain](domain.md) |ドメインを更新します。|
|[ドメインを削除する](../api/domain-delete.md) | None |ドメインを削除します。|
|[ForceDelete ドメイン](../api/domain-forcedelete.md)|None|非同期操作を使用してドメインを削除します。|
|[ドメインを確認する](../api/domain-verify.md)|[domain](domain.md)|ドメインの所有権を検証します。|

## <a name="properties"></a>プロパティ

| プロパティ   | 型 | 説明 |
|:---------------|:--------|:----------|
|authenticationType|String| ドメインに対して構成されている認証の種類を示します。 値は、*管理*されているか、*フェデレーション*されています。<br> *Managed*は、Azure AD がユーザー認証を実行するクラウド管理のドメインを示します。<br>*フェデレーション*は、Active Directory フェデレーションサービスを経由して、テナントの社内 Active directory などの id プロバイダーとの認証がフェデレーションされることを示します。 Null 許容ではない |
|availabilityStatus|String| [Verify](../api/domain-verify.md)アクションが使用される場合を除き、このプロパティは常に null になります。 [Verify](../api/domain-verify.md)アクションを使用すると、応答で**ドメイン**エンティティが返されます。 応答内の**ドメイン**エンティティの**availabilityStatus**プロパティは、*すぐに*、または*EmailVerifiedDomainTakeoverScheduled*でもかまいません。|
|id|String| ドメインの完全修飾名。 キー、不変、null 許容ではない、unique |
|isAdminManaged|Boolean| ドメインの DNS レコード管理が Office 365 に委任されている場合、このプロパティの値は false になります。 それ以外の場合、値は true になります。 Null 許容ではない |
|isDefault|ブール型 (Boolean)| これがユーザーの作成に使用される既定のドメインの場合は True。 会社ごとに既定のドメインが1つだけ存在します。 Null 許容ではない |
|isInitial|ブール値| True は、Microsoft Online Services (companyname.onmicrosoft.com) によって作成された初期ドメインの場合です。 会社ごとに1つの初期ドメインのみが存在します。 Null 許容ではない |
|isRoot|Boolean| ドメインが確認されたルートドメインの場合は True。 それ以外の場合は、ドメインがサブドメインまたは未確認の場合は false。 Null 許容ではない |
|isVerified|Boolean| ドメインの所有権の確認が完了した場合は True。 Null 許容ではない |
|passwordNotificationWindowInDays|Int32|ユーザーがパスワードの有効期限が切れると通知を受信するまでの日数を指定します。 このプロパティが設定されていない場合は、既定値の14日が使用されます。|
|passwordValidityPeriodInDays|Int32| パスワードを変更するまでの有効期間を指定します。 このプロパティが設定されていない場合は、既定値の90日が使用されます。 |
|supportedServices|文字列コレクション| ドメインに割り当てられている機能。<br><br>0、1または次の値を含めることができます。 *Email*、 *Sharepoint*、 *emailinternalrelayonly*、 *OfficeCommunicationsOnline*、 *sharepointdefaultdomain*、 *fullredelegation*、 *sharepointpublic*、*Orgidauthentication*、 *Yammer*、 *Intune*<br><br> Graph API を使用して追加または削除できる値は次のとおりです。 *Email*、 *OfficeCommunicationsOnline*、 *Yammer*<br>Null 許容ではない|
|state|[domainState](domainstate.md)| ドメインに対してスケジュールされた非同期操作の状態。 |

## <a name="relationships"></a>リレーションシップ

確認レコードやサービス構成レコードなど、ディレクトリ内のドメインとその他のオブジェクトとの関係は、ナビゲーションプロパティを通じて公開されます。 これらのリレーションシップは、要求でこれらのナビゲーションプロパティを対象にして確認できます。

| リレーションシップ | 型 |説明|
|:---------------|:--------|:----------|
|domainNameReferences|[directoryObject](directoryobject.md) collection| 読み取り専用、Null 許容|
|serviceConfigurationRecords|[Domaindnsrecord](domaindnsrecord.md)コレクション| DNS レコードユーザーが Microsoft Online services で使用できるようになる前に、ドメインの DNS ゾーンファイルに追加されます。<br>読み取り専用、Null 許容 |
|verificationDnsRecords|[Domaindnsrecord](domaindnsrecord.md)コレクション| お客様が Azure AD を使用してドメインの所有権の確認を完了する前に、お客様がドメインの DNS ゾーンファイルに追加する DNS レコード。<br>読み取り専用、Null 許容|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "keyProperty":"id",
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
  "passwordNotificationWindowInDays": 14,
  "passwordValidityPeriodInDays": 90,
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
  "suppressions": []
}
-->
