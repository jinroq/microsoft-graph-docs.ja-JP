---
title: alerttrigger リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 9142c4d86b627f1d1e1e790c9b3b279b07005ad2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339161"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="b8a0d-104">alerttrigger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8a0d-104">alertTrigger resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b8a0d-105">検出をトリガーしたプロパティに関する情報が含まれています (アラートエンティティにプロパティが存在します)。</span><span class="sxs-lookup"><span data-stu-id="b8a0d-105">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="b8a0d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8a0d-106">Properties</span></span>

| <span data-ttu-id="b8a0d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8a0d-107">Property</span></span>   | <span data-ttu-id="b8a0d-108">型</span><span class="sxs-lookup"><span data-stu-id="b8a0d-108">Type</span></span>|<span data-ttu-id="b8a0d-109">説明</span><span class="sxs-lookup"><span data-stu-id="b8a0d-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b8a0d-110">name</span><span class="sxs-lookup"><span data-stu-id="b8a0d-110">name</span></span>|<span data-ttu-id="b8a0d-111">String</span><span class="sxs-lookup"><span data-stu-id="b8a0d-111">String</span></span>|<span data-ttu-id="b8a0d-112">検出トリガーとして機能するプロパティの名前。</span><span class="sxs-lookup"><span data-stu-id="b8a0d-112">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="b8a0d-113">type</span><span class="sxs-lookup"><span data-stu-id="b8a0d-113">type</span></span>|<span data-ttu-id="b8a0d-114">String</span><span class="sxs-lookup"><span data-stu-id="b8a0d-114">String</span></span>|<span data-ttu-id="b8a0d-115">キーと値のペアで解釈するプロパティの型。</span><span class="sxs-lookup"><span data-stu-id="b8a0d-115">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="b8a0d-116">たとえば、String、Boolean、などです。</span><span class="sxs-lookup"><span data-stu-id="b8a0d-116">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="b8a0d-117">value</span><span class="sxs-lookup"><span data-stu-id="b8a0d-117">value</span></span>|<span data-ttu-id="b8a0d-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b8a0d-118">String</span></span>|<span data-ttu-id="b8a0d-119">検出トリガーとして提供されるプロパティの値。</span><span class="sxs-lookup"><span data-stu-id="b8a0d-119">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8a0d-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8a0d-120">JSON representation</span></span>

<span data-ttu-id="b8a0d-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b8a0d-121">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="b8a0d-122">例</span><span class="sxs-lookup"><span data-stu-id="b8a0d-122">Example</span></span>

```json
{
  "name": "hostState.privateIpAddress",
  "type": "String",
  "value": "10.154.9.40"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "alertTrigger resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
