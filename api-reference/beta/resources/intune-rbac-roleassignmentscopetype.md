---
title: roleAssignmentScopeType 列挙型
description: 役割の割り当てのスコープの種類を指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6089021851e3d953fce4874b11e343b4747adf40
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150695"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="bfd45-103">roleAssignmentScopeType 列挙型</span><span class="sxs-lookup"><span data-stu-id="bfd45-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="bfd45-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bfd45-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bfd45-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bfd45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bfd45-106">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="bfd45-106">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="bfd45-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="bfd45-107">Members</span></span>
|<span data-ttu-id="bfd45-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="bfd45-108">Member</span></span>|<span data-ttu-id="bfd45-109">値</span><span class="sxs-lookup"><span data-stu-id="bfd45-109">Value</span></span>|<span data-ttu-id="bfd45-110">説明</span><span class="sxs-lookup"><span data-stu-id="bfd45-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bfd45-111">resourcescope</span><span class="sxs-lookup"><span data-stu-id="bfd45-111">resourceScope</span></span>|<span data-ttu-id="bfd45-112">.0</span><span class="sxs-lookup"><span data-stu-id="bfd45-112">0</span></span>|<span data-ttu-id="bfd45-113">指定した ResourceScopes への割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="bfd45-113">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="bfd45-114">alldevices</span><span class="sxs-lookup"><span data-stu-id="bfd45-114">allDevices</span></span>|<span data-ttu-id="bfd45-115">1-d</span><span class="sxs-lookup"><span data-stu-id="bfd45-115">1</span></span>|<span data-ttu-id="bfd45-116">すべての Intune デバイスへの割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="bfd45-116">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="bfd45-117">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="bfd45-117">allLicensedUsers</span></span>|<span data-ttu-id="bfd45-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="bfd45-118">2</span></span>|<span data-ttu-id="bfd45-119">Intune にライセンスされたすべてのユーザーへの割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="bfd45-119">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="bfd45-120">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="bfd45-120">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="bfd45-121">1/3</span><span class="sxs-lookup"><span data-stu-id="bfd45-121">3</span></span>|<span data-ttu-id="bfd45-122">すべての Intune デバイスおよびライセンスされたユーザーへの割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="bfd45-122">Allow assignments to all Intune devices and licensed users.</span></span>|




