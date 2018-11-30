---
title: alertTrigger リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
ms.openlocfilehash: 353f7dd09b11a2bfc509b53665c7f13ec390c80a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066477"
---
# <a name="alerttrigger-resource-type"></a><span data-ttu-id="52424-104">alertTrigger リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52424-104">alertTrigger resource type</span></span>

 > <span data-ttu-id="52424-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="52424-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52424-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52424-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52424-107">(プロパティがアラートのエンティティに存在する)、検出をトリガーするプロパティについて説明します。</span><span class="sxs-lookup"><span data-stu-id="52424-107">Contains information about the properties that triggered a detection (properties exist in the alert entity).</span></span>

## <a name="properties"></a><span data-ttu-id="52424-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52424-108">Properties</span></span>

| <span data-ttu-id="52424-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52424-109">Property</span></span>   | <span data-ttu-id="52424-110">型</span><span class="sxs-lookup"><span data-stu-id="52424-110">Type</span></span>|<span data-ttu-id="52424-111">説明</span><span class="sxs-lookup"><span data-stu-id="52424-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52424-112">名前</span><span class="sxs-lookup"><span data-stu-id="52424-112">name</span></span>|<span data-ttu-id="52424-113">String</span><span class="sxs-lookup"><span data-stu-id="52424-113">String</span></span>|<span data-ttu-id="52424-114">検出のトリガーとして機能するプロパティの名前です。</span><span class="sxs-lookup"><span data-stu-id="52424-114">Name of the property serving as a detection trigger.</span></span>|
|<span data-ttu-id="52424-115">type</span><span class="sxs-lookup"><span data-stu-id="52424-115">type</span></span>|<span data-ttu-id="52424-116">String</span><span class="sxs-lookup"><span data-stu-id="52424-116">String</span></span>|<span data-ttu-id="52424-117">解釈のキーと値のペアのプロパティの型。</span><span class="sxs-lookup"><span data-stu-id="52424-117">Type of the property in the key:value pair for interpretation.</span></span> <span data-ttu-id="52424-118">たとえば、文字列、ブール値などです。</span><span class="sxs-lookup"><span data-stu-id="52424-118">For example, String, Boolean, etc.</span></span>|
|<span data-ttu-id="52424-119">value</span><span class="sxs-lookup"><span data-stu-id="52424-119">value</span></span>|<span data-ttu-id="52424-120">文字列</span><span class="sxs-lookup"><span data-stu-id="52424-120">String</span></span>|<span data-ttu-id="52424-121">検出のトリガーとして機能するプロパティの値です。</span><span class="sxs-lookup"><span data-stu-id="52424-121">Value of the property serving as a detection trigger.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52424-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52424-122">JSON representation</span></span>

<span data-ttu-id="52424-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="52424-123">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="52424-124">使用例</span><span class="sxs-lookup"><span data-stu-id="52424-124">Example</span></span>

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
