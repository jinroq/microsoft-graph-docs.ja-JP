---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型
description: Credential Guard 設定の可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8452f24f0bc5641d9d7ebcfd68c8cd593443554d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30167859"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="d5b25-103">deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d5b25-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="d5b25-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5b25-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5b25-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d5b25-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5b25-106">Credential Guard 設定の可能な値。</span><span class="sxs-lookup"><span data-stu-id="d5b25-106">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="d5b25-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5b25-107">Members</span></span>
|<span data-ttu-id="d5b25-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d5b25-108">Member</span></span>|<span data-ttu-id="d5b25-109">値</span><span class="sxs-lookup"><span data-stu-id="d5b25-109">Value</span></span>|<span data-ttu-id="d5b25-110">説明</span><span class="sxs-lookup"><span data-stu-id="d5b25-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5b25-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d5b25-111">notConfigured</span></span>|<span data-ttu-id="d5b25-112">.0</span><span class="sxs-lookup"><span data-stu-id="d5b25-112">0</span></span>|<span data-ttu-id="d5b25-113">以前に UEFI ロックを設定していない場合に、Credential Guard をリモートで無効にします。</span><span class="sxs-lookup"><span data-stu-id="d5b25-113">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="d5b25-114">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="d5b25-114">enableWithUEFILock</span></span>|<span data-ttu-id="d5b25-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d5b25-115">1</span></span>|<span data-ttu-id="d5b25-116">UEFI ロックを使用して Credential Guard を有効にします。</span><span class="sxs-lookup"><span data-stu-id="d5b25-116">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="d5b25-117">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="d5b25-117">enableWithoutUEFILock</span></span>|<span data-ttu-id="d5b25-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d5b25-118">2</span></span>|<span data-ttu-id="d5b25-119">UEFI ロックなしで Credential Guard を有効にします。</span><span class="sxs-lookup"><span data-stu-id="d5b25-119">Turns on Credential Guard without UEFI lock.</span></span>|




