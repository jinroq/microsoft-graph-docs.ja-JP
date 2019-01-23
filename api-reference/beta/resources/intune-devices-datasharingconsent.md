---
title: dataSharingConsent リソースの種類
description: データの共有についてを同意するものとします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bf77a252c323ce83c2dcda44ac294161a4fd4747
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425695"
---
# <a name="datasharingconsent-resource-type"></a>dataSharingConsent リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

データの共有についてを同意するものとします。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト dataSharingConsents](../api/intune-devices-datasharingconsent-list.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)コレクション|[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティと関係を一覧表示します。|
|[DataSharingConsent を取得します。](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティと関係を参照してください。|
|[DataSharingConsent を作成します。](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|新しい[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトを作成します。|
|[DataSharingConsent を削除します。](../api/intune-devices-datasharingconsent-delete.md)|なし|の[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)を削除します。|
|[DataSharingConsent を更新します。](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティを更新します。|
|[consentToDataSharing アクション](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|データ共有同意 Id|
|serviceDisplayName|String|サービス作業の流れの表示名|
|termsUrl|String|同意の共有データの TermsUrl|
|付与|Boolean|同意の共有データに付与されている状態|
|grantDateTime|DateTimeOffset|同意は、このアカウントに与えられました。|
|grantedByUpn|String|このアカウントに許可を付与するユーザーの Upn|
|grantedByUserId|String|このアカウントに許可を付与するユーザーのユーザー Id|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSharingConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "String (identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": true,
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
}
```




