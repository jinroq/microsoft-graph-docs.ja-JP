---
title: デバイス リソース型
description: 組織に登録されているデバイスを表します。 デバイスは、Device Registration Service を使用するか、Intune によってクラウドで作成されます。 これは、多要素認証の条件付きアクセス ポリシーで使用されます。 該当するデバイスの範囲は、デスクトップやノート PC から携帯電話やタブレットに及びます。 directoryObject から継承します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e72777691f0c599067c885168c0c58bb49cec3cb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574611"
---
# <a name="device-resource-type"></a>デバイス リソース型

組織に登録されているデバイスを表します。 デバイスは、Device Registration Service を使用するか、Intune によってクラウドで作成されます。 これは、多要素認証の条件付きアクセス ポリシーで使用されます。 該当するデバイスの範囲は、デスクトップやノート PC から携帯電話やタブレットに及びます。 [directoryObject](directoryobject.md) から継承します。

このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。


## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[デバイスを取得する](../api/device-get.md) | [device](device.md) |デバイス オブジェクトのプロパティとリレーションシップを読み取ります。|
|[デバイスを一覧表示する](../api/device-list.md) | [device](device.md) コレクション| ディレクトリに登録されたデバイスの一覧を取得します。 |
|[デバイスを更新する](../api/device-update.md) | [device](device.md) |デバイス オブジェクトのプロパティを更新します。 |
|[デバイスを削除する](../api/device-delete.md) | なし |デバイス オブジェクトを削除します。 |
|[List memberOf](../api/device-list-memberof.md) |[directoryObject](directoryobject.md) コレクション| デバイスが直接メンバーであるグループを一覧表示します。 |
|[registeredOwners を一覧表示する](../api/device-list-registeredowners.md) |[directoryObject](directoryobject.md) コレクション| registeredOwners ナビゲーション プロパティから、デバイスの登録済み所有者であるユーザーを取得します。|
|[registeredUsers を一覧表示する](../api/device-list-registeredusers.md) |[directoryObject](directoryobject.md) コレクション| registeredUsers ナビゲーション プロパティから、デバイスの登録済みユーザーを取得します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|accountEnabled|ブール型| アカウントが有効な場合は **true**。それ以外の場合は **false**。必須。|
|alternativeSecurityIds|alternativeSecurityId コレクション| 内部使用専用です。 null 許容ではありません。 |
|approximateLastSignInDateTime|DateTimeOffset| timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。 |
|complianceExpirationDateTime|DateTimeOffset| デバイスが準拠していると見なされなくなったときのタイムスタンプ。 timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。 |
|deviceId|string| 登録時に Azure の Device Registration Service により設定された一意の識別子。 |
|deviceMetadata|String| 内部使用専用です。 Null に設定します。 |
|deviceVersion|Int32| 内部使用専用です。 |
|displayName|String|デバイスの表示名。必須。 |
|id|String|デバイスの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用。|
|isCompliant|ブール値|デバイスがモバイル デバイス管理 (MDM) ポリシーに準拠している場合は **true**。それ以外の場合は **false**。 読み取り専用。 これは、任意のデバイスの OS タイプに対して、または Windows OS デバイス用の承認された[MDM アプリ](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)によってのみ、Intune によって更新できます。|
|isManaged|Boolean|デバイスがモバイル デバイス管理 (MDM) アプリで管理されている場合は **true**。それ以外の場合は **false**。 これは、任意のデバイスの OS タイプに対して、または Windows OS デバイス用の承認された[MDM アプリ](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)によってのみ、Intune によって更新できます。 |
|onPremisesLastSyncDateTime|DateTimeOffset|オブジェクトがオンプレミスのディレクトリと最後に同期された日時を示します。Timestamp 型は、ISO 8601 形式を使用して、常に UTC 時間での日付と時刻の情報を表します。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用。|
|onPremisesSyncEnabled|Boolean|このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。 読み取り専用。 |
|operatingSystem|String| デバイス上のオペレーティング システムの種類。必須。 |
|operatingSystemVersion|文字列|デバイス上のオペレーティング システムのバージョン。必須。 |
|physicalIds|String collection| 内部使用専用です。 null 許容ではありません。 |
|profiletype|String|デバイスのプロファイルの種類。 可能な値:<br />**registereddevice**限り<br />**securevm**<br />**Printer**<br />**Shared**<br />**hub**|
|systemlabels|String collection| システムによってデバイスに適用されるラベルのリスト。 |
|trustType|String| 参加済みデバイスの信頼の種類。 読み取り専用です。 可能な値: <br />**ワークプレース** - *bring your own personal devices* を示します<br />**AzureAd** - クラウド専用の参加済みデバイス<br />**ServerAd** -Azure AD に参加済みのオンプレミスのドメイン参加済みデバイス。 詳細については、「[Azure Active Directory のデバイス管理の概要](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction)」を参照してください |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|extensions|[extension](extension.md) コレクション|デバイスに対して定義されているオープン拡張機能のコレクション。読み取り専用です。Null 許容型。|
|memberOf|[directoryObject](directoryobject.md) コレクション|このグループがメンバーとして含まれているグループ。HTTP メソッド:GET (すべてのグループでサポートされます)。読み取り専用です。Null 許容型。|
|[推移的な memberOf を一覧表示する](../api/device-list-transitivememberof.md) |[directoryObject](directoryobject.md) コレクション| デバイスがメンバーであるグループを一覧表示します。 この操作は推移的です。 |
|registeredOwners|[directoryObject](directoryobject.md) コレクション|デバイスがクラウドに参加済みか、または個人用デバイスが登録済みのユーザー。 登録済み所有者は、登録時に設定されます。 現在、所有者は 1 人しかいることができません。 読み取り専用。 Null 許容型。 |
|registeredUsers|[directoryObject](directoryobject.md) コレクション|デバイスの登録済みユーザーのコレクション。 クラウドに参加済みのデバイスと登録済みの個人用デバイスの場合、登録済みのユーザーは、登録時に登録済み所有者と同じ値に設定されます。 読み取り専用。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [
    "extensions",
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
  "alternativeSecurityIds": [{"@odata.type": "microsoft.graph.alternativeSecurityId"}],
  "approximateLastSignInDateTime": "String (timestamp)",
  "complianceExpirationDateTime": "String (timestamp)",
  "deviceId": "string",
  "deviceMetadata": "string",
  "deviceVersion": 1024,
  "displayName": "string",
  "id": "string (identifier)",
  "isCompliant": true,
  "isManaged": true,
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesSyncEnabled": true,
  "operatingSystem": "string",
  "operatingSystemVersion": "string",
  "physicalIds": ["string"],
  "profileType": "string",
  "systemLabels": ["string"],
  "trustType": "string"
}
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
