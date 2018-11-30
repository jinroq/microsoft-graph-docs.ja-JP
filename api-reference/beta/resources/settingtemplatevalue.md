---
title: settingTemplateValue リソースの種類
description: 設定がインスタンス化されていない場合の、設定の既定値を含む個々のテンプレートの設定定義を表します。
ms.openlocfilehash: afc872f3e3d8d02acae639b967cdaf9375bb60cb
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069805"
---
# <a name="settingtemplatevalue-resource-type"></a><span data-ttu-id="3c071-103">settingTemplateValue リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3c071-103">settingTemplateValue resource type</span></span>

> <span data-ttu-id="3c071-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3c071-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3c071-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3c071-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3c071-106">設定がインスタンス化されていない場合の、設定の既定値を含む個々のテンプレートの設定定義を表します。</span><span class="sxs-lookup"><span data-stu-id="3c071-106">Represents an individual template setting definition, including the default value for the setting, if the setting is not instantiated.</span></span>


## <a name="properties"></a><span data-ttu-id="3c071-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c071-107">Properties</span></span>
| <span data-ttu-id="3c071-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c071-108">Property</span></span>     | <span data-ttu-id="3c071-109">型</span><span class="sxs-lookup"><span data-stu-id="3c071-109">Type</span></span>   |<span data-ttu-id="3c071-110">説明</span><span class="sxs-lookup"><span data-stu-id="3c071-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c071-111">defaultValue</span><span class="sxs-lookup"><span data-stu-id="3c071-111">defaultValue</span></span>|<span data-ttu-id="3c071-112">文字列</span><span class="sxs-lookup"><span data-stu-id="3c071-112">string</span></span>|<span data-ttu-id="3c071-113">設定の既定値です。</span><span class="sxs-lookup"><span data-stu-id="3c071-113">Default value for the setting.</span></span> <span data-ttu-id="3c071-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3c071-114">Read-only.</span></span>|
|<span data-ttu-id="3c071-115">説明</span><span class="sxs-lookup"><span data-stu-id="3c071-115">description</span></span>|<span data-ttu-id="3c071-116">文字列</span><span class="sxs-lookup"><span data-stu-id="3c071-116">string</span></span>|<span data-ttu-id="3c071-117">設定の説明です。</span><span class="sxs-lookup"><span data-stu-id="3c071-117">Description of the setting.</span></span> <span data-ttu-id="3c071-118">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c071-118">Read-only.</span></span>|
|<span data-ttu-id="3c071-119">name</span><span class="sxs-lookup"><span data-stu-id="3c071-119">name</span></span>|<span data-ttu-id="3c071-120">文字列</span><span class="sxs-lookup"><span data-stu-id="3c071-120">string</span></span>|<span data-ttu-id="3c071-121">設定の名前。</span><span class="sxs-lookup"><span data-stu-id="3c071-121">Name of the setting.</span></span> <span data-ttu-id="3c071-122">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c071-122">Read-only.</span></span>|
|<span data-ttu-id="3c071-123">type</span><span class="sxs-lookup"><span data-stu-id="3c071-123">type</span></span>|<span data-ttu-id="3c071-124">文字列</span><span class="sxs-lookup"><span data-stu-id="3c071-124">string</span></span>|<span data-ttu-id="3c071-125">設定の種類です。</span><span class="sxs-lookup"><span data-stu-id="3c071-125">Type of the setting.</span></span> <span data-ttu-id="3c071-126">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="3c071-126">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3c071-127">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3c071-127">JSON representation</span></span>

<span data-ttu-id="3c071-128">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3c071-128">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "settingTemplateValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
