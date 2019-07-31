---
title: vppTokenState 列挙型
description: Apple Volume Purchase Program のトークンに関連付けられている状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d9ae2b3bfb45ff33c5f0a39d746350212db3027c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010638"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="14273-103">vppTokenState 列挙型</span><span class="sxs-lookup"><span data-stu-id="14273-103">vppTokenState enum type</span></span>

> <span data-ttu-id="14273-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14273-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14273-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="14273-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14273-106">Apple Volume Purchase Program のトークンに関連付けられている状態。</span><span class="sxs-lookup"><span data-stu-id="14273-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="14273-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="14273-107">Members</span></span>
|<span data-ttu-id="14273-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="14273-108">Member</span></span>|<span data-ttu-id="14273-109">値</span><span class="sxs-lookup"><span data-stu-id="14273-109">Value</span></span>|<span data-ttu-id="14273-110">説明</span><span class="sxs-lookup"><span data-stu-id="14273-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14273-111">不明</span><span class="sxs-lookup"><span data-stu-id="14273-111">unknown</span></span>|<span data-ttu-id="14273-112">.0</span><span class="sxs-lookup"><span data-stu-id="14273-112">0</span></span>|<span data-ttu-id="14273-113">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="14273-113">Default state.</span></span>|
|<span data-ttu-id="14273-114">有効な</span><span class="sxs-lookup"><span data-stu-id="14273-114">valid</span></span>|<span data-ttu-id="14273-115">1-d</span><span class="sxs-lookup"><span data-stu-id="14273-115">1</span></span>|<span data-ttu-id="14273-116">トークンが有効です。</span><span class="sxs-lookup"><span data-stu-id="14273-116">Token is valid.</span></span>|
|<span data-ttu-id="14273-117">終了</span><span class="sxs-lookup"><span data-stu-id="14273-117">expired</span></span>|<span data-ttu-id="14273-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="14273-118">2</span></span>|<span data-ttu-id="14273-119">トークンの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="14273-119">Token is expired.</span></span>|
|<span data-ttu-id="14273-120">無効です</span><span class="sxs-lookup"><span data-stu-id="14273-120">invalid</span></span>|<span data-ttu-id="14273-121">1/3</span><span class="sxs-lookup"><span data-stu-id="14273-121">3</span></span>|<span data-ttu-id="14273-122">トークンが無効です。</span><span class="sxs-lookup"><span data-stu-id="14273-122">Token is invalid.</span></span>|
|<span data-ttu-id="14273-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="14273-123">assignedToExternalMDM</span></span>|<span data-ttu-id="14273-124">2/4</span><span class="sxs-lookup"><span data-stu-id="14273-124">4</span></span>|<span data-ttu-id="14273-125">トークンは別の MDM サービスによって管理されています。</span><span class="sxs-lookup"><span data-stu-id="14273-125">Token is managed by another MDM Service.</span></span>|





