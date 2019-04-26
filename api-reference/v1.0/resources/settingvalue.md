---
title: settingvalue リソースの種類
description: 名前と値のペアで表される設定。
localization_priority: Normal
ms.openlocfilehash: 3edf5bdc1fae77702206eae78d53fcf0fdc5b644
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549686"
---
# <a name="settingvalue-resource-type"></a><span data-ttu-id="7c18c-103">settingvalue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7c18c-103">settingValue resource type</span></span>

<span data-ttu-id="7c18c-104">名前と値のペアで表される設定。</span><span class="sxs-lookup"><span data-stu-id="7c18c-104">A setting represented by a name/value pair.</span></span>

### <a name="properties"></a><span data-ttu-id="7c18c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c18c-105">Properties</span></span>

| <span data-ttu-id="7c18c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7c18c-106">Property</span></span> | <span data-ttu-id="7c18c-107">型</span><span class="sxs-lookup"><span data-stu-id="7c18c-107">Type</span></span> | <span data-ttu-id="7c18c-108">説明</span><span class="sxs-lookup"><span data-stu-id="7c18c-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="7c18c-109">name</span><span class="sxs-lookup"><span data-stu-id="7c18c-109">name</span></span>|<span data-ttu-id="7c18c-110">String</span><span class="sxs-lookup"><span data-stu-id="7c18c-110">String</span></span>| <span data-ttu-id="7c18c-111">設定の名前 ( [groupsettingtemplate](groupsettingtemplate.md)で定義)。</span><span class="sxs-lookup"><span data-stu-id="7c18c-111">Name of the setting (as defined by the [groupSettingTemplate](groupsettingtemplate.md)).</span></span> |
|<span data-ttu-id="7c18c-112">value</span><span class="sxs-lookup"><span data-stu-id="7c18c-112">value</span></span>|<span data-ttu-id="7c18c-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="7c18c-113">String</span></span>| <span data-ttu-id="7c18c-114">設定の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c18c-114">Value of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="7c18c-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7c18c-115">JSON representation</span></span>

<span data-ttu-id="7c18c-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7c18c-116">Here is a JSON representation of the resource.</span></span>

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
