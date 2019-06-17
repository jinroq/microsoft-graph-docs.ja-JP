---
title: deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型
description: Credential Guard 設定の可能な値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9971c6e6f685180f95af89cc52f05540f3534fd1
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995848"
---
# <a name="deviceguardlocalsystemauthoritycredentialguardtype-enum-type"></a><span data-ttu-id="b16cf-103">deviceGuardLocalSystemAuthorityCredentialGuardType 列挙型</span><span class="sxs-lookup"><span data-stu-id="b16cf-103">deviceGuardLocalSystemAuthorityCredentialGuardType enum type</span></span>

> <span data-ttu-id="b16cf-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b16cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b16cf-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b16cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b16cf-106">Credential Guard 設定の可能な値。</span><span class="sxs-lookup"><span data-stu-id="b16cf-106">Possible values of Credential Guard settings.</span></span>

## <a name="members"></a><span data-ttu-id="b16cf-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="b16cf-107">Members</span></span>
|<span data-ttu-id="b16cf-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="b16cf-108">Member</span></span>|<span data-ttu-id="b16cf-109">値</span><span class="sxs-lookup"><span data-stu-id="b16cf-109">Value</span></span>|<span data-ttu-id="b16cf-110">説明</span><span class="sxs-lookup"><span data-stu-id="b16cf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b16cf-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b16cf-111">notConfigured</span></span>|<span data-ttu-id="b16cf-112">.0</span><span class="sxs-lookup"><span data-stu-id="b16cf-112">0</span></span>|<span data-ttu-id="b16cf-113">以前に UEFI ロックを設定していない場合に、Credential Guard をリモートで無効にします。</span><span class="sxs-lookup"><span data-stu-id="b16cf-113">Turns off Credential Guard remotely if configured previously without UEFI Lock.</span></span>|
|<span data-ttu-id="b16cf-114">enableWithUEFILock</span><span class="sxs-lookup"><span data-stu-id="b16cf-114">enableWithUEFILock</span></span>|<span data-ttu-id="b16cf-115">1-d</span><span class="sxs-lookup"><span data-stu-id="b16cf-115">1</span></span>|<span data-ttu-id="b16cf-116">UEFI ロックを使用して Credential Guard を有効にします。</span><span class="sxs-lookup"><span data-stu-id="b16cf-116">Turns on Credential Guard with UEFI lock.</span></span>|
|<span data-ttu-id="b16cf-117">enableWithoutUEFILock</span><span class="sxs-lookup"><span data-stu-id="b16cf-117">enableWithoutUEFILock</span></span>|<span data-ttu-id="b16cf-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="b16cf-118">2</span></span>|<span data-ttu-id="b16cf-119">UEFI ロックなしで Credential Guard を有効にします。</span><span class="sxs-lookup"><span data-stu-id="b16cf-119">Turns on Credential Guard without UEFI lock.</span></span>|





