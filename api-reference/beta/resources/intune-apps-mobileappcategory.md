---
title: mobileAppCategory リソースの種類
description: Intune のアプリの単一カテゴリのプロパティが含まれています。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b5cc3d55a717691fc3162bf0ca6f0a633b0e5a95
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327529"
---
# <a name="mobileappcategory-resource-type"></a>mobileAppCategory リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Intune のアプリの単一カテゴリのプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[mobileAppCategories のリスト](../api/intune-apps-mobileappcategory-list.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティとリレーションシップをリストします。|
|[mobileAppCategory の取得](../api/intune-apps-mobileappcategory-get.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティとリレーションシップを読み取ります。|
|[mobileAppCategory の作成](../api/intune-apps-mobileappcategory-create.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|新しい [mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトを作成します。|
|[mobileAppCategory の削除](../api/intune-apps-mobileappcategory-delete.md)|なし|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) を削除します。|
|[mobileAppCategory の更新](../api/intune-apps-mobileappcategory-update.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md)|[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|エンティティのキー。|
|displayName|String|アプリのカテゴリの名前。|
|lastModifiedDateTime|DateTimeOffset|mobileAppCategory が最後に変更された日時です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileAppCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```



