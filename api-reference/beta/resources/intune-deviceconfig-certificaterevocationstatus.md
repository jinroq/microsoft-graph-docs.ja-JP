---
title: certificateRevocationStatus 列挙型
description: 証明書の失効状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4544968e473c41d787df606112801c9b60e2cb98
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947429"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="df7d0-103">certificateRevocationStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="df7d0-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="df7d0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df7d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df7d0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="df7d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df7d0-106">証明書の失効状態。</span><span class="sxs-lookup"><span data-stu-id="df7d0-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="df7d0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="df7d0-107">Members</span></span>
|<span data-ttu-id="df7d0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="df7d0-108">Member</span></span>|<span data-ttu-id="df7d0-109">値</span><span class="sxs-lookup"><span data-stu-id="df7d0-109">Value</span></span>|<span data-ttu-id="df7d0-110">説明</span><span class="sxs-lookup"><span data-stu-id="df7d0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df7d0-111">none</span><span class="sxs-lookup"><span data-stu-id="df7d0-111">none</span></span>|<span data-ttu-id="df7d0-112">.0</span><span class="sxs-lookup"><span data-stu-id="df7d0-112">0</span></span>|<span data-ttu-id="df7d0-113">取り消されません。</span><span class="sxs-lookup"><span data-stu-id="df7d0-113">Not revoked.</span></span>|
|<span data-ttu-id="df7d0-114">対する</span><span class="sxs-lookup"><span data-stu-id="df7d0-114">pending</span></span>|<span data-ttu-id="df7d0-115">1-d</span><span class="sxs-lookup"><span data-stu-id="df7d0-115">1</span></span>|<span data-ttu-id="df7d0-116">失効が保留中です。</span><span class="sxs-lookup"><span data-stu-id="df7d0-116">Revocation pending.</span></span>|
|<span data-ttu-id="df7d0-117">発行</span><span class="sxs-lookup"><span data-stu-id="df7d0-117">issued</span></span>|<span data-ttu-id="df7d0-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="df7d0-118">2</span></span>|<span data-ttu-id="df7d0-119">失効コマンドが発行されました。</span><span class="sxs-lookup"><span data-stu-id="df7d0-119">Revocation command issued.</span></span>|
|<span data-ttu-id="df7d0-120">フェール</span><span class="sxs-lookup"><span data-stu-id="df7d0-120">failed</span></span>|<span data-ttu-id="df7d0-121">1/3</span><span class="sxs-lookup"><span data-stu-id="df7d0-121">3</span></span>|<span data-ttu-id="df7d0-122">取り消しに失敗しました。</span><span class="sxs-lookup"><span data-stu-id="df7d0-122">Revocation failed.</span></span>|
|<span data-ttu-id="df7d0-123">破棄</span><span class="sxs-lookup"><span data-stu-id="df7d0-123">revoked</span></span>|<span data-ttu-id="df7d0-124">2/4</span><span class="sxs-lookup"><span data-stu-id="df7d0-124">4</span></span>|<span data-ttu-id="df7d0-125">破棄.</span><span class="sxs-lookup"><span data-stu-id="df7d0-125">Revoked.</span></span>|




