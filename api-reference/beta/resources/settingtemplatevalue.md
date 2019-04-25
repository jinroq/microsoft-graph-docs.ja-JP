---
title: settingtemplatevalue リソースの種類
description: 設定がインスタンス化されていない場合に、設定の既定値を含む、個々のテンプレート設定の定義を表します。
localization_priority: Normal
ms.openlocfilehash: 80b640419eb2084888dcd6887ece54b4fd4bdf3c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32583680"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="2dfe3-103">settingtemplatevalue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2dfe3-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2dfe3-104">設定がインスタンス化されていない場合に、設定の既定値を含む、個々のテンプレート設定の定義を表します。</span><span class="sxs-lookup"><span data-stu-id="2dfe3-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="2dfe3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2dfe3-105">Properties</span></span>
| <span data-ttu-id="2dfe3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2dfe3-106">Property</span></span>     | <span data-ttu-id="2dfe3-107">型</span><span class="sxs-lookup"><span data-stu-id="2dfe3-107">Type</span></span>   |<span data-ttu-id="2dfe3-108">説明</span><span class="sxs-lookup"><span data-stu-id="2dfe3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2dfe3-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="2dfe3-109">defaultValue</span></span>|<span data-ttu-id="2dfe3-110">string</span><span class="sxs-lookup"><span data-stu-id="2dfe3-110">string</span></span>|<span data-ttu-id="2dfe3-111">設定の既定値。</span><span class="sxs-lookup"><span data-stu-id="2dfe3-111">Default value for the setting.</span></span> <span data-ttu-id="2dfe3-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2dfe3-112">Read-only.</span></span>|
|<span data-ttu-id="2dfe3-113">説明</span><span class="sxs-lookup"><span data-stu-id="2dfe3-113">description</span></span>|<span data-ttu-id="2dfe3-114">string</span><span class="sxs-lookup"><span data-stu-id="2dfe3-114">string</span></span>|<span data-ttu-id="2dfe3-115">設定の説明。</span><span class="sxs-lookup"><span data-stu-id="2dfe3-115">Description of the setting.</span></span> <span data-ttu-id="2dfe3-116">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="2dfe3-116">Read-only.</span></span>|
|<span data-ttu-id="2dfe3-117">name</span><span class="sxs-lookup"><span data-stu-id="2dfe3-117">name</span></span>|<span data-ttu-id="2dfe3-118">string</span><span class="sxs-lookup"><span data-stu-id="2dfe3-118">string</span></span>|<span data-ttu-id="2dfe3-119">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="2dfe3-119">Name of the setting.</span></span> <span data-ttu-id="2dfe3-120">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="2dfe3-120">Read-only.</span></span>|
|<span data-ttu-id="2dfe3-121">type</span><span class="sxs-lookup"><span data-stu-id="2dfe3-121">type</span></span>|<span data-ttu-id="2dfe3-122">string</span><span class="sxs-lookup"><span data-stu-id="2dfe3-122">string</span></span>|<span data-ttu-id="2dfe3-123">設定の種類。</span><span class="sxs-lookup"><span data-stu-id="2dfe3-123">Type of the setting.</span></span> <span data-ttu-id="2dfe3-124">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="2dfe3-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2dfe3-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2dfe3-125">JSON representation</span></span>

<span data-ttu-id="2dfe3-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2dfe3-126">Here is a JSON representation of the resource.</span></span>

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
