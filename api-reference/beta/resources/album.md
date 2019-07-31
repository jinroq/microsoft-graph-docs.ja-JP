---
author: JeremyKelley
ms.author: jeremyke
title: アルバムリソースの種類
description: フォトアルバムであるバンドルを記述するファセット。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 59717995870cbfe970fd23b160377d32cb722835
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35974452"
---
# <a name="album-resource-type"></a>アルバムリソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

フォトアルバムは、1つの[バンドル][]内で、ハードファセット[][]を使用して、事実上グループ化された[ドライブ][]アイテムをグループ化する方法です。 このタイプのバンドルには、[バンドル][]リソースに**アルバム**プロパティが設定されます。

## <a name="properties"></a>プロパティ

| プロパティ名     | 種類   | 説明
|:------------------|:-------|:------------------------------------------------
| イメージ Itemid のカバー | String | アルバムのカバーである[ドライブ項目][]の一意の識別子。

**注:** カバーされていない**Imageitemid**が前に設定されていない場合は、アルバムのサムネイルが自動的に選択されます。
**イメージ itemid**が設定された後は、アルバムのサムネイルは常にその id に関連付けられているアイテムになります。[バンドルアイテム][バンドル]にパッチを適用し、の`album`カバー **imageitemid**プロパティをアルバム内に含まれる画像の id に設定することで、既定のカバーを上書きできます。
ユーザー設定の表紙を削除するには、カバー **Imageitemid**プロパティを null に設定し、既定値を自動的に選択します。

## <a name="json-representation"></a>JSON 表記

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.album" } -->

```json
{
  "coverImageItemId": "string"
}
```

[バンドル]: bundle.md
[driveItem]: driveItem.md
[photo]: photo.md
