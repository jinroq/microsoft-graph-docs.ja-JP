---
title: settingvalue リソースの種類
description: 名前と値のペアで表される設定。
localization_priority: Normal
ms.openlocfilehash: dd2cb58c63ff560850bde285a17a06da2399711f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343176"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="9ff40-103">settingvalue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9ff40-103">settingValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ff40-104">名前と値のペアで表される設定。</span><span class="sxs-lookup"><span data-stu-id="9ff40-104">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="9ff40-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ff40-105">Properties</span></span>
| <span data-ttu-id="9ff40-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ff40-106">Property</span></span>     | <span data-ttu-id="9ff40-107">型</span><span class="sxs-lookup"><span data-stu-id="9ff40-107">Type</span></span>   |<span data-ttu-id="9ff40-108">説明</span><span class="sxs-lookup"><span data-stu-id="9ff40-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ff40-109">name</span><span class="sxs-lookup"><span data-stu-id="9ff40-109">name</span></span>|<span data-ttu-id="9ff40-110">string</span><span class="sxs-lookup"><span data-stu-id="9ff40-110">string</span></span>|<span data-ttu-id="9ff40-111">設定の名前 (directorysettingtemplate で定義されている)。</span><span class="sxs-lookup"><span data-stu-id="9ff40-111">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="9ff40-112">value</span><span class="sxs-lookup"><span data-stu-id="9ff40-112">value</span></span>|<span data-ttu-id="9ff40-113">string</span><span class="sxs-lookup"><span data-stu-id="9ff40-113">string</span></span>|<span data-ttu-id="9ff40-114">設定の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ff40-114">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9ff40-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9ff40-115">JSON representation</span></span>

<span data-ttu-id="9ff40-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9ff40-116">Here is a JSON representation of the resource.</span></span>

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
