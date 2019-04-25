---
title: vpptokenstate 列挙型
description: Apple volume purchase program のトークンに関連付けられている状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 573fe27064881f670e642e7c3727b8c9eb7db5a9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548160"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="da1b9-103">vpptokenstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="da1b9-103">vppTokenState enum type</span></span>

> <span data-ttu-id="da1b9-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="da1b9-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da1b9-105">Apple volume purchase program のトークンに関連付けられている状態。</span><span class="sxs-lookup"><span data-stu-id="da1b9-105">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="da1b9-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="da1b9-106">Members</span></span>
|<span data-ttu-id="da1b9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="da1b9-107">Member</span></span>|<span data-ttu-id="da1b9-108">値</span><span class="sxs-lookup"><span data-stu-id="da1b9-108">Value</span></span>|<span data-ttu-id="da1b9-109">説明</span><span class="sxs-lookup"><span data-stu-id="da1b9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da1b9-110">不明</span><span class="sxs-lookup"><span data-stu-id="da1b9-110">unknown</span></span>|<span data-ttu-id="da1b9-111">.0</span><span class="sxs-lookup"><span data-stu-id="da1b9-111">0</span></span>|<span data-ttu-id="da1b9-112">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="da1b9-112">Default state.</span></span>|
|<span data-ttu-id="da1b9-113">有効な</span><span class="sxs-lookup"><span data-stu-id="da1b9-113">valid</span></span>|<span data-ttu-id="da1b9-114">1 </span><span class="sxs-lookup"><span data-stu-id="da1b9-114">1</span></span>|<span data-ttu-id="da1b9-115">トークンが有効です。</span><span class="sxs-lookup"><span data-stu-id="da1b9-115">Token is valid.</span></span>|
|<span data-ttu-id="da1b9-116">終了</span><span class="sxs-lookup"><span data-stu-id="da1b9-116">expired</span></span>|<span data-ttu-id="da1b9-117">2 </span><span class="sxs-lookup"><span data-stu-id="da1b9-117">2</span></span>|<span data-ttu-id="da1b9-118">トークンの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="da1b9-118">Token is expired.</span></span>|
|<span data-ttu-id="da1b9-119">無効です</span><span class="sxs-lookup"><span data-stu-id="da1b9-119">invalid</span></span>|<span data-ttu-id="da1b9-120">3 </span><span class="sxs-lookup"><span data-stu-id="da1b9-120">3</span></span>|<span data-ttu-id="da1b9-121">トークンが無効です。</span><span class="sxs-lookup"><span data-stu-id="da1b9-121">Token is invalid.</span></span>|
|<span data-ttu-id="da1b9-122">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="da1b9-122">assignedToExternalMDM</span></span>|<span data-ttu-id="da1b9-123">4 </span><span class="sxs-lookup"><span data-stu-id="da1b9-123">4</span></span>|<span data-ttu-id="da1b9-124">トークンは別の MDM サービスによって管理されています。</span><span class="sxs-lookup"><span data-stu-id="da1b9-124">Token is managed by another MDM Service.</span></span>|



