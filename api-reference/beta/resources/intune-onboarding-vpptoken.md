---
title: vppToken リソースの種類
description: ビジネス向けまたは教育向けの Apple Volume Purchase Program で iOS アプリのライセンスを複数購入した場合、 Apple の Web サイトから Apple VPP アカウントを設定し、Intune にビジネス向けまたは教育向けの Apple VPP トークンをアップロードする必要があります。 これにより、ボリューム購入情報を Intune と同期して、ボリューム購入したアプリの使用状況を追跡できます。 ビジネス向けまたは教育向けの Apple VPP トークンは複数アップロードできます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6f964c2d69da7dbb8407b33e5d9503e9a8ac49e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158451"
---
# <a name="vpptoken-resource-type"></a>vppToken リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ビジネス向けまたは教育向けの Apple Volume Purchase Program で iOS アプリのライセンスを複数購入した場合、 Apple の Web サイトから Apple VPP アカウントを設定し、Intune にビジネス向けまたは教育向けの Apple VPP トークンをアップロードする必要があります。 これにより、ボリューム購入情報を Intune と同期して、ボリューム購入したアプリの使用状況を追跡できます。 ビジネス向けまたは教育向けの Apple VPP トークンは複数アップロードできます。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[vppToken のリスト](../api/intune-onboarding-vpptoken-list.md)|[vppToken](../resources/intune-onboarding-vpptoken.md) コレクション|[vppToken](../resources/intune-onboarding-vpptoken.md) オブジェクトのプロパティとリレーションシップのリストを作成します。|
|[vppToken の取得](../api/intune-onboarding-vpptoken-get.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|[vppToken](../resources/intune-onboarding-vpptoken.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[vppToken の作成](../api/intune-onboarding-vpptoken-create.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|新規に[vppToken](../resources/intune-onboarding-vpptoken.md) オブジェクトを作成します。|
|[vppToken の削除](../api/intune-onboarding-vpptoken-delete.md)|なし|[vppToken](../resources/intune-onboarding-vpptoken.md) を削除します。|
|[vppToken の更新](../api/intune-onboarding-vpptoken-update.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|[vppToken](../resources/intune-onboarding-vpptoken.md) オブジェクトのプロパティを更新します。|
|[syncLicenses アクション](../api/intune-onboarding-vpptoken-synclicenses.md)|[vppToken](../resources/intune-onboarding-vpptoken.md)|特定の appleVolumePurchaseProgramToken に関連付けられたライセンスを同期します|
|[revokeLicenses アクション](../api/intune-onboarding-vpptoken-revokelicenses.md)|なし|特定の appleVolumePurchaseProgramToken に関連付けられているライセンスを取り消す|
|[getLicensesForApp 関数](../api/intune-onboarding-vpptoken-getlicensesforapp.md)|[vpptokenlicensesummary](../resources/intune-onboarding-vpptokenlicensesummary.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|appleVolumePurchaseProgramToken 作成時に自動的に生成されます。 エンティティのキーになります。|
|organizationName|String|Apple Volume Purchase Program のトークンに関連付けられている組織|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類。 使用可能な値は、`business`、`education` です。 可能な値は、`business`、`education` です。|
|appleId|String|特定の Apple Volume Purchase Program のトークンに関連付けられている Apple ID。|
|expirationDateTime|DateTimeOffset|Apple Volume Purchase Program のトークンの有効期限。|
|lastSyncDateTime|DateTimeOffset|Apple Volume Purchase Program のトークンを使用して、Apple ボリューム購入プログラム サービスと最後にアプリケーションの同期を行った日時。|
|token|String|Apple Volume Purchase Program からダウンロードした Apple ボリューム購入プログラムのトークン文字列。|
|lastModifiedDateTime|DateTimeOffset|Apple Volume Purchase Program のトークンに関連付けられている最終変更日時。|
|state|[vpptokenstate](../resources/intune-onboarding-vpptokenstate.md)|Apple Volume Purchase Program のトークンの現在の状態。 可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。 可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。|
|tokenactionresults|[vpptokenactionresult](../resources/intune-onboarding-vpptokenactionresult.md)コレクション|Apple volume purchase program トークンで実行されたアクションのステータスのコレクション。|
|lastSyncStatus|[vpptokensyncstatus](../resources/intune-onboarding-vpptokensyncstatus.md)|Apple Volume Purchase Program のトークンを使用して行われた最後のアプリケーションの同期の現在の同期状態。 可能な値は、`none`、`inProgress`、`completed`、`failed` です。 可能な値は、`none`、`inProgress`、`completed`、`failed` です。|
|automaticallyUpdateApps|Boolean|VPP トークンのアプリを自動で更新するかどうか。|
|countryOrRegion|文字列|VPP トークンのアプリを自動で更新するかどうか。|
|dataSharingConsentGranted|ブール値|Apple volume purchase program でのデータ共有に対して付与される同意。|
|displayName|文字列型 (String)|管理者が指定したトークンのフレンドリ名。|
|msrtcsip-locationname|String|Apple VPP から返されるトークンの場所。|
|claimtokenmanagementfromexternalmdm|ブール値|管理者の同意を得て、外部 MDM からのトークン管理を許可します。|
|roleScopeTagIds|String collection|このエンティティに割り当てられているロールスコープタグ id。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.vppToken"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "String (identifier)",
  "organizationName": "String",
  "vppTokenAccountType": "String",
  "appleId": "String",
  "expirationDateTime": "String (timestamp)",
  "lastSyncDateTime": "String (timestamp)",
  "token": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "state": "String",
  "tokenActionResults": [
    {
      "@odata.type": "microsoft.graph.vppTokenActionResult",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ],
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String",
  "dataSharingConsentGranted": true,
  "displayName": "String",
  "locationName": "String",
  "claimTokenManagementFromExternalMdm": true,
  "roleScopeTagIds": [
    "String"
  ]
}
```




