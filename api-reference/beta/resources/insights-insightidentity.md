---
title: insightIdentity
description: " リソースの種類"
ms.openlocfilehash: e13d08eb111844896c96b02ab22c52d2f598ce58
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071083"
---
# <a name="insightidentity"></a><span data-ttu-id="2b165-103">insightIdentity</span><span class="sxs-lookup"><span data-stu-id="2b165-103">insightIdentity</span></span>

> <span data-ttu-id="2b165-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b165-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b165-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b165-105">Use of these APIs in production applications is not supported.</span></span>

 <span data-ttu-id="2b165-106">リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b165-106">resource type</span></span>

<span data-ttu-id="2b165-107">[共有](insights-shared.md)アイテムのプロパティを格納する複合型。</span><span class="sxs-lookup"><span data-stu-id="2b165-107">Complex type containing properties of [Shared](insights-shared.md) items.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="2b165-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b165-108">JSON representation</span></span>
<span data-ttu-id="2b165-109">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="2b165-109">Here is a JSON representation of the resource</span></span>

```json
{
  "displayName": "string",
  "id": "string",
  "address": "string"
}
```

## <a name="properties"></a><span data-ttu-id="2b165-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b165-110">Properties</span></span>

| <span data-ttu-id="2b165-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b165-111">Property</span></span>              | <span data-ttu-id="2b165-112">型</span><span class="sxs-lookup"><span data-stu-id="2b165-112">Type</span></span>          | <span data-ttu-id="2b165-113">説明</span><span class="sxs-lookup"><span data-stu-id="2b165-113">Description</span></span>  |
| -------------         |-----------    | -------------|
| <span data-ttu-id="2b165-114">displayName</span><span class="sxs-lookup"><span data-stu-id="2b165-114">displayName</span></span>       | <span data-ttu-id="2b165-115">String</span><span class="sxs-lookup"><span data-stu-id="2b165-115">String</span></span>          | <span data-ttu-id="2b165-116">アイテムを共有するユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="2b165-116">The display name of the user who shared the item.</span></span> |
| <span data-ttu-id="2b165-117">id</span><span class="sxs-lookup"><span data-stu-id="2b165-117">id</span></span>              | <span data-ttu-id="2b165-118">String</span><span class="sxs-lookup"><span data-stu-id="2b165-118">String</span></span>        | <span data-ttu-id="2b165-119">アイテムを共有するユーザーの id です。</span><span class="sxs-lookup"><span data-stu-id="2b165-119">The id of the user who shared the item.</span></span>     |
| <span data-ttu-id="2b165-120">address</span><span class="sxs-lookup"><span data-stu-id="2b165-120">address</span></span>             | <span data-ttu-id="2b165-121">String</span><span class="sxs-lookup"><span data-stu-id="2b165-121">String</span></span>      | <span data-ttu-id="2b165-122">アイテムを共有するユーザーの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="2b165-122">The email address of the user who shared the item.</span></span>  |