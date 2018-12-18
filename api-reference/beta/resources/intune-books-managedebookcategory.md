---
title: managedEBookCategory リソースの種類
description: Intune eBook の分類項目を 1 つのプロパティが含まれています。
author: tfitzmac
ms.openlocfilehash: 5bc95696a9949fa4be2f58d39a18adf4875a9056
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356918"
---
# <a name="managedebookcategory-resource-type"></a>managedEBookCategory リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Intune eBook の分類項目を 1 つのプロパティが含まれています。
## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト managedEBookCategories](../api/intune-books-managedebookcategory-list.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)コレクション|[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティと関係を一覧表示します。|
|[ManagedEBookCategory を取得します。](../api/intune-books-managedebookcategory-get.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティと関係を参照してください。|
|[ManagedEBookCategory を作成します。](../api/intune-books-managedebookcategory-create.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|新しい[managedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトを作成します。|
|[ManagedEBookCategory を削除します。](../api/intune-books-managedebookcategory-delete.md)|なし|の[managedEBookCategory](../resources/intune-books-managedebookcategory.md)を削除します。|
|[ManagedEBookCategory を更新します。](../api/intune-books-managedebookcategory-update.md)|[managedEBookCategory](../resources/intune-books-managedebookcategory.md)|[ManagedEBookCategory](../resources/intune-books-managedebookcategory.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|エンティティのキー。|
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





