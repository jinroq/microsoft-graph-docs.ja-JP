---
title: certificateRevocationStatus 列挙型
description: 証明書の失効状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ef7181707e6e80c9ad816f345f2a299dbce147e7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990114"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="17077-103">certificateRevocationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="17077-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="17077-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17077-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17077-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="17077-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17077-106">証明書の失効状態。</span><span class="sxs-lookup"><span data-stu-id="17077-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="17077-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="17077-107">Members</span></span>
|<span data-ttu-id="17077-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="17077-108">Member</span></span>|<span data-ttu-id="17077-109">値</span><span class="sxs-lookup"><span data-stu-id="17077-109">Value</span></span>|<span data-ttu-id="17077-110">説明</span><span class="sxs-lookup"><span data-stu-id="17077-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17077-111">none</span><span class="sxs-lookup"><span data-stu-id="17077-111">none</span></span>|<span data-ttu-id="17077-112">.0</span><span class="sxs-lookup"><span data-stu-id="17077-112">0</span></span>|<span data-ttu-id="17077-113">取り消されません。</span><span class="sxs-lookup"><span data-stu-id="17077-113">Not revoked.</span></span>|
|<span data-ttu-id="17077-114">対する</span><span class="sxs-lookup"><span data-stu-id="17077-114">pending</span></span>|<span data-ttu-id="17077-115">1-d</span><span class="sxs-lookup"><span data-stu-id="17077-115">1</span></span>|<span data-ttu-id="17077-116">失効が保留中です。</span><span class="sxs-lookup"><span data-stu-id="17077-116">Revocation pending.</span></span>|
|<span data-ttu-id="17077-117">発行</span><span class="sxs-lookup"><span data-stu-id="17077-117">issued</span></span>|<span data-ttu-id="17077-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="17077-118">2</span></span>|<span data-ttu-id="17077-119">失効コマンドが発行されました。</span><span class="sxs-lookup"><span data-stu-id="17077-119">Revocation command issued.</span></span>|
|<span data-ttu-id="17077-120">フェール</span><span class="sxs-lookup"><span data-stu-id="17077-120">failed</span></span>|<span data-ttu-id="17077-121">1/3</span><span class="sxs-lookup"><span data-stu-id="17077-121">3</span></span>|<span data-ttu-id="17077-122">取り消しに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="17077-122">Revocation failed.</span></span>|
|<span data-ttu-id="17077-123">破棄</span><span class="sxs-lookup"><span data-stu-id="17077-123">revoked</span></span>|<span data-ttu-id="17077-124">2/4</span><span class="sxs-lookup"><span data-stu-id="17077-124">4</span></span>|<span data-ttu-id="17077-125">破棄.</span><span class="sxs-lookup"><span data-stu-id="17077-125">Revoked.</span></span>|





