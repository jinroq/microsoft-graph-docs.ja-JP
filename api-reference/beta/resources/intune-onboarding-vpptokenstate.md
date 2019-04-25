---
title: vpptokenstate 列挙型
description: Apple volume purchase program のトークンに関連付けられている状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dbc62b855035ebf68fefae3d628582b566804449
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566424"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="259ed-103">vpptokenstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="259ed-103">vppTokenState enum type</span></span>

> <span data-ttu-id="259ed-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="259ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="259ed-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="259ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="259ed-106">Apple volume purchase program のトークンに関連付けられている状態。</span><span class="sxs-lookup"><span data-stu-id="259ed-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="259ed-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="259ed-107">Members</span></span>
|<span data-ttu-id="259ed-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="259ed-108">Member</span></span>|<span data-ttu-id="259ed-109">値</span><span class="sxs-lookup"><span data-stu-id="259ed-109">Value</span></span>|<span data-ttu-id="259ed-110">説明</span><span class="sxs-lookup"><span data-stu-id="259ed-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="259ed-111">不明</span><span class="sxs-lookup"><span data-stu-id="259ed-111">unknown</span></span>|<span data-ttu-id="259ed-112">.0</span><span class="sxs-lookup"><span data-stu-id="259ed-112">0</span></span>|<span data-ttu-id="259ed-113">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="259ed-113">Default state.</span></span>|
|<span data-ttu-id="259ed-114">有効な</span><span class="sxs-lookup"><span data-stu-id="259ed-114">valid</span></span>|<span data-ttu-id="259ed-115">1 </span><span class="sxs-lookup"><span data-stu-id="259ed-115">1</span></span>|<span data-ttu-id="259ed-116">トークンが有効です。</span><span class="sxs-lookup"><span data-stu-id="259ed-116">Token is valid.</span></span>|
|<span data-ttu-id="259ed-117">終了</span><span class="sxs-lookup"><span data-stu-id="259ed-117">expired</span></span>|<span data-ttu-id="259ed-118">2 </span><span class="sxs-lookup"><span data-stu-id="259ed-118">2</span></span>|<span data-ttu-id="259ed-119">トークンの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="259ed-119">Token is expired.</span></span>|
|<span data-ttu-id="259ed-120">無効です</span><span class="sxs-lookup"><span data-stu-id="259ed-120">invalid</span></span>|<span data-ttu-id="259ed-121">3 </span><span class="sxs-lookup"><span data-stu-id="259ed-121">3</span></span>|<span data-ttu-id="259ed-122">トークンが無効です。</span><span class="sxs-lookup"><span data-stu-id="259ed-122">Token is invalid.</span></span>|
|<span data-ttu-id="259ed-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="259ed-123">assignedToExternalMDM</span></span>|<span data-ttu-id="259ed-124">4 </span><span class="sxs-lookup"><span data-stu-id="259ed-124">4</span></span>|<span data-ttu-id="259ed-125">トークンは別の MDM サービスによって管理されています。</span><span class="sxs-lookup"><span data-stu-id="259ed-125">Token is managed by another MDM Service.</span></span>|





