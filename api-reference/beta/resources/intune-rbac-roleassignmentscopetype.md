---
title: roleAssignmentScopeType 列挙型
description: 役割の割り当てのスコープの種類を指定します。
ms.openlocfilehash: dcfac7b345dde2d8f107b8ec756d017966a6a94a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071698"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="1cf24-103">roleAssignmentScopeType 列挙型</span><span class="sxs-lookup"><span data-stu-id="1cf24-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="1cf24-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1cf24-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1cf24-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1cf24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1cf24-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1cf24-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1cf24-107">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="1cf24-107">Specifies the type of scope for a Role Assignment.</span></span>
## <a name="members"></a><span data-ttu-id="1cf24-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1cf24-108">Members</span></span>
|<span data-ttu-id="1cf24-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="1cf24-109">Member</span></span>|<span data-ttu-id="1cf24-110">値</span><span class="sxs-lookup"><span data-stu-id="1cf24-110">Value</span></span>|<span data-ttu-id="1cf24-111">説明</span><span class="sxs-lookup"><span data-stu-id="1cf24-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1cf24-112">resourceScope</span><span class="sxs-lookup"><span data-stu-id="1cf24-112">resourceScope</span></span>|<span data-ttu-id="1cf24-113">0</span><span class="sxs-lookup"><span data-stu-id="1cf24-113">0</span></span>|<span data-ttu-id="1cf24-114">指定された ResourceScopes への割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="1cf24-114">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="1cf24-115">しています。</span><span class="sxs-lookup"><span data-stu-id="1cf24-115">allDevices</span></span>|<span data-ttu-id="1cf24-116">1</span><span class="sxs-lookup"><span data-stu-id="1cf24-116">1</span></span>|<span data-ttu-id="1cf24-117">Intune のすべてのデバイスへの割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="1cf24-117">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="1cf24-118">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="1cf24-118">allLicensedUsers</span></span>|<span data-ttu-id="1cf24-119">2</span><span class="sxs-lookup"><span data-stu-id="1cf24-119">2</span></span>|<span data-ttu-id="1cf24-120">Intune にライセンスのすべてのユーザーへの割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="1cf24-120">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="1cf24-121">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="1cf24-121">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="1cf24-122">3</span><span class="sxs-lookup"><span data-stu-id="1cf24-122">3</span></span>|<span data-ttu-id="1cf24-123">Intune デバイスおよびライセンスを受けたユーザーのすべての割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="1cf24-123">Allow assignments to all Intune devices and licensed users.</span></span>|





