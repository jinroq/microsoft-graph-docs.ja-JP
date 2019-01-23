---
title: sharedPCAccountDeletionPolicyType 列挙型
description: 共有の PC でアカウントが削除されたときに指定できる値です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 645cd3dfd4121c6c9bdd9d57a0dc3b63723cc461
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415167"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="4945a-103">sharedPCAccountDeletionPolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4945a-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="4945a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4945a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4945a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4945a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4945a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4945a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4945a-107">共有の PC でアカウントが削除されたときに指定できる値です。</span><span class="sxs-lookup"><span data-stu-id="4945a-107">Possible values for when accounts are deleted on a shared PC.</span></span>

## <a name="members"></a><span data-ttu-id="4945a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4945a-108">Members</span></span>
|<span data-ttu-id="4945a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4945a-109">Member</span></span>|<span data-ttu-id="4945a-110">値</span><span class="sxs-lookup"><span data-stu-id="4945a-110">Value</span></span>|<span data-ttu-id="4945a-111">説明</span><span class="sxs-lookup"><span data-stu-id="4945a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4945a-112">イミディ エイト</span><span class="sxs-lookup"><span data-stu-id="4945a-112">immediate</span></span>|<span data-ttu-id="4945a-113">0</span><span class="sxs-lookup"><span data-stu-id="4945a-113">0</span></span>|<span data-ttu-id="4945a-114">すぐに削除します。</span><span class="sxs-lookup"><span data-stu-id="4945a-114">Delete immediately.</span></span>|
|<span data-ttu-id="4945a-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="4945a-115">diskSpaceThreshold</span></span>|<span data-ttu-id="4945a-116">1</span><span class="sxs-lookup"><span data-stu-id="4945a-116">1</span></span>|<span data-ttu-id="4945a-117">ディスク容量のしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="4945a-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="4945a-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="4945a-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="4945a-119">2</span><span class="sxs-lookup"><span data-stu-id="4945a-119">2</span></span>|<span data-ttu-id="4945a-120">ディスク容量のしきい値または非アクティブのしきい値を削除します。</span><span class="sxs-lookup"><span data-stu-id="4945a-120">Delete at disk space threshold or inactive threshold.</span></span>|




