---
title: insightIdentity
description: 共有アイテムのプロパティを格納する複合型。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: 395c865a38ebe6ea84dc64857f441cd529e4f2d6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886577"
---
# <a name="insightidentity"></a><span data-ttu-id="0d21b-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="0d21b-103">insightIdentity</span></span>

> <span data-ttu-id="0d21b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0d21b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d21b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0d21b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d21b-106">[共有](insights-shared.md)アイテムのプロパティを格納する複合型。</span><span class="sxs-lookup"><span data-stu-id="0d21b-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="0d21b-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0d21b-107">JSON representation</span></span>
<span data-ttu-id="0d21b-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0d21b-108">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="0d21b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d21b-109">Properties</span></span>

| <span data-ttu-id="0d21b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0d21b-110">Property</span></span>              | <span data-ttu-id="0d21b-111">種類</span><span class="sxs-lookup"><span data-stu-id="0d21b-111">Type</span></span>          | <span data-ttu-id="0d21b-112">説明</span><span class="sxs-lookup"><span data-stu-id="0d21b-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="0d21b-113">displayName</span><span class="sxs-lookup"><span data-stu-id="0d21b-113">displayName</span></span>       | <span data-ttu-id="0d21b-114">String</span><span class="sxs-lookup"><span data-stu-id="0d21b-114">String</span></span>          | <span data-ttu-id="0d21b-115">アイテムを共有するユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="0d21b-115">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="0d21b-116">id</span><span class="sxs-lookup"><span data-stu-id="0d21b-116">id</span></span>              | <span data-ttu-id="0d21b-117">String</span><span class="sxs-lookup"><span data-stu-id="0d21b-117">String</span></span>        | <span data-ttu-id="0d21b-118">アイテムを共有するユーザーの id です。</span><span class="sxs-lookup"><span data-stu-id="0d21b-118">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="0d21b-119">address</span><span class="sxs-lookup"><span data-stu-id="0d21b-119">address</span></span>             | <span data-ttu-id="0d21b-120">String</span><span class="sxs-lookup"><span data-stu-id="0d21b-120">String</span></span>      | <span data-ttu-id="0d21b-121">アイテムを共有するユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="0d21b-121">The email address of the user who shared the item.</span></span>  |
