---
title: managedEBookCategory リソースの種類
description: Intune eBook の分類項目を 1 つのプロパティが含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df057c3aa05d181365397d150aeae93754b63dad
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415335"
---
# <a name="managedebookcategory-resource-type"></a>managedEBookCategory リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Intune eBook の分類項目を 1 つのプロパティが含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト managedEBookCategories](../api/intune-books-managedebookcategory-list.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)コレクション|[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティと関係を一覧表示します。|
|[ManagedEBookCategory を取得します。](../api/intune-books-managedebookcategory-get.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティと関係を参照してください。|
|[ManagedEBookCategory を作成します。](../api/intune-books-managedebookcategory-create.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|新しい[managedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトを作成します。|
|[ManagedEBookCategory を削除します。](../api/intune-books-managedebookcategory-delete.md)|なし|の[managedEBookCategory](../resources/intune-books-managedebookcategory.md)を削除します。|
|[ManagedEBookCategory を更新します。](../api/intune-books-managedebookcategory-update.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|String|エンティティのキー。|
|displayName|String|EBook カテゴリの名前です。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、ManagedEBookCategory が最後に修正されました。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedEBookCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "lastModifiedDateTime": "String (timestamp)"
}
```




