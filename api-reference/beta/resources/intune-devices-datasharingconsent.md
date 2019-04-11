---
title: dataSharingConsent リソースの種類
description: データ共有の同意情報。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e1cb144957ee000a4e077f0f9c58065fad3a8dc
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31780197"
---
# <a name="datasharingconsent-resource-type"></a>dataSharingConsent リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

データ共有の同意情報。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト dataSharingConsents](../api/intune-devices-datasharingconsent-list.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)コレクション|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[dataSharingConsent を取得する](../api/intune-devices-datasharingconsent-get.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[dataSharingConsent を作成する](../api/intune-devices-datasharingconsent-create.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|新しい[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトを作成します。|
|[dataSharingConsent の削除](../api/intune-devices-datasharingconsent-delete.md)|なし|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)を削除します。|
|[dataSharingConsent の更新](../api/intune-devices-datasharingconsent-update.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティを更新します。|
|[consentToDataSharing アクション](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|データ共有の同意 Id|
|servicedisplayname|文字列|サービスワークフローの表示名|
|termsUrl|文字列|データ共有の同意の TermsUrl|
|granted|Boolean|データ共有の同意の付与された状態|
|grantDateTime|DateTimeOffset|このアカウントに対して同意が与えられた時間|
|grantedByUpn|文字列|このアカウントに同意を付与したユーザーの Upn|
|grantedByUserId|文字列|このアカウントに同意を付与したユーザーの UserId|

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





