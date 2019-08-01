---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有 PC でアカウントを削除する場合に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: da4f053301206143cf6ee617a6818ea57ddab3d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027826"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="97bd8-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="97bd8-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="97bd8-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="97bd8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97bd8-105">共有 PC でアカウントを削除する場合に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="97bd8-105">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="97bd8-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="97bd8-106">Members</span></span>
|<span data-ttu-id="97bd8-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="97bd8-107">Member</span></span>|<span data-ttu-id="97bd8-108">値</span><span class="sxs-lookup"><span data-stu-id="97bd8-108">Value</span></span>|<span data-ttu-id="97bd8-109">説明</span><span class="sxs-lookup"><span data-stu-id="97bd8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97bd8-110">瞬時</span><span class="sxs-lookup"><span data-stu-id="97bd8-110">immediate</span></span>|<span data-ttu-id="97bd8-111">.0</span><span class="sxs-lookup"><span data-stu-id="97bd8-111">0</span></span>|<span data-ttu-id="97bd8-112">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="97bd8-112">Delete immediately.</span></span>|
|<span data-ttu-id="97bd8-113">ディスクスペースしきい値</span><span class="sxs-lookup"><span data-stu-id="97bd8-113">diskSpaceThreshold</span></span>|<span data-ttu-id="97bd8-114">1-d</span><span class="sxs-lookup"><span data-stu-id="97bd8-114">1</span></span>|<span data-ttu-id="97bd8-115">ディスク容量のしきい値で削除します。</span><span class="sxs-lookup"><span data-stu-id="97bd8-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="97bd8-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="97bd8-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="97bd8-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="97bd8-117">2</span></span>|<span data-ttu-id="97bd8-118">ディスク容量のしきい値または非アクティブなしきい値での削除。</span><span class="sxs-lookup"><span data-stu-id="97bd8-118">Delete at disk space threshold or inactive threshold.</span></span>|



