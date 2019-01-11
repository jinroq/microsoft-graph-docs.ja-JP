---
title: alertTrigger リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: e375538806f09f85539f7a03e31c8a1ae041afdc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866648"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="8638e-104">alertTrigger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8638e-104">alertTrigger resource type</span></span>

 > <span data-ttu-id="8638e-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8638e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8638e-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8638e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8638e-107">(プロパティがアラートのエンティティに存在する)、検出をトリガーするプロパティについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8638e-107">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="8638e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8638e-108">Properties</span></span>

| <span data-ttu-id="8638e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8638e-109">Property</span></span>   | <span data-ttu-id="8638e-110">種類</span><span class="sxs-lookup"><span data-stu-id="8638e-110">Type</span></span>|<span data-ttu-id="8638e-111">説明</span><span class="sxs-lookup"><span data-stu-id="8638e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8638e-112">名前</span><span class="sxs-lookup"><span data-stu-id="8638e-112">name</span></span>|<span data-ttu-id="8638e-113">String</span><span class="sxs-lookup"><span data-stu-id="8638e-113">String</span></span>|<span data-ttu-id="8638e-114">検出のトリガーとして機能するプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="8638e-114">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="8638e-115">type</span><span class="sxs-lookup"><span data-stu-id="8638e-115">type</span></span>|<span data-ttu-id="8638e-116">String</span><span class="sxs-lookup"><span data-stu-id="8638e-116">String</span></span>|<span data-ttu-id="8638e-117">解釈のキーと値のペアのプロパティの型。</span><span class="sxs-lookup"><span data-stu-id="8638e-117">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="8638e-118">たとえば、文字列、ブール値などです。</span><span class="sxs-lookup"><span data-stu-id="8638e-118">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="8638e-119">value</span><span class="sxs-lookup"><span data-stu-id="8638e-119">value</span></span>|<span data-ttu-id="8638e-120">文字列</span><span class="sxs-lookup"><span data-stu-id="8638e-120">String</span></span>|<span data-ttu-id="8638e-121">検出のトリガーとして機能するプロパティの値です。</span><span class="sxs-lookup"><span data-stu-id="8638e-121">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8638e-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8638e-122">JSON representation</span></span>

<span data-ttu-id="8638e-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8638e-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertTrigger"
}-->

```json
{
  "name": "String",
  "type": "String",
  "value": "String"
}

```

## <a name="example"></a><span data-ttu-id="8638e-124">例</span><span class="sxs-lookup"><span data-stu-id="8638e-124">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
