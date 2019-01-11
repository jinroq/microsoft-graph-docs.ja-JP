---
title: settingValue リソースの種類
description: 名前と値の組で表される設定。
localization_priority: Normal
ms.openlocfilehash: 0ddd6388e14ea3deff99e927541694a97c594195
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815527"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="0b6c9-103">settingValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0b6c9-103">settingValue resource type</span></span>

> <span data-ttu-id="0b6c9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0b6c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b6c9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b6c9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0b6c9-106">名前と値の組で表される設定。</span><span class="sxs-lookup"><span data-stu-id="0b6c9-106">A setting represented by a name/value pair.</span></span>


## <a name="properties"></a><span data-ttu-id="0b6c9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b6c9-107">Properties</span></span>
| <span data-ttu-id="0b6c9-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b6c9-108">Property</span></span>     | <span data-ttu-id="0b6c9-109">種類</span><span class="sxs-lookup"><span data-stu-id="0b6c9-109">Type</span></span>   |<span data-ttu-id="0b6c9-110">説明</span><span class="sxs-lookup"><span data-stu-id="0b6c9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b6c9-111">name</span><span class="sxs-lookup"><span data-stu-id="0b6c9-111">name</span></span>|<span data-ttu-id="0b6c9-112">文字列</span><span class="sxs-lookup"><span data-stu-id="0b6c9-112">string</span></span>|<span data-ttu-id="0b6c9-113">設定で定義された、directorySettingTemplate) の名前です。</span><span class="sxs-lookup"><span data-stu-id="0b6c9-113">Name of the setting (as defined by the directorySettingTemplate).</span></span>|
|<span data-ttu-id="0b6c9-114">value</span><span class="sxs-lookup"><span data-stu-id="0b6c9-114">value</span></span>|<span data-ttu-id="0b6c9-115">文字列</span><span class="sxs-lookup"><span data-stu-id="0b6c9-115">string</span></span>|<span data-ttu-id="0b6c9-116">設定の値です。</span><span class="sxs-lookup"><span data-stu-id="0b6c9-116">Value of the setting.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b6c9-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0b6c9-117">JSON representation</span></span>

<span data-ttu-id="0b6c9-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0b6c9-118">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "settingValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
