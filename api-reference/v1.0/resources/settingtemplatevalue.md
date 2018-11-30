---
title: settingTemplateValue リソースの種類
description: 設定がインスタンス化されていない場合の、設定の既定値を含む個々のテンプレートの設定定義を表します。
ms.openlocfilehash: 00e424e36338855d8ef603d06c7a9ee52a99c621
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023692"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="caa16-103">settingTemplateValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="caa16-103">settingTemplateValue resource type</span></span>

<span data-ttu-id="caa16-104">設定がインスタンス化されていない場合の、設定の既定値を含む個々のテンプレートの設定定義を表します。</span><span class="sxs-lookup"><span data-stu-id="caa16-104">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>

### <a name="properties"></a><span data-ttu-id="caa16-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="caa16-105">Properties</span></span>

| <span data-ttu-id="caa16-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="caa16-106">Property</span></span> | <span data-ttu-id="caa16-107">型</span><span class="sxs-lookup"><span data-stu-id="caa16-107">Type</span></span> | <span data-ttu-id="caa16-108">説明</span><span class="sxs-lookup"><span data-stu-id="caa16-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="caa16-109">defaultValue</span><span class="sxs-lookup"><span data-stu-id="caa16-109">defaultValue</span></span>|<span data-ttu-id="caa16-110">文字列</span><span class="sxs-lookup"><span data-stu-id="caa16-110">String</span></span>| <span data-ttu-id="caa16-111">設定の既定値です。</span><span class="sxs-lookup"><span data-stu-id="caa16-111">Default value for the setting.</span></span> |
|<span data-ttu-id="caa16-112">説明</span><span class="sxs-lookup"><span data-stu-id="caa16-112">description</span></span>|<span data-ttu-id="caa16-113">文字列</span><span class="sxs-lookup"><span data-stu-id="caa16-113">String</span></span>| <span data-ttu-id="caa16-114">設定の説明です。</span><span class="sxs-lookup"><span data-stu-id="caa16-114">Description of the setting.</span></span> |
|<span data-ttu-id="caa16-115">名前</span><span class="sxs-lookup"><span data-stu-id="caa16-115">name</span></span>|<span data-ttu-id="caa16-116">String</span><span class="sxs-lookup"><span data-stu-id="caa16-116">String</span></span>| <span data-ttu-id="caa16-117">設定の名前です。</span><span class="sxs-lookup"><span data-stu-id="caa16-117">Name of the setting.</span></span> |
|<span data-ttu-id="caa16-118">種類</span><span class="sxs-lookup"><span data-stu-id="caa16-118">type</span></span>|<span data-ttu-id="caa16-119">文字列</span><span class="sxs-lookup"><span data-stu-id="caa16-119">String</span></span>| <span data-ttu-id="caa16-120">設定の種類です。</span><span class="sxs-lookup"><span data-stu-id="caa16-120">Type of the setting.</span></span> |

### <a name="json-representation"></a><span data-ttu-id="caa16-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="caa16-121">JSON representation</span></span>

<span data-ttu-id="caa16-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="caa16-122">Here is a JSON representation of the resource.</span></span>

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