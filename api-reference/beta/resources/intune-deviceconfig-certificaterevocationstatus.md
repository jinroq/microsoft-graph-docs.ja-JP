---
title: certificateRevocationStatus 列挙型
description: 証明書の失効状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5fd9a6cd34df322a057d16e3d803d8685f7cd173
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782808"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="060a2-103">certificateRevocationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="060a2-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="060a2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="060a2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="060a2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="060a2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="060a2-106">証明書の失効状態。</span><span class="sxs-lookup"><span data-stu-id="060a2-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="060a2-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="060a2-107">Members</span></span>
|<span data-ttu-id="060a2-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="060a2-108">Member</span></span>|<span data-ttu-id="060a2-109">値</span><span class="sxs-lookup"><span data-stu-id="060a2-109">Value</span></span>|<span data-ttu-id="060a2-110">説明</span><span class="sxs-lookup"><span data-stu-id="060a2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="060a2-111">none</span><span class="sxs-lookup"><span data-stu-id="060a2-111">none</span></span>|<span data-ttu-id="060a2-112">.0</span><span class="sxs-lookup"><span data-stu-id="060a2-112">0</span></span>|<span data-ttu-id="060a2-113">取り消されません。</span><span class="sxs-lookup"><span data-stu-id="060a2-113">Not revoked.</span></span>|
|<span data-ttu-id="060a2-114">対する</span><span class="sxs-lookup"><span data-stu-id="060a2-114">pending</span></span>|<span data-ttu-id="060a2-115">1-d</span><span class="sxs-lookup"><span data-stu-id="060a2-115">1</span></span>|<span data-ttu-id="060a2-116">失効が保留中です。</span><span class="sxs-lookup"><span data-stu-id="060a2-116">Revocation pending.</span></span>|
|<span data-ttu-id="060a2-117">発行</span><span class="sxs-lookup"><span data-stu-id="060a2-117">issued</span></span>|<span data-ttu-id="060a2-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="060a2-118">2</span></span>|<span data-ttu-id="060a2-119">失効コマンドが発行されました。</span><span class="sxs-lookup"><span data-stu-id="060a2-119">Revocation command issued.</span></span>|
|<span data-ttu-id="060a2-120">フェール</span><span class="sxs-lookup"><span data-stu-id="060a2-120">failed</span></span>|<span data-ttu-id="060a2-121">1/3</span><span class="sxs-lookup"><span data-stu-id="060a2-121">3</span></span>|<span data-ttu-id="060a2-122">取り消しに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="060a2-122">Revocation failed.</span></span>|
|<span data-ttu-id="060a2-123">破棄</span><span class="sxs-lookup"><span data-stu-id="060a2-123">revoked</span></span>|<span data-ttu-id="060a2-124">2/4</span><span class="sxs-lookup"><span data-stu-id="060a2-124">4</span></span>|<span data-ttu-id="060a2-125">破棄.</span><span class="sxs-lookup"><span data-stu-id="060a2-125">Revoked.</span></span>|





