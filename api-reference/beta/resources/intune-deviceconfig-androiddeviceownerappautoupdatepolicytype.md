---
title: androidDeviceOwnerAppAutoUpdatePolicyType 列挙型
description: Android デバイス所有者デバイスのアプリ自動更新ポリシーの状態の値を指定できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5e67dbdd96c1df067ead3724705a4c2067757130
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556517"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="57248-103">androidDeviceOwnerAppAutoUpdatePolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="57248-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="57248-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="57248-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57248-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="57248-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57248-106">Android デバイス所有者デバイスのアプリ自動更新ポリシーの状態の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="57248-106">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="57248-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="57248-107">Members</span></span>
|<span data-ttu-id="57248-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="57248-108">Member</span></span>|<span data-ttu-id="57248-109">値</span><span class="sxs-lookup"><span data-stu-id="57248-109">Value</span></span>|<span data-ttu-id="57248-110">説明</span><span class="sxs-lookup"><span data-stu-id="57248-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57248-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="57248-111">notConfigured</span></span>|<span data-ttu-id="57248-112">.0</span><span class="sxs-lookup"><span data-stu-id="57248-112">0</span></span>|<span data-ttu-id="57248-113">未構成。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="57248-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="57248-114">userchoice</span><span class="sxs-lookup"><span data-stu-id="57248-114">userChoice</span></span>|<span data-ttu-id="57248-115">1 </span><span class="sxs-lookup"><span data-stu-id="57248-115">1</span></span>|<span data-ttu-id="57248-116">ユーザーは自動更新を制御できます。</span><span class="sxs-lookup"><span data-stu-id="57248-116">The user can control auto-updates.</span></span>|
|<span data-ttu-id="57248-117">ぜんぜん</span><span class="sxs-lookup"><span data-stu-id="57248-117">never</span></span>|<span data-ttu-id="57248-118">2 </span><span class="sxs-lookup"><span data-stu-id="57248-118">2</span></span>|<span data-ttu-id="57248-119">アプリが自動更新されることはありません。</span><span class="sxs-lookup"><span data-stu-id="57248-119">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="57248-120">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="57248-120">wiFiOnly</span></span>|<span data-ttu-id="57248-121">3 </span><span class="sxs-lookup"><span data-stu-id="57248-121">3</span></span>|<span data-ttu-id="57248-122">アプリは wi-fi 経由で自動更新されます。</span><span class="sxs-lookup"><span data-stu-id="57248-122">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="57248-123">いつも</span><span class="sxs-lookup"><span data-stu-id="57248-123">always</span></span>|<span data-ttu-id="57248-124">4 </span><span class="sxs-lookup"><span data-stu-id="57248-124">4</span></span>|<span data-ttu-id="57248-125">アプリはいつでも自動更新されます。</span><span class="sxs-lookup"><span data-stu-id="57248-125">Apps are auto-updated at any time.</span></span> <span data-ttu-id="57248-126">データ料金が適用される場合があります。</span><span class="sxs-lookup"><span data-stu-id="57248-126">Data charges may apply.</span></span>|





