---
title: settingtemplatevalue リソースの種類
description: 設定がインスタンス化されていない場合に、設定の既定値を含む、個々のテンプレート設定の定義を表します。
localization_priority: Normal
ms.openlocfilehash: 0cb3376177e3a4efcae54a591a083914db6b56d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549693"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="bba5d-103">settingtemplatevalue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bba5d-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="bba5d-104">設定がインスタンス化されていない場合に、設定の既定値を含む、個々のテンプレート設定の定義を表します。</span><span class="sxs-lookup"><span data-stu-id="bba5d-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="bba5d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bba5d-105">Properties</span></span>

| <span data-ttu-id="bba5d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bba5d-106">Property</span></span> | <span data-ttu-id="bba5d-107">型</span><span class="sxs-lookup"><span data-stu-id="bba5d-107">Type</span></span> | <span data-ttu-id="bba5d-108">説明</span><span class="sxs-lookup"><span data-stu-id="bba5d-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="bba5d-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="bba5d-109">defaultValue</span></span>|<span data-ttu-id="bba5d-110">String</span><span class="sxs-lookup"><span data-stu-id="bba5d-110">String</span></span>| <span data-ttu-id="bba5d-111">設定の既定値。</span><span class="sxs-lookup"><span data-stu-id="bba5d-111">Default value for the setting.</span></span> |
|<span data-ttu-id="bba5d-112">description</span><span class="sxs-lookup"><span data-stu-id="bba5d-112">description</span></span>|<span data-ttu-id="bba5d-113">String</span><span class="sxs-lookup"><span data-stu-id="bba5d-113">String</span></span>| <span data-ttu-id="bba5d-114">設定の説明。</span><span class="sxs-lookup"><span data-stu-id="bba5d-114">Description of the setting.</span></span> |
|<span data-ttu-id="bba5d-115">name</span><span class="sxs-lookup"><span data-stu-id="bba5d-115">name</span></span>|<span data-ttu-id="bba5d-116">String</span><span class="sxs-lookup"><span data-stu-id="bba5d-116">String</span></span>| <span data-ttu-id="bba5d-117">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="bba5d-117">Name of the setting.</span></span> |
|<span data-ttu-id="bba5d-118">type</span><span class="sxs-lookup"><span data-stu-id="bba5d-118">type</span></span>|<span data-ttu-id="bba5d-119">String</span><span class="sxs-lookup"><span data-stu-id="bba5d-119">String</span></span>| <span data-ttu-id="bba5d-120">設定の種類。</span><span class="sxs-lookup"><span data-stu-id="bba5d-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="bba5d-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bba5d-121">JSON representation</span></span>

<span data-ttu-id="bba5d-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bba5d-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.settingTemplateValue"
}-->

```json
{
  "defaultValue": "String",
  "description": "String",
  "name": "String",
  "type": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
