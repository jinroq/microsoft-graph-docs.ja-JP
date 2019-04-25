---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有 PC でアカウントを削除する場合に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c547a59c02e3c4cad9bd8140a2e11ca6e3c84a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534620"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="e3136-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e3136-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="e3136-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3136-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3136-105">共有 PC でアカウントを削除する場合に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="e3136-105">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="e3136-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e3136-106">Members</span></span>
|<span data-ttu-id="e3136-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e3136-107">Member</span></span>|<span data-ttu-id="e3136-108">値</span><span class="sxs-lookup"><span data-stu-id="e3136-108">Value</span></span>|<span data-ttu-id="e3136-109">説明</span><span class="sxs-lookup"><span data-stu-id="e3136-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3136-110">瞬時</span><span class="sxs-lookup"><span data-stu-id="e3136-110">immediate</span></span>|<span data-ttu-id="e3136-111">.0</span><span class="sxs-lookup"><span data-stu-id="e3136-111">0</span></span>|<span data-ttu-id="e3136-112">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="e3136-112">Delete immediately.</span></span>|
|<span data-ttu-id="e3136-113">ディスクスペースしきい値</span><span class="sxs-lookup"><span data-stu-id="e3136-113">diskSpaceThreshold</span></span>|<span data-ttu-id="e3136-114">1 </span><span class="sxs-lookup"><span data-stu-id="e3136-114">1</span></span>|<span data-ttu-id="e3136-115">ディスク容量のしきい値で削除します。</span><span class="sxs-lookup"><span data-stu-id="e3136-115">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="e3136-116">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="e3136-116">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="e3136-117">2 </span><span class="sxs-lookup"><span data-stu-id="e3136-117">2</span></span>|<span data-ttu-id="e3136-118">ディスク容量のしきい値または非アクティブなしきい値での削除。</span><span class="sxs-lookup"><span data-stu-id="e3136-118">Delete at disk space threshold or inactive threshold.</span></span>|



