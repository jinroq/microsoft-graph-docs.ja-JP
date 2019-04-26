---
title: actionstate 列挙型
description: デバイス上のアクションの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e06b492e41ffa5e2f9aa4b64782e96125ea746a2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548461"
---
# <a name="actionstate-enum-type"></a><span data-ttu-id="8f369-103">actionstate 列挙型</span><span class="sxs-lookup"><span data-stu-id="8f369-103">actionState enum type</span></span>

> <span data-ttu-id="8f369-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8f369-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f369-105">デバイス上のアクションの状態</span><span class="sxs-lookup"><span data-stu-id="8f369-105">State of the action on the device</span></span>

## <a name="members"></a><span data-ttu-id="8f369-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="8f369-106">Members</span></span>
|<span data-ttu-id="8f369-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="8f369-107">Member</span></span>|<span data-ttu-id="8f369-108">値</span><span class="sxs-lookup"><span data-stu-id="8f369-108">Value</span></span>|<span data-ttu-id="8f369-109">説明</span><span class="sxs-lookup"><span data-stu-id="8f369-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f369-110">なし</span><span class="sxs-lookup"><span data-stu-id="8f369-110">none</span></span>|<span data-ttu-id="8f369-111">.0</span><span class="sxs-lookup"><span data-stu-id="8f369-111">0</span></span>|<span data-ttu-id="8f369-112">有効なアクション状態ではありません</span><span class="sxs-lookup"><span data-stu-id="8f369-112">Not a valid action state</span></span>|
|<span data-ttu-id="8f369-113">対する</span><span class="sxs-lookup"><span data-stu-id="8f369-113">pending</span></span>|<span data-ttu-id="8f369-114">1 </span><span class="sxs-lookup"><span data-stu-id="8f369-114">1</span></span>|<span data-ttu-id="8f369-115">アクションが保留中</span><span class="sxs-lookup"><span data-stu-id="8f369-115">Action is pending</span></span>|
|<span data-ttu-id="8f369-116">取り消す</span><span class="sxs-lookup"><span data-stu-id="8f369-116">canceled</span></span>|<span data-ttu-id="8f369-117">2 </span><span class="sxs-lookup"><span data-stu-id="8f369-117">2</span></span>|<span data-ttu-id="8f369-118">アクションが取り消されました。</span><span class="sxs-lookup"><span data-stu-id="8f369-118">Action has been cancelled.</span></span>|
|<span data-ttu-id="8f369-119">active</span><span class="sxs-lookup"><span data-stu-id="8f369-119">active</span></span>|<span data-ttu-id="8f369-120">3 </span><span class="sxs-lookup"><span data-stu-id="8f369-120">3</span></span>|<span data-ttu-id="8f369-121">アクションはアクティブです。</span><span class="sxs-lookup"><span data-stu-id="8f369-121">Action is active.</span></span>|
|<span data-ttu-id="8f369-122">done</span><span class="sxs-lookup"><span data-stu-id="8f369-122">done</span></span>|<span data-ttu-id="8f369-123">4 </span><span class="sxs-lookup"><span data-stu-id="8f369-123">4</span></span>|<span data-ttu-id="8f369-124">操作はエラーなしで完了しました。</span><span class="sxs-lookup"><span data-stu-id="8f369-124">Action completed without errors.</span></span>|
|<span data-ttu-id="8f369-125">フェール</span><span class="sxs-lookup"><span data-stu-id="8f369-125">failed</span></span>|<span data-ttu-id="8f369-126">5 </span><span class="sxs-lookup"><span data-stu-id="8f369-126">5</span></span>|<span data-ttu-id="8f369-127">アクションの失敗</span><span class="sxs-lookup"><span data-stu-id="8f369-127">Action failed</span></span>|
|<span data-ttu-id="8f369-128">notSupported</span><span class="sxs-lookup"><span data-stu-id="8f369-128">notSupported</span></span>|<span data-ttu-id="8f369-129">6 </span><span class="sxs-lookup"><span data-stu-id="8f369-129">6</span></span>|<span data-ttu-id="8f369-130">アクションはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f369-130">Action is not supported.</span></span>|



