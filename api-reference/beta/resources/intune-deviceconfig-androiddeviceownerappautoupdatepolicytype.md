---
title: androidDeviceOwnerAppAutoUpdatePolicyType 列挙型
description: Android デバイス所有者デバイスのアプリ自動更新ポリシーの状態の値を指定できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 703e8bbb46ae289acfa09267052f9c78fe0da912
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965719"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="3b3c0-103">androidDeviceOwnerAppAutoUpdatePolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="3b3c0-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="3b3c0-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b3c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b3c0-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3b3c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b3c0-106">Android デバイス所有者デバイスのアプリ自動更新ポリシーの状態の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="3b3c0-106">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="3b3c0-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="3b3c0-107">Members</span></span>
|<span data-ttu-id="3b3c0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="3b3c0-108">Member</span></span>|<span data-ttu-id="3b3c0-109">値</span><span class="sxs-lookup"><span data-stu-id="3b3c0-109">Value</span></span>|<span data-ttu-id="3b3c0-110">説明</span><span class="sxs-lookup"><span data-stu-id="3b3c0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b3c0-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="3b3c0-111">notConfigured</span></span>|<span data-ttu-id="3b3c0-112">.0</span><span class="sxs-lookup"><span data-stu-id="3b3c0-112">0</span></span>|<span data-ttu-id="3b3c0-113">未構成。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="3b3c0-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="3b3c0-114">userChoice</span><span class="sxs-lookup"><span data-stu-id="3b3c0-114">userChoice</span></span>|<span data-ttu-id="3b3c0-115">1-d</span><span class="sxs-lookup"><span data-stu-id="3b3c0-115">1</span></span>|<span data-ttu-id="3b3c0-116">ユーザーは自動更新を制御できます。</span><span class="sxs-lookup"><span data-stu-id="3b3c0-116">The user can control auto-updates.</span></span>|
|<span data-ttu-id="3b3c0-117">ぜんぜん</span><span class="sxs-lookup"><span data-stu-id="3b3c0-117">never</span></span>|<span data-ttu-id="3b3c0-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="3b3c0-118">2</span></span>|<span data-ttu-id="3b3c0-119">アプリが自動更新されることはありません。</span><span class="sxs-lookup"><span data-stu-id="3b3c0-119">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="3b3c0-120">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="3b3c0-120">wiFiOnly</span></span>|<span data-ttu-id="3b3c0-121">1/3</span><span class="sxs-lookup"><span data-stu-id="3b3c0-121">3</span></span>|<span data-ttu-id="3b3c0-122">アプリは Wi-fi 経由で自動更新されます。</span><span class="sxs-lookup"><span data-stu-id="3b3c0-122">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="3b3c0-123">いつも</span><span class="sxs-lookup"><span data-stu-id="3b3c0-123">always</span></span>|<span data-ttu-id="3b3c0-124">2/4</span><span class="sxs-lookup"><span data-stu-id="3b3c0-124">4</span></span>|<span data-ttu-id="3b3c0-125">アプリはいつでも自動更新されます。</span><span class="sxs-lookup"><span data-stu-id="3b3c0-125">Apps are auto-updated at any time.</span></span> <span data-ttu-id="3b3c0-126">データ料金が適用される場合があります。</span><span class="sxs-lookup"><span data-stu-id="3b3c0-126">Data charges may apply.</span></span>|





