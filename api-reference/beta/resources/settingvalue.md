---
title: settingValue リソースの種類
description: 名前と値のペアで表される設定。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d8e652501f8cd96e3e820e61b4ad9d353b61f3fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008475"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="e28a6-103">settingValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e28a6-103">settingValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e28a6-104">名前と値のペアで表される設定。</span><span class="sxs-lookup"><span data-stu-id="e28a6-104">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="e28a6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e28a6-105">Properties</span></span>
| <span data-ttu-id="e28a6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e28a6-106">Property</span></span>     | <span data-ttu-id="e28a6-107">型</span><span class="sxs-lookup"><span data-stu-id="e28a6-107">Type</span></span>   |<span data-ttu-id="e28a6-108">説明</span><span class="sxs-lookup"><span data-stu-id="e28a6-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e28a6-109">name</span><span class="sxs-lookup"><span data-stu-id="e28a6-109">name</span></span>|<span data-ttu-id="e28a6-110">string</span><span class="sxs-lookup"><span data-stu-id="e28a6-110">string</span></span>|<span data-ttu-id="e28a6-111">設定の名前 (directorySettingTemplate で定義されている)。</span><span class="sxs-lookup"><span data-stu-id="e28a6-111">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="e28a6-112">value</span><span class="sxs-lookup"><span data-stu-id="e28a6-112">value</span></span>|<span data-ttu-id="e28a6-113">string</span><span class="sxs-lookup"><span data-stu-id="e28a6-113">string</span></span>|<span data-ttu-id="e28a6-114">設定の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e28a6-114">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e28a6-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e28a6-115">JSON representation</span></span>

<span data-ttu-id="e28a6-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e28a6-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingValue"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
