---
title: androidManagedAppSafetyNetDeviceAttestationType 列挙型
description: 管理者が管理対象アプリに Android の saf etynet デバイスの構成証明の要件を適用している。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cef86d779a866174749a0916ab606f64374bfa1d
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775472"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="1799f-103">androidManagedAppSafetyNetDeviceAttestationType 列挙型</span><span class="sxs-lookup"><span data-stu-id="1799f-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="1799f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1799f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1799f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1799f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1799f-106">管理者が管理対象アプリに Android の saf etynet デバイスの構成証明の要件を適用している。</span><span class="sxs-lookup"><span data-stu-id="1799f-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="1799f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="1799f-107">Members</span></span>
|<span data-ttu-id="1799f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1799f-108">Member</span></span>|<span data-ttu-id="1799f-109">値</span><span class="sxs-lookup"><span data-stu-id="1799f-109">Value</span></span>|<span data-ttu-id="1799f-110">説明</span><span class="sxs-lookup"><span data-stu-id="1799f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1799f-111">none</span><span class="sxs-lookup"><span data-stu-id="1799f-111">none</span></span>|<span data-ttu-id="1799f-112">.0</span><span class="sxs-lookup"><span data-stu-id="1799f-112">0</span></span>|<span data-ttu-id="1799f-113">要件セットなし</span><span class="sxs-lookup"><span data-stu-id="1799f-113">no requirement set</span></span>|
|<span data-ttu-id="1799f-114">basicintegrity</span><span class="sxs-lookup"><span data-stu-id="1799f-114">basicIntegrity</span></span>|<span data-ttu-id="1799f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="1799f-115">1</span></span>|<span data-ttu-id="1799f-116">Android デバイスが安全であることを必要とするのは、安全な整合性検証</span><span class="sxs-lookup"><span data-stu-id="1799f-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="1799f-117">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="1799f-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="1799f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="1799f-118">2</span></span>|<span data-ttu-id="1799f-119">Android デバイスが安全であることを必要とする、の基本的な整合性とデバイス証明の検証</span><span class="sxs-lookup"><span data-stu-id="1799f-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|





