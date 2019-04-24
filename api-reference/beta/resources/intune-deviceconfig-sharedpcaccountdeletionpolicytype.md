---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有 PC でアカウントを削除する場合に使用できる値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6db021476afdc47129fd677702bc6cc58af204fd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464951"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="f798b-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="f798b-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="f798b-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f798b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f798b-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f798b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f798b-106">共有 PC でアカウントを削除する場合に使用できる値。</span><span class="sxs-lookup"><span data-stu-id="f798b-106">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="f798b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="f798b-107">Members</span></span>
|<span data-ttu-id="f798b-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="f798b-108">Member</span></span>|<span data-ttu-id="f798b-109">値</span><span class="sxs-lookup"><span data-stu-id="f798b-109">Value</span></span>|<span data-ttu-id="f798b-110">説明</span><span class="sxs-lookup"><span data-stu-id="f798b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f798b-111">瞬時</span><span class="sxs-lookup"><span data-stu-id="f798b-111">immediate</span></span>|<span data-ttu-id="f798b-112">.0</span><span class="sxs-lookup"><span data-stu-id="f798b-112">0</span></span>|<span data-ttu-id="f798b-113">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="f798b-113">Delete immediately.</span></span>|
|<span data-ttu-id="f798b-114">ディスクスペースしきい値</span><span class="sxs-lookup"><span data-stu-id="f798b-114">diskSpaceThreshold</span></span>|<span data-ttu-id="f798b-115">1-d</span><span class="sxs-lookup"><span data-stu-id="f798b-115">1</span></span>|<span data-ttu-id="f798b-116">ディスク容量のしきい値で削除します。</span><span class="sxs-lookup"><span data-stu-id="f798b-116">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="f798b-117">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="f798b-117">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="f798b-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="f798b-118">2</span></span>|<span data-ttu-id="f798b-119">ディスク容量のしきい値または非アクティブなしきい値での削除。</span><span class="sxs-lookup"><span data-stu-id="f798b-119">Delete at disk space threshold or inactive threshold.</span></span>|





