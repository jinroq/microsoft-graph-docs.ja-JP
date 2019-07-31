---
title: userPfxIntendedPurpose 列挙型
description: ユーザー PFX 証明書の目的のためにサポートされている値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 473f06515b1cb9a1eee966a471c8a8adb81aca7d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010610"
---
# <a name="userpfxintendedpurpose-enum-type"></a><span data-ttu-id="fc2e1-103">userPfxIntendedPurpose 列挙型</span><span class="sxs-lookup"><span data-stu-id="fc2e1-103">userPfxIntendedPurpose enum type</span></span>

> <span data-ttu-id="fc2e1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc2e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc2e1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fc2e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc2e1-106">ユーザー PFX 証明書の目的のためにサポートされている値。</span><span class="sxs-lookup"><span data-stu-id="fc2e1-106">Supported values for the intended purpose of a user PFX certificate.</span></span>

## <a name="members"></a><span data-ttu-id="fc2e1-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="fc2e1-107">Members</span></span>
|<span data-ttu-id="fc2e1-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="fc2e1-108">Member</span></span>|<span data-ttu-id="fc2e1-109">値</span><span class="sxs-lookup"><span data-stu-id="fc2e1-109">Value</span></span>|<span data-ttu-id="fc2e1-110">説明</span><span class="sxs-lookup"><span data-stu-id="fc2e1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc2e1-111">未定義</span><span class="sxs-lookup"><span data-stu-id="fc2e1-111">unassigned</span></span>|<span data-ttu-id="fc2e1-112">.0</span><span class="sxs-lookup"><span data-stu-id="fc2e1-112">0</span></span>|<span data-ttu-id="fc2e1-113">役割/使用状況は割り当てられていません。</span><span class="sxs-lookup"><span data-stu-id="fc2e1-113">No roles/usages assigned.</span></span>|
|<span data-ttu-id="fc2e1-114">smimeEncryption</span><span class="sxs-lookup"><span data-stu-id="fc2e1-114">smimeEncryption</span></span>|<span data-ttu-id="fc2e1-115">1-d</span><span class="sxs-lookup"><span data-stu-id="fc2e1-115">1</span></span>|<span data-ttu-id="fc2e1-116">S/MIME 暗号化に対して有効です。</span><span class="sxs-lookup"><span data-stu-id="fc2e1-116">Valid for S/MIME encryption.</span></span>|
|<span data-ttu-id="fc2e1-117">smimeSigning</span><span class="sxs-lookup"><span data-stu-id="fc2e1-117">smimeSigning</span></span>|<span data-ttu-id="fc2e1-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="fc2e1-118">2</span></span>|<span data-ttu-id="fc2e1-119">S/MIME 署名に対して有効です。</span><span class="sxs-lookup"><span data-stu-id="fc2e1-119">Valid for S/MIME signing.</span></span>|
|<span data-ttu-id="fc2e1-120">仮想</span><span class="sxs-lookup"><span data-stu-id="fc2e1-120">vpn</span></span>|<span data-ttu-id="fc2e1-121">2/4</span><span class="sxs-lookup"><span data-stu-id="fc2e1-121">4</span></span>|<span data-ttu-id="fc2e1-122">VPN で使用する場合に有効です。</span><span class="sxs-lookup"><span data-stu-id="fc2e1-122">Valid for use in VPN.</span></span>|
|<span data-ttu-id="fc2e1-123">wi-fi</span><span class="sxs-lookup"><span data-stu-id="fc2e1-123">wifi</span></span>|<span data-ttu-id="fc2e1-124">8 </span><span class="sxs-lookup"><span data-stu-id="fc2e1-124">8</span></span>|<span data-ttu-id="fc2e1-125">WiFi で使用するのに有効です。</span><span class="sxs-lookup"><span data-stu-id="fc2e1-125">Valid for use in WiFi.</span></span>|





