---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有 PC でアカウントを削除する場合に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6db021476afdc47129fd677702bc6cc58af204fd
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787128"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="62eda-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="62eda-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="62eda-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="62eda-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62eda-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="62eda-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62eda-106">共有 PC でアカウントを削除する場合に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="62eda-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="62eda-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="62eda-107">Members</span></span>
|<span data-ttu-id="62eda-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="62eda-108">Member</span></span>|<span data-ttu-id="62eda-109">値</span><span class="sxs-lookup"><span data-stu-id="62eda-109">Value</span></span>|<span data-ttu-id="62eda-110">説明</span><span class="sxs-lookup"><span data-stu-id="62eda-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62eda-111">瞬時</span><span class="sxs-lookup"><span data-stu-id="62eda-111">immediate</span></span>|<span data-ttu-id="62eda-112">.0</span><span class="sxs-lookup"><span data-stu-id="62eda-112">0</span></span>|<span data-ttu-id="62eda-113">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="62eda-113">Delete immediately.</span></span>|
|<span data-ttu-id="62eda-114">ディスクスペースしきい値</span><span class="sxs-lookup"><span data-stu-id="62eda-114">diskSpaceThreshold</span></span>|<span data-ttu-id="62eda-115">1-d</span><span class="sxs-lookup"><span data-stu-id="62eda-115">1</span></span>|<span data-ttu-id="62eda-116">ディスク容量のしきい値で削除します。</span><span class="sxs-lookup"><span data-stu-id="62eda-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="62eda-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="62eda-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="62eda-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="62eda-118">2</span></span>|<span data-ttu-id="62eda-119">ディスク容量のしきい値または非アクティブなしきい値での削除。</span><span class="sxs-lookup"><span data-stu-id="62eda-119">Delete at disk space threshold or inactive threshold.</span></span>|





