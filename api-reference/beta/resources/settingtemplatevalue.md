---
title: settingTemplateValue リソースの種類
description: 設定がインスタンス化されていない場合に、設定の既定値を含む、個々のテンプレート設定の定義を表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9a49dd291bd9cc7baa31d90ba8e247ac984b1906
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965188"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="cbb6a-103">settingTemplateValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cbb6a-103">settingTemplateValue resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbb6a-104">設定がインスタンス化されていない場合に、設定の既定値を含む、個々のテンプレート設定の定義を表します。</span><span class="sxs-lookup"><span data-stu-id="cbb6a-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="cbb6a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbb6a-105">Properties</span></span>
| <span data-ttu-id="cbb6a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cbb6a-106">Property</span></span>     | <span data-ttu-id="cbb6a-107">型</span><span class="sxs-lookup"><span data-stu-id="cbb6a-107">Type</span></span>   |<span data-ttu-id="cbb6a-108">説明</span><span class="sxs-lookup"><span data-stu-id="cbb6a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbb6a-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="cbb6a-109">defaultValue</span></span>|<span data-ttu-id="cbb6a-110">string</span><span class="sxs-lookup"><span data-stu-id="cbb6a-110">string</span></span>|<span data-ttu-id="cbb6a-111">設定の既定値。</span><span class="sxs-lookup"><span data-stu-id="cbb6a-111">Default value for the setting.</span></span> <span data-ttu-id="cbb6a-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cbb6a-112">Read-only.</span></span>|
|<span data-ttu-id="cbb6a-113">説明</span><span class="sxs-lookup"><span data-stu-id="cbb6a-113">description</span></span>|<span data-ttu-id="cbb6a-114">string</span><span class="sxs-lookup"><span data-stu-id="cbb6a-114">string</span></span>|<span data-ttu-id="cbb6a-115">設定の説明。</span><span class="sxs-lookup"><span data-stu-id="cbb6a-115">Description of the setting.</span></span> <span data-ttu-id="cbb6a-116">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="cbb6a-116">Read-only.</span></span>|
|<span data-ttu-id="cbb6a-117">name</span><span class="sxs-lookup"><span data-stu-id="cbb6a-117">name</span></span>|<span data-ttu-id="cbb6a-118">string</span><span class="sxs-lookup"><span data-stu-id="cbb6a-118">string</span></span>|<span data-ttu-id="cbb6a-119">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="cbb6a-119">Name of the setting.</span></span> <span data-ttu-id="cbb6a-120">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="cbb6a-120">Read-only.</span></span>|
|<span data-ttu-id="cbb6a-121">type</span><span class="sxs-lookup"><span data-stu-id="cbb6a-121">type</span></span>|<span data-ttu-id="cbb6a-122">string</span><span class="sxs-lookup"><span data-stu-id="cbb6a-122">string</span></span>|<span data-ttu-id="cbb6a-123">設定の種類。</span><span class="sxs-lookup"><span data-stu-id="cbb6a-123">Type of the setting.</span></span> <span data-ttu-id="cbb6a-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cbb6a-124">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cbb6a-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cbb6a-125">JSON representation</span></span>

<span data-ttu-id="cbb6a-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cbb6a-126">Here is a JSON representation of the resource.</span></span>

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
