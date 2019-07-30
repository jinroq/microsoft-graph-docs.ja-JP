---
author: JeremyKelley
ms.author: jeremyke
title: アルバムリソースの種類
description: フォトアルバムであるバンドルを記述するファセット。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3bb5391557c3dfb0a97702a0e78de60c0a4876c7
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932878"
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
