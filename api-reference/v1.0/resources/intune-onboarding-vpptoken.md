---
title: vppToken リソースの種類
description: ビジネス向けまたは教育向けの Apple Volume Purchase Program で iOS アプリのライセンスを複数購入した場合、 Apple の Web サイトから Apple VPP アカウントを設定し、Intune にビジネス向けまたは教育向けの Apple VPP トークンをアップロードする必要があります。 これにより、ボリューム購入情報を Intune と同期して、ボリューム購入したアプリの使用状況を追跡できます。 ビジネス向けまたは教育向けの Apple VPP トークンは複数アップロードできます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1e49c075b23ead38b4893c38283521d550428e2c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27973455"
---
# <a name="vpptoken-resource-type"></a>vppToken リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

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

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|ID|String|appleVolumePurchaseProgramToken 作成時に自動的に生成されます。 エンティティのキーになります。|
|organizationName|String|Apple Volume Purchase Program のトークンに関連付けられている組織|
|vppTokenAccountType|[vppTokenAccountType](../resources/intune-shared-vpptokenaccounttype.md)|特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類。 可能な値は、`business`、`education` です。 可能な値は、`business`、`education` です。|
|appleId|String|特定の Apple Volume Purchase Program のトークンに関連付けられている Apple ID。|
|expirationDateTime|DateTimeOffset|Apple Volume Purchase Program のトークンの有効期限。|
|lastSyncDateTime|DateTimeOffset|Apple Volume Purchase Program のトークンを使用して、Apple ボリューム購入プログラム サービスと最後にアプリケーションの同期を行った日時。|
|token|String|Apple Volume Purchase Program からダウンロードした Apple ボリューム購入プログラムのトークン文字列。|
|lastModifiedDateTime|DateTimeOffset|Apple Volume Purchase Program のトークンに関連付けられている最終変更日時。|
|state|[vppTokenState](../resources/intune-onboarding-vpptokenstate.md)|Apple Volume Purchase Program のトークンの現在の状態。 可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。 可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。|
|lastSyncStatus|[vppTokenSyncStatus](../resources/intune-onboarding-vpptokensyncstatus.md)|Apple Volume Purchase Program のトークンを使用して行われた最後のアプリケーションの同期の現在の同期状態。 可能な値は、`none`、`inProgress`、`completed`、`failed` です。 可能な値は、`none`、`inProgress`、`completed`、`failed` です。|
|automaticallyUpdateApps|ブール型|VPP トークンのアプリを自動で更新するかどうか。|
|countryOrRegion|String|VPP トークンのアプリを自動で更新するかどうか。|

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
  "lastSyncStatus": "String",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "String"
}
```



