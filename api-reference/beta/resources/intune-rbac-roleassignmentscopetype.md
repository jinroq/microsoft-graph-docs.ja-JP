---
title: roleAssignmentScopeType 列挙型
description: 役割の割り当てのスコープの種類を指定します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b815cf7eb396aa82f49df792ceee0612678077c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419892"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="fc90a-103">roleAssignmentScopeType 列挙型</span><span class="sxs-lookup"><span data-stu-id="fc90a-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="fc90a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fc90a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fc90a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc90a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc90a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fc90a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc90a-107">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="fc90a-107">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="fc90a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="fc90a-108">Members</span></span>
|<span data-ttu-id="fc90a-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="fc90a-109">Member</span></span>|<span data-ttu-id="fc90a-110">値</span><span class="sxs-lookup"><span data-stu-id="fc90a-110">Value</span></span>|<span data-ttu-id="fc90a-111">説明</span><span class="sxs-lookup"><span data-stu-id="fc90a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc90a-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="fc90a-112">resourceScope</span></span>|<span data-ttu-id="fc90a-113">0</span><span class="sxs-lookup"><span data-stu-id="fc90a-113">0</span></span>|<span data-ttu-id="fc90a-114">指定された ResourceScopes への割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="fc90a-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="fc90a-115">しています。</span><span class="sxs-lookup"><span data-stu-id="fc90a-115">allDevices</span></span>|<span data-ttu-id="fc90a-116">1</span><span class="sxs-lookup"><span data-stu-id="fc90a-116">1</span></span>|<span data-ttu-id="fc90a-117">Intune のすべてのデバイスへの割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="fc90a-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="fc90a-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="fc90a-118">allLicensedUsers</span></span>|<span data-ttu-id="fc90a-119">2</span><span class="sxs-lookup"><span data-stu-id="fc90a-119">2</span></span>|<span data-ttu-id="fc90a-120">Intune にライセンスのすべてのユーザーへの割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="fc90a-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="fc90a-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="fc90a-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="fc90a-122">3</span><span class="sxs-lookup"><span data-stu-id="fc90a-122">3</span></span>|<span data-ttu-id="fc90a-123">Intune デバイスおよびライセンスを受けたユーザーのすべての割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="fc90a-123">Allow assignments to all Intune devices and licensed users.</span></span>|




