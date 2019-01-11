---
title: settingTemplateValue リソースの種類
description: 設定がインスタンス化されていない場合の、設定の既定値を含む個々のテンプレートの設定定義を表します。
localization_priority: Normal
ms.openlocfilehash: 0cb3376177e3a4efcae54a591a083914db6b56d7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27828323"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="53221-103">settingTemplateValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="53221-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="53221-104">設定がインスタンス化されていない場合の、設定の既定値を含む個々のテンプレートの設定定義を表します。</span><span class="sxs-lookup"><span data-stu-id="53221-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="53221-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53221-105">Properties</span></span>

| <span data-ttu-id="53221-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="53221-106">Property</span></span> | <span data-ttu-id="53221-107">種類</span><span class="sxs-lookup"><span data-stu-id="53221-107">Type</span></span> | <span data-ttu-id="53221-108">説明</span><span class="sxs-lookup"><span data-stu-id="53221-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="53221-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="53221-109">defaultValue</span></span>|<span data-ttu-id="53221-110">文字列</span><span class="sxs-lookup"><span data-stu-id="53221-110">String</span></span>| <span data-ttu-id="53221-111">設定の既定値です。</span><span class="sxs-lookup"><span data-stu-id="53221-111">Default value for the setting.</span></span> |
|<span data-ttu-id="53221-112">説明</span><span class="sxs-lookup"><span data-stu-id="53221-112">description</span></span>|<span data-ttu-id="53221-113">文字列</span><span class="sxs-lookup"><span data-stu-id="53221-113">String</span></span>| <span data-ttu-id="53221-114">設定の説明です。</span><span class="sxs-lookup"><span data-stu-id="53221-114">Description of the setting.</span></span> |
|<span data-ttu-id="53221-115">名前</span><span class="sxs-lookup"><span data-stu-id="53221-115">name</span></span>|<span data-ttu-id="53221-116">String</span><span class="sxs-lookup"><span data-stu-id="53221-116">String</span></span>| <span data-ttu-id="53221-117">設定の名前です。</span><span class="sxs-lookup"><span data-stu-id="53221-117">Name of the setting.</span></span> |
|<span data-ttu-id="53221-118">種類</span><span class="sxs-lookup"><span data-stu-id="53221-118">type</span></span>|<span data-ttu-id="53221-119">文字列</span><span class="sxs-lookup"><span data-stu-id="53221-119">String</span></span>| <span data-ttu-id="53221-120">設定の種類です。</span><span class="sxs-lookup"><span data-stu-id="53221-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="53221-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="53221-121">JSON representation</span></span>

<span data-ttu-id="53221-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="53221-122">Here is a JSON representation of the resource.</span></span>

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
