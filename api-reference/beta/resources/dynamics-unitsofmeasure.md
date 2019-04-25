---
title: unitsOfMeasure リソースの種類
description: Dynamics 365 Business Central の測定単位オブジェクト。
services: project-madeira
documentationcenter: ''
author: SusanneWindfeldPedersen
localization_priority: Normal
ms.prod: dynamics-365-business-central
ms.openlocfilehash: 870e188939646594b62e6eebf3e234eb0211f140
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543029"
---
# <a name="unitsofmeasure-resource-type"></a>unitsOfMeasure リソースの種類
Dynamics 365 Business Central の、数量の標準測定基準である測定単位を表します。

## <a name="methods"></a>メソッド

| メソッド       | 戻り値の型  |説明|
|:---------------|:--------|:----------|
|[unitsOfMeasure を取得する](../api/dynamics-unitsofmeasure-get.md)|unitsOfMeasure|測定単位オブジェクトを取得します。|
|[Post unitsOfMeasure](../api/dynamics-create-unitsofmeasure.md)|unitsOfMeasure|測定単位オブジェクトを作成します。|
|[Patch unitsOfMeasure](../api/dynamics-unitsofmeasure-update.md)|unitsOfMeasure|測定単位オブジェクトを更新します。|
|[unitsOfMeasure の削除](../api/dynamics-unitsofmeasure-delete.md)|なし|測定単位オブジェクトを削除します。|

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|id|GUID|unitsOfMeasure の一意の ID。 編集できません。|
|code|string|測定単位のコードを指定します。|
|displayName|string|測定単位の表示名を指定します。|
|internationalStandardCode|string|営業ドキュメントの電子送信に関連して、UNECE Rec20 standard に従って表される測定単位コードの単位を指定します。|
|lastModifiedDateTime|datetime|測定単位が変更された最後の datetime。 読み取り専用。|  


## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記

ここでは、 **unitsOfMeasure**リソースの JSON 表記を示します。

```json
{
  "id": "GUID",
  "code": "string",
  "displayName": "string",
  "internationalStandardCode": "string",
  "lastModifiedDateTime": "datetime"
}

```
