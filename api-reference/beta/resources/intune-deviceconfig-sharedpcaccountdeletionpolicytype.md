---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有 PC でアカウントを削除する場合に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9d94233233577d22a8c3661fb6e2ce82408d2a9
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139936"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="e1a67-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e1a67-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="e1a67-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1a67-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1a67-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e1a67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1a67-106">共有 PC でアカウントを削除する場合に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="e1a67-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="e1a67-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e1a67-107">Members</span></span>
|<span data-ttu-id="e1a67-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e1a67-108">Member</span></span>|<span data-ttu-id="e1a67-109">値</span><span class="sxs-lookup"><span data-stu-id="e1a67-109">Value</span></span>|<span data-ttu-id="e1a67-110">説明</span><span class="sxs-lookup"><span data-stu-id="e1a67-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1a67-111">瞬時</span><span class="sxs-lookup"><span data-stu-id="e1a67-111">immediate</span></span>|<span data-ttu-id="e1a67-112">.0</span><span class="sxs-lookup"><span data-stu-id="e1a67-112">0</span></span>|<span data-ttu-id="e1a67-113">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="e1a67-113">Delete immediately.</span></span>|
|<span data-ttu-id="e1a67-114">ディスクスペースしきい値</span><span class="sxs-lookup"><span data-stu-id="e1a67-114">diskSpaceThreshold</span></span>|<span data-ttu-id="e1a67-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e1a67-115">1</span></span>|<span data-ttu-id="e1a67-116">ディスク容量のしきい値で削除します。</span><span class="sxs-lookup"><span data-stu-id="e1a67-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="e1a67-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="e1a67-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="e1a67-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e1a67-118">2</span></span>|<span data-ttu-id="e1a67-119">ディスク容量のしきい値または非アクティブなしきい値での削除。</span><span class="sxs-lookup"><span data-stu-id="e1a67-119">Delete at disk space threshold or inactive threshold.</span></span>|




