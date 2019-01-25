---
title: settingTemplateValue リソースの種類
description: 設定がインスタンス化されていない場合の、設定の既定値を含む個々のテンプレートの設定定義を表します。
localization_priority: Normal
ms.openlocfilehash: 80b640419eb2084888dcd6887ece54b4fd4bdf3c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528012"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="0dc7d-103">settingTemplateValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0dc7d-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0dc7d-104">設定がインスタンス化されていない場合の、設定の既定値を含む個々のテンプレートの設定定義を表します。</span><span class="sxs-lookup"><span data-stu-id="0dc7d-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="0dc7d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0dc7d-105">Properties</span></span>
| <span data-ttu-id="0dc7d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0dc7d-106">Property</span></span>     | <span data-ttu-id="0dc7d-107">型</span><span class="sxs-lookup"><span data-stu-id="0dc7d-107">Type</span></span>   |<span data-ttu-id="0dc7d-108">説明</span><span class="sxs-lookup"><span data-stu-id="0dc7d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0dc7d-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="0dc7d-109">defaultValue</span></span>|<span data-ttu-id="0dc7d-110">string</span><span class="sxs-lookup"><span data-stu-id="0dc7d-110">string</span></span>|<span data-ttu-id="0dc7d-111">設定の既定値です。</span><span class="sxs-lookup"><span data-stu-id="0dc7d-111">Default value for the setting.</span></span> <span data-ttu-id="0dc7d-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0dc7d-112">Read-only.</span></span>|
|<span data-ttu-id="0dc7d-113">説明</span><span class="sxs-lookup"><span data-stu-id="0dc7d-113">description</span></span>|<span data-ttu-id="0dc7d-114">string</span><span class="sxs-lookup"><span data-stu-id="0dc7d-114">string</span></span>|<span data-ttu-id="0dc7d-115">設定の説明です。</span><span class="sxs-lookup"><span data-stu-id="0dc7d-115">Description of the setting.</span></span> <span data-ttu-id="0dc7d-116">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0dc7d-116">Read-only.</span></span>|
|<span data-ttu-id="0dc7d-117">name</span><span class="sxs-lookup"><span data-stu-id="0dc7d-117">name</span></span>|<span data-ttu-id="0dc7d-118">string</span><span class="sxs-lookup"><span data-stu-id="0dc7d-118">string</span></span>|<span data-ttu-id="0dc7d-119">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="0dc7d-119">Name of the setting.</span></span> <span data-ttu-id="0dc7d-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0dc7d-120">Read-only.</span></span>|
|<span data-ttu-id="0dc7d-121">type</span><span class="sxs-lookup"><span data-stu-id="0dc7d-121">type</span></span>|<span data-ttu-id="0dc7d-122">string</span><span class="sxs-lookup"><span data-stu-id="0dc7d-122">string</span></span>|<span data-ttu-id="0dc7d-123">設定の種類です。</span><span class="sxs-lookup"><span data-stu-id="0dc7d-123">Type of the setting.</span></span> <span data-ttu-id="0dc7d-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0dc7d-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0dc7d-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0dc7d-125">JSON representation</span></span>

<span data-ttu-id="0dc7d-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0dc7d-126">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/settingtemplatevalue.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
