---
author: daspek
ms.author: dspektor
ms.date: 09/12/2017
title: ContentType
ms.openlocfilehash: ee869e5f2925af92fea9eef04fd26ec483baad5b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="contenttype-resource-type"></a>ContentType リソース型

**contentType** リソースは、SharePoint の_コンテンツ タイプ_を表します。
コンテンツ タイプによって、[**list**][list] 内の [**listItem**][listItem] ごとに存在する必要のある列のセットを定義することができます。

[list]: list.md
[listItem]: listItem.md

## <a name="json-representation"></a>JSON 表記

以下は、**contentType** リソースの JSON 表記です。
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.contentType" } -->

```json
{
  "description": "string",
  "group": "string",
  "hidden": false,
  "id": "string",
  "inheritedFrom": { "@type": "microsoft.graph.itemReference" },
  "name": "string",
  "order": { "@type": "microsoft.graph.contentTypeOrder" },
  "parentId": "string",
  "readOnly": false,
  "sealed": false,

  "columnLinks": [{ "@type": "microsoft.graph.columnLink" }]
}
```

## <a name="properties"></a>プロパティ

| プロパティ名     | 種類                 | 説明
|:------------------|:---------------------|:----------------------------------
| **description**   | string               | アイテムの説明テキストです。
| **group**         | string               | このコンテンツ タイプが属するグループの名前。 関連するコンテンツ タイプを整理するのに役立ちます。
| **hidden**        | boolean              | コンテンツ タイプがリストの [新規作成] メニューで非表示かどうかを示します。
| **id**            | string               | コンテンツ タイプの一意識別子。
| **inheritedFrom** | [itemReference][]    | このコンテンツ タイプが、別のスコープ (サイトなど) から継承されている場合、そのコンテンツ タイプが定義されているアイテムへの参照を提供します。
| **name**          | string               | コンテンツ タイプの名前。
| **order**         | [contentTypeOrder][] | 選択 UI でコンテンツ タイプを表示する順番を指定します。
| **parentId**      | string               | コンテンツ タイプの一意識別子。
| **readOnly**      | boolean              | `true` の場合、コンテンツ タイプは変更できません。変更する場合は、この値を先に `false` に設定します。
| **sealed**        | boolean              | `true` の場合、ユーザーまたはプッシュダウン操作ではコンテンツ タイプを変更できません。 サイト コレクションの管理者だけがコンテンツ タイプのシールまたはシール解除ができます。

## <a name="relationships"></a>リレーションシップ

| プロパティ名   | 種類                      | 説明
|:----------------|:--------------------------|:-------------------------------
| **columnLinks** | [columnLink][] コレクション | このコンテンツ タイプに必要とされる列のコレクション

詳細については、「[コンテンツ タイプとコンテンツ タイプ発行の概要][contentTypeIntro]」を参照してください。

[columnLink]: columnLink.md
[contentTypeIntro]: https://support.office.com/en-us/article/Introduction-to-content-types-and-content-type-publishing-e1277a2e-a1e8-4473-9126-91a0647766e5
[itemReference]: itemReference.md
[contentTypeOrder]: contentTypeOrder.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ContentType"
} -->
