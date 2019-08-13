---
title: roleAssignmentScopeType 列挙型
description: 役割の割り当てのスコープの種類を指定します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 6699af01c2e2a2e03e0d5ef00cce0fb572d8c57d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369242"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="6df20-103">roleAssignmentScopeType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6df20-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="6df20-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6df20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6df20-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6df20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6df20-106">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="6df20-106">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="6df20-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6df20-107">Members</span></span>
|<span data-ttu-id="6df20-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6df20-108">Member</span></span>|<span data-ttu-id="6df20-109">値</span><span class="sxs-lookup"><span data-stu-id="6df20-109">Value</span></span>|<span data-ttu-id="6df20-110">説明</span><span class="sxs-lookup"><span data-stu-id="6df20-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6df20-111">resourceScope</span><span class="sxs-lookup"><span data-stu-id="6df20-111">resourceScope</span></span>|<span data-ttu-id="6df20-112">.0</span><span class="sxs-lookup"><span data-stu-id="6df20-112">0</span></span>|<span data-ttu-id="6df20-113">指定した ResourceScopes への割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="6df20-113">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="6df20-114">allDevices</span><span class="sxs-lookup"><span data-stu-id="6df20-114">allDevices</span></span>|<span data-ttu-id="6df20-115">1-d</span><span class="sxs-lookup"><span data-stu-id="6df20-115">1</span></span>|<span data-ttu-id="6df20-116">すべての Intune デバイスへの割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="6df20-116">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="6df20-117">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="6df20-117">allLicensedUsers</span></span>|<span data-ttu-id="6df20-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="6df20-118">2</span></span>|<span data-ttu-id="6df20-119">Intune にライセンスされたすべてのユーザーへの割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="6df20-119">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="6df20-120">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="6df20-120">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="6df20-121">1/3</span><span class="sxs-lookup"><span data-stu-id="6df20-121">3</span></span>|<span data-ttu-id="6df20-122">すべての Intune デバイスおよびライセンスされたユーザーへの割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="6df20-122">Allow assignments to all Intune devices and licensed users.</span></span>|



