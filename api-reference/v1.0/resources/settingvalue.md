---
title: settingValue リソースの種類
description: 名前と値の組で表される設定。
ms.openlocfilehash: b47c5c746117390cfd59db71d832928e482403b9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024285"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="946b2-103">settingValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="946b2-103">settingValue resource type</span></span>

<span data-ttu-id="946b2-104">名前と値の組で表される設定。</span><span class="sxs-lookup"><span data-stu-id="946b2-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="946b2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="946b2-105">Properties</span></span>

| <span data-ttu-id="946b2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="946b2-106">Property</span></span> | <span data-ttu-id="946b2-107">型</span><span class="sxs-lookup"><span data-stu-id="946b2-107">Type</span></span> | <span data-ttu-id="946b2-108">説明</span><span class="sxs-lookup"><span data-stu-id="946b2-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="946b2-109">名前</span><span class="sxs-lookup"><span data-stu-id="946b2-109">name</span></span>|<span data-ttu-id="946b2-110">文字列</span><span class="sxs-lookup"><span data-stu-id="946b2-110">String</span></span>| <span data-ttu-id="946b2-111">設定の名前 ([groupSettingTemplate](groupsettingtemplate.md) によって定義されている)。</span><span class="sxs-lookup"><span data-stu-id="946b2-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="946b2-112">値</span><span class="sxs-lookup"><span data-stu-id="946b2-112">value</span></span>|<span data-ttu-id="946b2-113">文字列</span><span class="sxs-lookup"><span data-stu-id="946b2-113">String</span></span>| <span data-ttu-id="946b2-114">設定の値です。</span><span class="sxs-lookup"><span data-stu-id="946b2-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="946b2-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="946b2-115">JSON representation</span></span>

<span data-ttu-id="946b2-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="946b2-116">Here is a JSON representation of the resource.</span></span>

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