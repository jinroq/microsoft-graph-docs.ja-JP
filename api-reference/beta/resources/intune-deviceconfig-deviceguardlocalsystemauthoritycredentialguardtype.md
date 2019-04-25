---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型
description: Credential Guard 設定の可能な値。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f22336a37c3d10d4e86b3db2af41e8103dcfe33
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567229"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="a0a11-103">deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a0a11-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="a0a11-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0a11-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0a11-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a0a11-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0a11-106">Credential Guard 設定の可能な値。</span><span class="sxs-lookup"><span data-stu-id="a0a11-106">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="a0a11-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a0a11-107">Members</span></span>
|<span data-ttu-id="a0a11-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a0a11-108">Member</span></span>|<span data-ttu-id="a0a11-109">値</span><span class="sxs-lookup"><span data-stu-id="a0a11-109">Value</span></span>|<span data-ttu-id="a0a11-110">説明</span><span class="sxs-lookup"><span data-stu-id="a0a11-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0a11-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="a0a11-111">notConfigured</span></span>|<span data-ttu-id="a0a11-112">.0</span><span class="sxs-lookup"><span data-stu-id="a0a11-112">0</span></span>|<span data-ttu-id="a0a11-113">以前に UEFI ロックを設定していない場合に、Credential Guard をリモートで無効にします。</span><span class="sxs-lookup"><span data-stu-id="a0a11-113">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="a0a11-114">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="a0a11-114">enableWithUEFILock</span></span>|<span data-ttu-id="a0a11-115">1 </span><span class="sxs-lookup"><span data-stu-id="a0a11-115">1</span></span>|<span data-ttu-id="a0a11-116">UEFI ロックを使用して Credential Guard を有効にします。</span><span class="sxs-lookup"><span data-stu-id="a0a11-116">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="a0a11-117">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="a0a11-117">enableWithoutUEFILock</span></span>|<span data-ttu-id="a0a11-118">2 </span><span class="sxs-lookup"><span data-stu-id="a0a11-118">2</span></span>|<span data-ttu-id="a0a11-119">UEFI ロックなしで Credential Guard を有効にします。</span><span class="sxs-lookup"><span data-stu-id="a0a11-119">Turns on Credential Guard without UEFI lock.</span></span>|





