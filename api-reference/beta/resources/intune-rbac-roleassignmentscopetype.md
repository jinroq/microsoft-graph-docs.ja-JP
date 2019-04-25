---
title: roleAssignmentScopeType 列挙型
description: 役割の割り当てのスコープの種類を指定します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d9659c4eaa1f4080ef5dd07a5e69f76a7a14d50
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573054"
---
# <a name="roleassignmentscopetype-enum-type"></a><span data-ttu-id="74f22-103">roleAssignmentScopeType 列挙型</span><span class="sxs-lookup"><span data-stu-id="74f22-103">roleAssignmentScopeType enum type</span></span>

> <span data-ttu-id="74f22-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74f22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74f22-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="74f22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74f22-106">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="74f22-106">Specifies the type of scope for a Role Assignment.</span></span>

## <a name="members"></a><span data-ttu-id="74f22-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="74f22-107">Members</span></span>
|<span data-ttu-id="74f22-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="74f22-108">Member</span></span>|<span data-ttu-id="74f22-109">値</span><span class="sxs-lookup"><span data-stu-id="74f22-109">Value</span></span>|<span data-ttu-id="74f22-110">説明</span><span class="sxs-lookup"><span data-stu-id="74f22-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74f22-111">resourcescope</span><span class="sxs-lookup"><span data-stu-id="74f22-111">resourceScope</span></span>|<span data-ttu-id="74f22-112">.0</span><span class="sxs-lookup"><span data-stu-id="74f22-112">0</span></span>|<span data-ttu-id="74f22-113">指定した ResourceScopes への割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="74f22-113">Allow assignments to the specified ResourceScopes.</span></span>|
|<span data-ttu-id="74f22-114">alldevices</span><span class="sxs-lookup"><span data-stu-id="74f22-114">allDevices</span></span>|<span data-ttu-id="74f22-115">1 </span><span class="sxs-lookup"><span data-stu-id="74f22-115">1</span></span>|<span data-ttu-id="74f22-116">すべての Intune デバイスへの割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="74f22-116">Allow assignments to all Intune devices.</span></span>|
|<span data-ttu-id="74f22-117">allLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="74f22-117">allLicensedUsers</span></span>|<span data-ttu-id="74f22-118">2 </span><span class="sxs-lookup"><span data-stu-id="74f22-118">2</span></span>|<span data-ttu-id="74f22-119">Intune にライセンスされたすべてのユーザーへの割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="74f22-119">Allow assignments to all Intune licensed users.</span></span>|
|<span data-ttu-id="74f22-120">allDevicesAndLicensedUsers</span><span class="sxs-lookup"><span data-stu-id="74f22-120">allDevicesAndLicensedUsers</span></span>|<span data-ttu-id="74f22-121">3 </span><span class="sxs-lookup"><span data-stu-id="74f22-121">3</span></span>|<span data-ttu-id="74f22-122">すべての Intune デバイスおよびライセンスされたユーザーへの割り当てを許可します。</span><span class="sxs-lookup"><span data-stu-id="74f22-122">Allow assignments to all Intune devices and licensed users.</span></span>|





