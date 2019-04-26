---
title: settingtemplatevalue リソースの種類
description: 設定がインスタンス化されていない場合に、設定の既定値を含む、個々のテンプレート設定の定義を表します。
localization_priority: Normal
ms.openlocfilehash: 2277f4b7bb66839164a1b09011d20886baf2bd1f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343186"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="76bfd-103">settingtemplatevalue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="76bfd-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76bfd-104">設定がインスタンス化されていない場合に、設定の既定値を含む、個々のテンプレート設定の定義を表します。</span><span class="sxs-lookup"><span data-stu-id="76bfd-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="76bfd-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76bfd-105">Properties</span></span>
| <span data-ttu-id="76bfd-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76bfd-106">Property</span></span>     | <span data-ttu-id="76bfd-107">型</span><span class="sxs-lookup"><span data-stu-id="76bfd-107">Type</span></span>   |<span data-ttu-id="76bfd-108">説明</span><span class="sxs-lookup"><span data-stu-id="76bfd-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="76bfd-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="76bfd-109">defaultValue</span></span>|<span data-ttu-id="76bfd-110">string</span><span class="sxs-lookup"><span data-stu-id="76bfd-110">string</span></span>|<span data-ttu-id="76bfd-111">設定の既定値。</span><span class="sxs-lookup"><span data-stu-id="76bfd-111">Default value for the setting.</span></span> <span data-ttu-id="76bfd-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="76bfd-112">Read-only.</span></span>|
|<span data-ttu-id="76bfd-113">説明</span><span class="sxs-lookup"><span data-stu-id="76bfd-113">description</span></span>|<span data-ttu-id="76bfd-114">string</span><span class="sxs-lookup"><span data-stu-id="76bfd-114">string</span></span>|<span data-ttu-id="76bfd-115">設定の説明。</span><span class="sxs-lookup"><span data-stu-id="76bfd-115">Description of the setting.</span></span> <span data-ttu-id="76bfd-116">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="76bfd-116">Read-only.</span></span>|
|<span data-ttu-id="76bfd-117">name</span><span class="sxs-lookup"><span data-stu-id="76bfd-117">name</span></span>|<span data-ttu-id="76bfd-118">string</span><span class="sxs-lookup"><span data-stu-id="76bfd-118">string</span></span>|<span data-ttu-id="76bfd-119">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="76bfd-119">Name of the setting.</span></span> <span data-ttu-id="76bfd-120">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="76bfd-120">Read-only.</span></span>|
|<span data-ttu-id="76bfd-121">type</span><span class="sxs-lookup"><span data-stu-id="76bfd-121">type</span></span>|<span data-ttu-id="76bfd-122">string</span><span class="sxs-lookup"><span data-stu-id="76bfd-122">string</span></span>|<span data-ttu-id="76bfd-123">設定の種類。</span><span class="sxs-lookup"><span data-stu-id="76bfd-123">Type of the setting.</span></span> <span data-ttu-id="76bfd-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="76bfd-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="76bfd-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="76bfd-125">JSON representation</span></span>

<span data-ttu-id="76bfd-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="76bfd-126">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "string",
  "description": "string",
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
