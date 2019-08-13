---
title: androidDeviceOwnerAppAutoUpdatePolicyType 列挙型
description: Android デバイス所有者デバイスのアプリ自動更新ポリシーの状態の値を指定できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3491d175f4157bae2229277e35ea937741d06324
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334865"
---
# <a name="androiddeviceownerappautoupdatepolicytype-enum-type"></a><span data-ttu-id="5ca8f-103">androidDeviceOwnerAppAutoUpdatePolicyType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5ca8f-103">androidDeviceOwnerAppAutoUpdatePolicyType enum type</span></span>

> <span data-ttu-id="5ca8f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5ca8f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ca8f-106">Android デバイス所有者デバイスのアプリ自動更新ポリシーの状態の値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-106">Android Device Owner possible values for states of the device's app auto update policy.</span></span>

## <a name="members"></a><span data-ttu-id="5ca8f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5ca8f-107">Members</span></span>
|<span data-ttu-id="5ca8f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5ca8f-108">Member</span></span>|<span data-ttu-id="5ca8f-109">値</span><span class="sxs-lookup"><span data-stu-id="5ca8f-109">Value</span></span>|<span data-ttu-id="5ca8f-110">説明</span><span class="sxs-lookup"><span data-stu-id="5ca8f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ca8f-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="5ca8f-111">notConfigured</span></span>|<span data-ttu-id="5ca8f-112">.0</span><span class="sxs-lookup"><span data-stu-id="5ca8f-112">0</span></span>|<span data-ttu-id="5ca8f-113">未構成。この値は無視されます。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-113">Not configured; this value is ignored.</span></span>|
|<span data-ttu-id="5ca8f-114">userChoice</span><span class="sxs-lookup"><span data-stu-id="5ca8f-114">userChoice</span></span>|<span data-ttu-id="5ca8f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="5ca8f-115">1</span></span>|<span data-ttu-id="5ca8f-116">ユーザーは自動更新を制御できます。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-116">The user can control auto-updates.</span></span>|
|<span data-ttu-id="5ca8f-117">ぜんぜん</span><span class="sxs-lookup"><span data-stu-id="5ca8f-117">never</span></span>|<span data-ttu-id="5ca8f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="5ca8f-118">2</span></span>|<span data-ttu-id="5ca8f-119">アプリが自動更新されることはありません。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-119">Apps are never auto-updated.</span></span>|
|<span data-ttu-id="5ca8f-120">wiFiOnly</span><span class="sxs-lookup"><span data-stu-id="5ca8f-120">wiFiOnly</span></span>|<span data-ttu-id="5ca8f-121">1/3</span><span class="sxs-lookup"><span data-stu-id="5ca8f-121">3</span></span>|<span data-ttu-id="5ca8f-122">アプリは Wi-fi 経由で自動更新されます。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-122">Apps are auto-updated over Wi-Fi only.</span></span>|
|<span data-ttu-id="5ca8f-123">いつも</span><span class="sxs-lookup"><span data-stu-id="5ca8f-123">always</span></span>|<span data-ttu-id="5ca8f-124">2/4</span><span class="sxs-lookup"><span data-stu-id="5ca8f-124">4</span></span>|<span data-ttu-id="5ca8f-125">アプリはいつでも自動更新されます。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-125">Apps are auto-updated at any time.</span></span> <span data-ttu-id="5ca8f-126">データ料金が適用される場合があります。</span><span class="sxs-lookup"><span data-stu-id="5ca8f-126">Data charges may apply.</span></span>|



