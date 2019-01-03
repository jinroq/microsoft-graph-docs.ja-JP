---
title: resourceReference リソースの種類
description: 複合型のプロパティ情報にはが含まれています。
author: simonhult
ms.openlocfilehash: 2f1a44412eebbb7a74895c12db9a07696d6ee409
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27363621"
---
# <a name="resourcereference-resource-type"></a><span data-ttu-id="c08fd-103">resourceReference リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c08fd-103">resourceReference resource type</span></span>

> <span data-ttu-id="c08fd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c08fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c08fd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c08fd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c08fd-106">複合型のプロパティ[情報](insights.md)にはが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c08fd-106">Complex type containing properties of [Insights](insights.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="c08fd-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c08fd-107">JSON representation</span></span>

<span data-ttu-id="c08fd-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="c08fd-108">Here is a JSON representation of the resource</span></span>

```json
{
  "webUrl": "string",
  "id": "string",
  "type": "string"
}
```

## <a name="properties"></a><span data-ttu-id="c08fd-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c08fd-109">Properties</span></span>

| <span data-ttu-id="c08fd-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c08fd-110">Property</span></span>      | <span data-ttu-id="c08fd-111">種類</span><span class="sxs-lookup"><span data-stu-id="c08fd-111">Type</span></span>      | <span data-ttu-id="c08fd-112">説明</span><span class="sxs-lookup"><span data-stu-id="c08fd-112">Description</span></span>  |
| ------------- |-----------| -------------|
| <span data-ttu-id="c08fd-113">webUrl</span><span class="sxs-lookup"><span data-stu-id="c08fd-113">webUrl</span></span>        | <span data-ttu-id="c08fd-114">String</span><span class="sxs-lookup"><span data-stu-id="c08fd-114">String</span></span>    | <span data-ttu-id="c08fd-115">参照先の項目に先行する URL です。</span><span class="sxs-lookup"><span data-stu-id="c08fd-115">A URL leading to the referenced item.</span></span> |
| <span data-ttu-id="c08fd-116">id</span><span class="sxs-lookup"><span data-stu-id="c08fd-116">id</span></span>            | <span data-ttu-id="c08fd-117">String</span><span class="sxs-lookup"><span data-stu-id="c08fd-117">String</span></span>    | <span data-ttu-id="c08fd-118">アイテムの一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="c08fd-118">The item's unique identifier.</span></span>           |
| <span data-ttu-id="c08fd-119">type</span><span class="sxs-lookup"><span data-stu-id="c08fd-119">type</span></span>          | <span data-ttu-id="c08fd-120">String</span><span class="sxs-lookup"><span data-stu-id="c08fd-120">String</span></span>    | <span data-ttu-id="c08fd-121">文字列値"microsoft.graph.driveItem"など、アイテムの分類に使用できます。</span><span class="sxs-lookup"><span data-stu-id="c08fd-121">A string value that can be used to classify the item, such as "microsoft.graph.driveItem"</span></span> |