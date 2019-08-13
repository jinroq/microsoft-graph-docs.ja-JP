---
title: dataSharingConsent リソースの種類
description: データ共有の同意情報。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0fabb90bebb112ccb2e74b7914f14be08523e0a8
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370243"
---
# <a name="datasharingconsent-resource-type"></a>dataSharingConsent リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

データ共有の同意情報。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト dataSharingConsents](../api/intune-devices-datasharingconsent-list.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)コレクション|[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DataSharingConsent を取得する](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DataSharingConsent を作成する](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|新しい[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトを作成します。|
|[DataSharingConsent の削除](../api/intune-devices-datasharingconsent-delete.md)|None|[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)を削除します。|
|[DataSharingConsent の更新](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティを更新します。|
|[consentToDataSharing アクション](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|データ共有の同意 Id|
|serviceDisplayName|String|サービスワークフローの表示名|
|termsUrl|String|データ共有の同意の TermsUrl|
|granted|Boolean|データ共有の同意の付与された状態|
|grantDateTime|DateTimeOffset|このアカウントに対して同意が与えられた時間|
|grantedByUpn|String|このアカウントに同意を付与したユーザーの Upn|
|grantedByUserId|String|このアカウントに同意を付与したユーザーの UserId|

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



