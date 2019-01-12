---
title: alertTrigger リソースの種類
description: (プロパティがアラートのエンティティに存在する)、検出をトリガーするプロパティについて説明します。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 3a2f6818bad0c5600e4b2a2a2682707643d1900c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991259"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="3622a-103">alertTrigger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3622a-103">alertTrigger resource type</span></span>

<span data-ttu-id="3622a-104">(プロパティがアラートのエンティティに存在する)、検出をトリガーするプロパティについて説明します。</span><span class="sxs-lookup"><span data-stu-id="3622a-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="3622a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3622a-105">Properties</span></span>

| <span data-ttu-id="3622a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3622a-106">Property</span></span>   | <span data-ttu-id="3622a-107">種類</span><span class="sxs-lookup"><span data-stu-id="3622a-107">Type</span></span>|<span data-ttu-id="3622a-108">説明</span><span class="sxs-lookup"><span data-stu-id="3622a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3622a-109">名前</span><span class="sxs-lookup"><span data-stu-id="3622a-109">name</span></span>|<span data-ttu-id="3622a-110">String</span><span class="sxs-lookup"><span data-stu-id="3622a-110">String</span></span>|<span data-ttu-id="3622a-111">検出のトリガーとして機能するプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="3622a-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="3622a-112">type</span><span class="sxs-lookup"><span data-stu-id="3622a-112">type</span></span>|<span data-ttu-id="3622a-113">String</span><span class="sxs-lookup"><span data-stu-id="3622a-113">String</span></span>|<span data-ttu-id="3622a-114">解釈のキーと値のペアのプロパティの型。</span><span class="sxs-lookup"><span data-stu-id="3622a-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="3622a-115">たとえば、文字列、ブール値などです。</span><span class="sxs-lookup"><span data-stu-id="3622a-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="3622a-116">value</span><span class="sxs-lookup"><span data-stu-id="3622a-116">value</span></span>|<span data-ttu-id="3622a-117">文字列</span><span class="sxs-lookup"><span data-stu-id="3622a-117">String</span></span>|<span data-ttu-id="3622a-118">検出のトリガーとして機能するプロパティの値です。</span><span class="sxs-lookup"><span data-stu-id="3622a-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3622a-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3622a-119">JSON representation</span></span>

<span data-ttu-id="3622a-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3622a-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="3622a-121">例</span><span class="sxs-lookup"><span data-stu-id="3622a-121">Example</span></span>

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
