---
title: insightIdentity
description: 共有アイテムのプロパティを格納する複合型。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: a263caa68280128a67a027b75682407fd4932605
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938938"
---
# <a name="insightidentity"></a><span data-ttu-id="16ad2-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="16ad2-103">insightIdentity</span></span>

> <span data-ttu-id="16ad2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16ad2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16ad2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16ad2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="16ad2-106">[共有](insights-shared.md)アイテムのプロパティを格納する複合型。</span><span class="sxs-lookup"><span data-stu-id="16ad2-106">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="16ad2-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="16ad2-107">JSON representation</span></span>
<span data-ttu-id="16ad2-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="16ad2-108">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="16ad2-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16ad2-109">Properties</span></span>

| <span data-ttu-id="16ad2-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16ad2-110">Property</span></span>              | <span data-ttu-id="16ad2-111">種類</span><span class="sxs-lookup"><span data-stu-id="16ad2-111">Type</span></span>          | <span data-ttu-id="16ad2-112">説明</span><span class="sxs-lookup"><span data-stu-id="16ad2-112">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="16ad2-113">displayName</span><span class="sxs-lookup"><span data-stu-id="16ad2-113">displayName</span></span>       | <span data-ttu-id="16ad2-114">String</span><span class="sxs-lookup"><span data-stu-id="16ad2-114">String</span></span>          | <span data-ttu-id="16ad2-115">アイテムを共有するユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="16ad2-115">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="16ad2-116">id</span><span class="sxs-lookup"><span data-stu-id="16ad2-116">id</span></span>              | <span data-ttu-id="16ad2-117">String</span><span class="sxs-lookup"><span data-stu-id="16ad2-117">String</span></span>        | <span data-ttu-id="16ad2-118">アイテムを共有するユーザーの id です。</span><span class="sxs-lookup"><span data-stu-id="16ad2-118">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="16ad2-119">address</span><span class="sxs-lookup"><span data-stu-id="16ad2-119">address</span></span>             | <span data-ttu-id="16ad2-120">String</span><span class="sxs-lookup"><span data-stu-id="16ad2-120">String</span></span>      | <span data-ttu-id="16ad2-121">アイテムを共有するユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="16ad2-121">The email address of the user who shared the item.</span></span>  |
