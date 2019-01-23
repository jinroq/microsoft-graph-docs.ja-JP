---
title: androidDeviceOwnerAppAutoUpdatePolicyType 列挙型
description: Android デバイスの所有者に指定できる値のデバイスのアプリケーションの自動状態では、ポリシーを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 68dec6bb21cf27a7b5b54f9fc8a839fba3dc6f00
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419073"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="81ec5-103">androidDeviceOwnerAppAutoUpdatePolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="81ec5-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="81ec5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="81ec5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="81ec5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81ec5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81ec5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="81ec5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81ec5-107">Android デバイスの所有者に指定できる値のデバイスのアプリケーションの自動状態では、ポリシーを更新します。</span><span class="sxs-lookup"><span data-stu-id="81ec5-107">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="81ec5-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="81ec5-108">Members</span></span>
|<span data-ttu-id="81ec5-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="81ec5-109">Member</span></span>|<span data-ttu-id="81ec5-110">値</span><span class="sxs-lookup"><span data-stu-id="81ec5-110">Value</span></span>|<span data-ttu-id="81ec5-111">説明</span><span class="sxs-lookup"><span data-stu-id="81ec5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81ec5-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="81ec5-112">notConfigured</span></span>|<span data-ttu-id="81ec5-113">0</span><span class="sxs-lookup"><span data-stu-id="81ec5-113">0</span></span>|<span data-ttu-id="81ec5-114">次のように構成されません。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="81ec5-114">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="81ec5-115">userChoice</span><span class="sxs-lookup"><span data-stu-id="81ec5-115">userChoice</span></span>|<span data-ttu-id="81ec5-116">1</span><span class="sxs-lookup"><span data-stu-id="81ec5-116">1</span></span>|<span data-ttu-id="81ec5-117">ユーザーは、自動更新を制御できます。</span><span class="sxs-lookup"><span data-stu-id="81ec5-117">The user can control auto-updates.</span></span>|
|<span data-ttu-id="81ec5-118">ぜんぜん</span><span class="sxs-lookup"><span data-stu-id="81ec5-118">never</span></span>|<span data-ttu-id="81ec5-119">2</span><span class="sxs-lookup"><span data-stu-id="81ec5-119">2</span></span>|<span data-ttu-id="81ec5-120">アプリは自動で更新しません。</span><span class="sxs-lookup"><span data-stu-id="81ec5-120">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="81ec5-121">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="81ec5-121">wiFiOnly</span></span>|<span data-ttu-id="81ec5-122">3</span><span class="sxs-lookup"><span data-stu-id="81ec5-122">3</span></span>|<span data-ttu-id="81ec5-123">アプリケーションは自動的に更新 Wi-fi 経由のみです。</span><span class="sxs-lookup"><span data-stu-id="81ec5-123">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="81ec5-124">いつも</span><span class="sxs-lookup"><span data-stu-id="81ec5-124">always</span></span>|<span data-ttu-id="81ec5-125">4</span><span class="sxs-lookup"><span data-stu-id="81ec5-125">4</span></span>|<span data-ttu-id="81ec5-126">アプリケーションは、いつでも自動的に更新します。</span><span class="sxs-lookup"><span data-stu-id="81ec5-126">Apps are auto-updated at any time.</span></span> <span data-ttu-id="81ec5-127">データ料がかかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="81ec5-127">Data charges may apply.</span></span>|




