---
title: settingValue リソースの種類
description: 名前と値のペアで表される設定。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f37a429fd9bb8e8d3cf65aef55d6af5033f4a598
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034357"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="5c5a8-103">settingValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5c5a8-103">settingValue resource type</span></span>

<span data-ttu-id="5c5a8-104">名前と値のペアで表される設定。</span><span class="sxs-lookup"><span data-stu-id="5c5a8-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="5c5a8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c5a8-105">Properties</span></span>

| <span data-ttu-id="5c5a8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c5a8-106">Property</span></span> | <span data-ttu-id="5c5a8-107">型</span><span class="sxs-lookup"><span data-stu-id="5c5a8-107">Type</span></span> | <span data-ttu-id="5c5a8-108">説明</span><span class="sxs-lookup"><span data-stu-id="5c5a8-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="5c5a8-109">name</span><span class="sxs-lookup"><span data-stu-id="5c5a8-109">name</span></span>|<span data-ttu-id="5c5a8-110">String</span><span class="sxs-lookup"><span data-stu-id="5c5a8-110">String</span></span>| <span data-ttu-id="5c5a8-111">設定の名前 ( [Groupsettingtemplate](groupsettingtemplate.md)で定義)。</span><span class="sxs-lookup"><span data-stu-id="5c5a8-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="5c5a8-112">value</span><span class="sxs-lookup"><span data-stu-id="5c5a8-112">value</span></span>|<span data-ttu-id="5c5a8-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="5c5a8-113">String</span></span>| <span data-ttu-id="5c5a8-114">設定の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5c5a8-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="5c5a8-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c5a8-115">JSON representation</span></span>

<span data-ttu-id="5c5a8-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5c5a8-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
