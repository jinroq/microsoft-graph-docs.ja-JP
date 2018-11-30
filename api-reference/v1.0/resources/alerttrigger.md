---
title: alertTrigger リソースの種類
description: (プロパティがアラートのエンティティに存在する)、検出をトリガーするプロパティについて説明します。
ms.openlocfilehash: b4af3be67669fd27f27e888cbc28b60b0c1c67a5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023539"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="52448-103">alertTrigger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52448-103">alertTrigger resource type</span></span>

<span data-ttu-id="52448-104">(プロパティがアラートのエンティティに存在する)、検出をトリガーするプロパティについて説明します。</span><span class="sxs-lookup"><span data-stu-id="52448-104">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="52448-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52448-105">Properties</span></span>

| <span data-ttu-id="52448-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52448-106">Property</span></span>   | <span data-ttu-id="52448-107">型</span><span class="sxs-lookup"><span data-stu-id="52448-107">Type</span></span>|<span data-ttu-id="52448-108">説明</span><span class="sxs-lookup"><span data-stu-id="52448-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52448-109">名前</span><span class="sxs-lookup"><span data-stu-id="52448-109">name</span></span>|<span data-ttu-id="52448-110">String</span><span class="sxs-lookup"><span data-stu-id="52448-110">String</span></span>|<span data-ttu-id="52448-111">検出のトリガーとして機能するプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="52448-111">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="52448-112">type</span><span class="sxs-lookup"><span data-stu-id="52448-112">type</span></span>|<span data-ttu-id="52448-113">String</span><span class="sxs-lookup"><span data-stu-id="52448-113">String</span></span>|<span data-ttu-id="52448-114">解釈のキーと値のペアのプロパティの型。</span><span class="sxs-lookup"><span data-stu-id="52448-114">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="52448-115">たとえば、文字列、ブール値などです。</span><span class="sxs-lookup"><span data-stu-id="52448-115">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="52448-116">value</span><span class="sxs-lookup"><span data-stu-id="52448-116">value</span></span>|<span data-ttu-id="52448-117">文字列</span><span class="sxs-lookup"><span data-stu-id="52448-117">String</span></span>|<span data-ttu-id="52448-118">検出のトリガーとして機能するプロパティの値です。</span><span class="sxs-lookup"><span data-stu-id="52448-118">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52448-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52448-119">JSON representation</span></span>

<span data-ttu-id="52448-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52448-120">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="52448-121">使用例</span><span class="sxs-lookup"><span data-stu-id="52448-121">Example</span></span>

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