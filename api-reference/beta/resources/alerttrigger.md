---
title: alertTrigger リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 56034fb566f960ec858b86cdb4bcac86e5b9b47a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946428"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="d4ba4-104">alertTrigger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d4ba4-104">alertTrigger resource type</span></span>

 > <span data-ttu-id="d4ba4-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d4ba4-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4ba4-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4ba4-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d4ba4-107">(プロパティがアラートのエンティティに存在する)、検出をトリガーするプロパティについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d4ba4-107">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="d4ba4-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4ba4-108">Properties</span></span>

| <span data-ttu-id="d4ba4-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4ba4-109">Property</span></span>   | <span data-ttu-id="d4ba4-110">種類</span><span class="sxs-lookup"><span data-stu-id="d4ba4-110">Type</span></span>|<span data-ttu-id="d4ba4-111">説明</span><span class="sxs-lookup"><span data-stu-id="d4ba4-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d4ba4-112">名前</span><span class="sxs-lookup"><span data-stu-id="d4ba4-112">name</span></span>|<span data-ttu-id="d4ba4-113">String</span><span class="sxs-lookup"><span data-stu-id="d4ba4-113">String</span></span>|<span data-ttu-id="d4ba4-114">検出のトリガーとして機能するプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="d4ba4-114">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="d4ba4-115">type</span><span class="sxs-lookup"><span data-stu-id="d4ba4-115">type</span></span>|<span data-ttu-id="d4ba4-116">String</span><span class="sxs-lookup"><span data-stu-id="d4ba4-116">String</span></span>|<span data-ttu-id="d4ba4-117">解釈のキーと値のペアのプロパティの型。</span><span class="sxs-lookup"><span data-stu-id="d4ba4-117">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="d4ba4-118">たとえば、文字列、ブール値などです。</span><span class="sxs-lookup"><span data-stu-id="d4ba4-118">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="d4ba4-119">value</span><span class="sxs-lookup"><span data-stu-id="d4ba4-119">value</span></span>|<span data-ttu-id="d4ba4-120">文字列</span><span class="sxs-lookup"><span data-stu-id="d4ba4-120">String</span></span>|<span data-ttu-id="d4ba4-121">検出のトリガーとして機能するプロパティの値です。</span><span class="sxs-lookup"><span data-stu-id="d4ba4-121">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d4ba4-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d4ba4-122">JSON representation</span></span>

<span data-ttu-id="d4ba4-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d4ba4-123">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="d4ba4-124">例</span><span class="sxs-lookup"><span data-stu-id="d4ba4-124">Example</span></span>

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
