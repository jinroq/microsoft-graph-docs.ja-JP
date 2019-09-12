---
title: デバイス リソース型
description: ディレクトリに登録されているデバイスを表します。 デバイスは、Device Registration Service を使用するか、Intune によってクラウドで作成されます。 これは、多要素認証の条件付きアクセス ポリシーで使用されます。 該当するデバイスの範囲は、デスクトップやノート PC から携帯電話やタブレットに及びます。 directoryObject から継承します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: a13c39b5d38abb3f44b0fb51ef7a5702ece74b25
ms.sourcegitcommit: 4ce5060cddfa92cc282321bd9cfbf0a39de51aae
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/12/2019
ms.locfileid: "36853827"
---
# <a name="device-resource-type"></a>デバイス リソース型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ディレクトリに登録されているデバイスを表します。 デバイスは、Device Registration Service を使用するか、Intune によってクラウドで作成されます。 これは、多要素認証の条件付きアクセス ポリシーで使用されます。 該当するデバイスの範囲は、デスクトップやノート PC から携帯電話やタブレットに及びます。 [directoryObject](directoryobject.md) から継承します。

このリソースでは、[拡張機能](/graph/extensibility-overview)を使用してカスタム プロパティに独自のデータを追加することができます。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[デバイスを取得する](../api/device-get.md) | [device](device.md) |デバイスオブジェクトのプロパティと関係を読み取ります。|
|[デバイスを一覧表示する](../api/device-list.md) | [device](device.md) コレクション| ディレクトリに登録されたデバイスの一覧を取得します。 |
|[デバイスを更新する](../api/device-update.md) | [device](device.md)  |デバイスオブジェクトのプロパティを更新します。 |
|[デバイスを削除する](../api/device-delete.md) | なし |デバイスオブジェクトを削除します。 |
|[memberOf を一覧表示する](../api/device-list-memberof.md) |[directoryObject](directoryobject.md) collection| デバイスが直接メンバーであるグループを一覧表示します。 |
|[推移的な memberOf を一覧表示する](../api/device-list-transitivememberof.md) |[directoryObject](directoryobject.md) コレクション| デバイスがメンバーであるグループを一覧表示します。 この操作は推移的です。 |
|[registeredOwners を一覧表示する](../api/device-list-registeredowners.md) |[directoryObject](directoryobject.md) collection| registeredOwners ナビゲーション プロパティから、デバイスの登録済み所有者であるユーザーを取得します。|
|[registeredUsers を一覧表示する](../api/device-list-registeredusers.md) |[directoryObject](directoryobject.md) コレクション| registeredUsers ナビゲーション プロパティから、デバイスの登録済みユーザーを取得します。|
|[checkMemberObjects](../api/device-checkmemberobjects.md) | 文字列コレクション | グループ、ディレクトリの役割、または管理単位オブジェクトの一覧のメンバーシップを確認します。 |
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|accountEnabled|Boolean| アカウントが有効な場合は **true**。それ以外の場合は **false**。 既定値は true です。|
|alternativeSecurityIds|alternativeSecurityId コレクション| 内部使用専用です。 null 許容ではありません。 |
|approximateLastSignInDateTime|DateTimeOffset| Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。 |
|complianceExpirationDateTime|DateTimeOffset| デバイスが準拠していると見なされなくなったときのタイムスタンプ。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用です。 |
|deviceId|Guid| 登録時に Azure の Device Registration Service により設定された一意の識別子。 |
|deviceMetadata|String| 内部使用のために用意されています。 Null に設定します。 |
|deviceVersion|Int32| 内部使用のみ。 |
|displayName|String| デバイスの表示名。必須。 |
|id|文字列|デバイスの一意識別子。[directoryObject](directoryobject.md) から継承されます。キーであり、Null は許容されません。読み取り専用。|
|isCompliant|ブール値|デバイスがモバイル デバイス管理 (MDM) ポリシーに準拠している場合は **true**。それ以外の場合は **false**。 読み取り専用です。 これは、任意のデバイスの OS タイプに対して、または Windows OS デバイス用の承認された[MDM アプリ](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)によってのみ、Intune によって更新できます。|
|isManaged|Boolean|デバイスがモバイル デバイス管理 (MDM) アプリで管理されている場合は **true**。それ以外の場合は **false**。 これは、任意のデバイスの OS タイプに対して、または Windows OS デバイス用の承認された[MDM アプリ](https://docs.microsoft.com/windows/client-management/mdm/azure-active-directory-integration-with-mdm)によってのみ、Intune によって更新できます。 |
|onPremisesLastSyncDateTime|DateTimeOffset|オブジェクトがオンプレミスのディレクトリと最後に同期された日時を示します。Timestamp 型は、ISO 8601 形式を使用して、常に UTC 時間での日付と時刻の情報を表します。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'` 読み取り専用。 |
|onPremisesSyncEnabled|Boolean|このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。 読み取り専用です。|
|operatingSystem|String| デバイス上のオペレーティング システムの種類。必須。 |
|operatingSystemVersion|String| デバイスのオペレーティング システムのバージョン。 必須。 |
|physicalIds|String collection| 内部使用専用です。 null 許容ではありません。 |
|profileType|String|デバイスのプロファイルの種類。 可能な値:<br />**Registereddevice**限り<br />**SecureVM**<br />**Printer**<br />**Shared**<br />**Hub**|
|systemLabels|文字列コレクション| システムによってデバイスに適用されるラベルのリスト。 |
|trustType|String| 参加済みデバイスの信頼の種類。 読み取り専用です。 可能な値: <br />**ワークプレース** - *bring your own personal devices* を示します<br />**AzureAd** - クラウド専用の参加済みデバイス<br />**ServerAd** -Azure AD に参加済みのオンプレミスのドメイン参加済みデバイス。 詳細については、「[Azure Active Directory のデバイス管理の概要](https://docs.microsoft.com/en-us/azure/active-directory/device-management-introduction)」を参照してください |
|名前| String | デバイスのフレンドリ名。 ユーザーが Microsoft アカウントでプロジェクトローマの一部としてサインインした場合にのみ返されます。 |
|状態 | String| デバイスがオンラインまたはオフライン。 ユーザーが Microsoft アカウントでプロジェクトローマの一部としてサインインした場合にのみ返されます。 |
|プラットフォーム |String|デバイスのプラットフォーム。 ユーザーが Microsoft アカウントでプロジェクトローマの一部としてサインインした場合にのみ返されます。 ユーザーが Microsoft アカウントでプロジェクトローマの一部としてサインインした場合にのみ返されます。|
|Kind| 文字列| デバイスのフォームファクター。 ユーザーが Microsoft アカウントでプロジェクトローマの一部としてサインインした場合にのみ返されます。 |
|モデル| String| デバイスのモデル。 ユーザーが Microsoft アカウントでプロジェクトローマの一部としてサインインした場合にのみ返されます。 |
|製造| String| デバイスの製造元。 ユーザーが Microsoft アカウントでプロジェクトローマの一部としてサインインした場合にのみ返されます。 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|extensions|[extension](extension.md) コレクション|デバイスに対して定義されているオープン拡張機能のコレクション。読み取り専用です。Null 許容型。|
|registeredOwners|[directoryObject](directoryobject.md) collection| デバイスがクラウドに参加済みか、または個人用デバイスが登録済みのユーザー。 登録済み所有者は、登録時に設定されます。 現在、所有者は 1 人しかいることができません。 読み取り専用です。 Null 許容型。|
|registeredUsers|[directoryObject](directoryobject.md) コレクション| デバイスの登録済みユーザーのコレクション。 クラウドに参加済みのデバイスと登録済みの個人用デバイスの場合、登録済みのユーザーは、登録時に登録済み所有者と同じ値に設定されます。 読み取り専用です。 Null 許容型。|
|extensions|[extension](extension.md) コレクション|デバイスに対して定義されているオープン拡張機能のコレクション。 Null 許容型。|
|registeredOwners|[directoryObject](directoryobject.md) collection|デバイスの登録済み所有者であるユーザー。読み取り専用。Null 許容型。|
|registeredUsers|[directoryObject](directoryobject.md) コレクション|デバイスの登録済みユーザーであるユーザー。読み取り専用。Null 許容型。|
| コマンド | [command](command.md)コレクション | このデバイスに送信されるコマンドのセット|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "registeredOwners",
    "registeredUsers"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.device"
}-->

```json
{
  "accountEnabled": true,
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
  "trustType": "string",
  "Name": "string",
  "Status": "string",
  "Platform": "string",
  "Kind": "string",
  "Model": "string",
  "Manufacturer": "string"
}
```

## <a name="see-also"></a>関連項目

- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "device resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
