---
title: alerttrigger リソースの種類
description: 検出をトリガーしたプロパティに関する情報が含まれています (アラートエンティティにプロパティが存在します)。
author: preetikr
localization_priority: Normal
ms.prod: security
ms.openlocfilehash: 3a2f6818bad0c5600e4b2a2a2682707643d1900c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32569467"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="f616a-103">alerttrigger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f616a-103">alertTrigger resource type</span></span>

<span data-ttu-id="f616a-104">検出をトリガーしたプロパティに関する情報が含まれています (アラートエンティティにプロパティが存在します)。</span><span class="sxs-lookup"><span data-stu-id="f616a-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="f616a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f616a-105">Properties</span></span>

| <span data-ttu-id="f616a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f616a-106">Property</span></span>   | <span data-ttu-id="f616a-107">型</span><span class="sxs-lookup"><span data-stu-id="f616a-107">Type</span></span>|<span data-ttu-id="f616a-108">説明</span><span class="sxs-lookup"><span data-stu-id="f616a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f616a-109">name</span><span class="sxs-lookup"><span data-stu-id="f616a-109">name</span></span>|<span data-ttu-id="f616a-110">String</span><span class="sxs-lookup"><span data-stu-id="f616a-110">String</span></span>|<span data-ttu-id="f616a-111">検出トリガーとして機能するプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="f616a-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="f616a-112">type</span><span class="sxs-lookup"><span data-stu-id="f616a-112">type</span></span>|<span data-ttu-id="f616a-113">String</span><span class="sxs-lookup"><span data-stu-id="f616a-113">String</span></span>|<span data-ttu-id="f616a-114">キーと値のペアで解釈するプロパティの型。</span><span class="sxs-lookup"><span data-stu-id="f616a-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="f616a-115">たとえば、String、Boolean、などです。</span><span class="sxs-lookup"><span data-stu-id="f616a-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="f616a-116">value</span><span class="sxs-lookup"><span data-stu-id="f616a-116">value</span></span>|<span data-ttu-id="f616a-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f616a-117">String</span></span>|<span data-ttu-id="f616a-118">検出トリガーとして提供されるプロパティの値。</span><span class="sxs-lookup"><span data-stu-id="f616a-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f616a-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f616a-119">JSON representation</span></span>

<span data-ttu-id="f616a-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f616a-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="f616a-121">例</span><span class="sxs-lookup"><span data-stu-id="f616a-121">Example</span></span>

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
