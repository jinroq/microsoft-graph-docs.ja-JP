---
title: androidDeviceOwnerAppAutoUpdatePolicyType 列挙型
description: Android デバイス所有者デバイスのアプリ自動更新ポリシーの状態の値を指定できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 92ea62ccd7f1077558d91eef4ca9e4f7157ec258
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949193"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="d41cc-103">androidDeviceOwnerAppAutoUpdatePolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d41cc-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="d41cc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d41cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d41cc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d41cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d41cc-106">Android デバイス所有者デバイスのアプリ自動更新ポリシーの状態の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="d41cc-106">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="d41cc-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d41cc-107">Members</span></span>
|<span data-ttu-id="d41cc-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d41cc-108">Member</span></span>|<span data-ttu-id="d41cc-109">値</span><span class="sxs-lookup"><span data-stu-id="d41cc-109">Value</span></span>|<span data-ttu-id="d41cc-110">説明</span><span class="sxs-lookup"><span data-stu-id="d41cc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d41cc-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d41cc-111">notConfigured</span></span>|<span data-ttu-id="d41cc-112">.0</span><span class="sxs-lookup"><span data-stu-id="d41cc-112">0</span></span>|<span data-ttu-id="d41cc-113">未構成。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="d41cc-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="d41cc-114">userChoice</span><span class="sxs-lookup"><span data-stu-id="d41cc-114">userChoice</span></span>|<span data-ttu-id="d41cc-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d41cc-115">1</span></span>|<span data-ttu-id="d41cc-116">ユーザーは自動更新を制御できます。</span><span class="sxs-lookup"><span data-stu-id="d41cc-116">The user can control auto-updates.</span></span>|
|<span data-ttu-id="d41cc-117">ぜんぜん</span><span class="sxs-lookup"><span data-stu-id="d41cc-117">never</span></span>|<span data-ttu-id="d41cc-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d41cc-118">2</span></span>|<span data-ttu-id="d41cc-119">アプリが自動更新されることはありません。</span><span class="sxs-lookup"><span data-stu-id="d41cc-119">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="d41cc-120">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="d41cc-120">wiFiOnly</span></span>|<span data-ttu-id="d41cc-121">1/3</span><span class="sxs-lookup"><span data-stu-id="d41cc-121">3</span></span>|<span data-ttu-id="d41cc-122">アプリは Wi-fi 経由で自動更新されます。</span><span class="sxs-lookup"><span data-stu-id="d41cc-122">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="d41cc-123">いつも</span><span class="sxs-lookup"><span data-stu-id="d41cc-123">always</span></span>|<span data-ttu-id="d41cc-124">2/4</span><span class="sxs-lookup"><span data-stu-id="d41cc-124">4</span></span>|<span data-ttu-id="d41cc-125">アプリはいつでも自動更新されます。</span><span class="sxs-lookup"><span data-stu-id="d41cc-125">Apps are auto-updated at any time.</span></span> <span data-ttu-id="d41cc-126">データ料金が適用される場合があります。</span><span class="sxs-lookup"><span data-stu-id="d41cc-126">Data charges may apply.</span></span>|




