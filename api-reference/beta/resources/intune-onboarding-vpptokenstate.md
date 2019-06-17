---
title: vppTokenState 列挙型
description: Apple Volume Purchase Program のトークンに関連付けられている状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: faef244a196ae99a9ba82f4c5396db22b79be8b5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958516"
---
# <a name="vpptokenstate-enum-type"></a><span data-ttu-id="0520f-103">vppTokenState 列挙型</span><span class="sxs-lookup"><span data-stu-id="0520f-103">vppTokenState enum type</span></span>

> <span data-ttu-id="0520f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0520f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0520f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0520f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0520f-106">Apple Volume Purchase Program のトークンに関連付けられている状態。</span><span class="sxs-lookup"><span data-stu-id="0520f-106">Possible states associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="0520f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0520f-107">Members</span></span>
|<span data-ttu-id="0520f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="0520f-108">Member</span></span>|<span data-ttu-id="0520f-109">値</span><span class="sxs-lookup"><span data-stu-id="0520f-109">Value</span></span>|<span data-ttu-id="0520f-110">説明</span><span class="sxs-lookup"><span data-stu-id="0520f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0520f-111">不明</span><span class="sxs-lookup"><span data-stu-id="0520f-111">unknown</span></span>|<span data-ttu-id="0520f-112">.0</span><span class="sxs-lookup"><span data-stu-id="0520f-112">0</span></span>|<span data-ttu-id="0520f-113">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="0520f-113">Default state.</span></span>|
|<span data-ttu-id="0520f-114">有効な</span><span class="sxs-lookup"><span data-stu-id="0520f-114">valid</span></span>|<span data-ttu-id="0520f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="0520f-115">1</span></span>|<span data-ttu-id="0520f-116">トークンが有効です。</span><span class="sxs-lookup"><span data-stu-id="0520f-116">Token is valid.</span></span>|
|<span data-ttu-id="0520f-117">終了</span><span class="sxs-lookup"><span data-stu-id="0520f-117">expired</span></span>|<span data-ttu-id="0520f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0520f-118">2</span></span>|<span data-ttu-id="0520f-119">トークンの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="0520f-119">Token is expired.</span></span>|
|<span data-ttu-id="0520f-120">無効です</span><span class="sxs-lookup"><span data-stu-id="0520f-120">invalid</span></span>|<span data-ttu-id="0520f-121">1/3</span><span class="sxs-lookup"><span data-stu-id="0520f-121">3</span></span>|<span data-ttu-id="0520f-122">トークンが無効です。</span><span class="sxs-lookup"><span data-stu-id="0520f-122">Token is invalid.</span></span>|
|<span data-ttu-id="0520f-123">assignedToExternalMDM</span><span class="sxs-lookup"><span data-stu-id="0520f-123">assignedToExternalMDM</span></span>|<span data-ttu-id="0520f-124">2/4</span><span class="sxs-lookup"><span data-stu-id="0520f-124">4</span></span>|<span data-ttu-id="0520f-125">トークンは別の MDM サービスによって管理されています。</span><span class="sxs-lookup"><span data-stu-id="0520f-125">Token is managed by another MDM Service.</span></span>|





