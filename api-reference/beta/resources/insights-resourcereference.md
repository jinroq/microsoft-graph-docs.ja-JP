---
title: resourceReference リソースの種類
description: 複合型のプロパティ情報にはが含まれています。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 8ab2a79d66db6a45ecf3df748cf8f5740721ef80
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874327"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="47169-103">resourceReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="47169-103">resourceReference resource type</span></span>

> <span data-ttu-id="47169-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="47169-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="47169-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47169-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="47169-106">複合型のプロパティ[情報](insights.md)にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="47169-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="47169-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="47169-107">JSON representation</span></span>

<span data-ttu-id="47169-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="47169-108">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="47169-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47169-109">Properties</span></span>

| <span data-ttu-id="47169-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="47169-110">Property</span></span>      | <span data-ttu-id="47169-111">種類</span><span class="sxs-lookup"><span data-stu-id="47169-111">Type</span></span>      | <span data-ttu-id="47169-112">説明</span><span class="sxs-lookup"><span data-stu-id="47169-112">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="47169-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="47169-113">webUrl</span></span>        | <span data-ttu-id="47169-114">String</span><span class="sxs-lookup"><span data-stu-id="47169-114">String</span></span>    | <span data-ttu-id="47169-115">参照先の項目に先行する URL です。</span><span class="sxs-lookup"><span data-stu-id="47169-115">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="47169-116">id</span><span class="sxs-lookup"><span data-stu-id="47169-116">id</span></span>            | <span data-ttu-id="47169-117">String</span><span class="sxs-lookup"><span data-stu-id="47169-117">String</span></span>    | <span data-ttu-id="47169-118">アイテムの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="47169-118">The item's unique identifier.</span></span>           |
| <span data-ttu-id="47169-119">type</span><span class="sxs-lookup"><span data-stu-id="47169-119">type</span></span>          | <span data-ttu-id="47169-120">String</span><span class="sxs-lookup"><span data-stu-id="47169-120">String</span></span>    | <span data-ttu-id="47169-121">文字列値"microsoft.graph.driveItem"など、アイテムの分類に使用できます。</span><span class="sxs-lookup"><span data-stu-id="47169-121">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |
