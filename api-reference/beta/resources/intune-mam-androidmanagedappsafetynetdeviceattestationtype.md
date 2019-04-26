---
title: androidManagedAppSafetyNetDeviceAttestationType 列挙型
description: 管理者が管理対象アプリに Android の saf etynet デバイスの構成証明の要件を適用している。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cef86d779a866174749a0916ab606f64374bfa1d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564002"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="17297-103">androidManagedAppSafetyNetDeviceAttestationType 列挙型</span><span class="sxs-lookup"><span data-stu-id="17297-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="17297-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="17297-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="17297-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="17297-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="17297-106">管理者が管理対象アプリに Android の saf etynet デバイスの構成証明の要件を適用している。</span><span class="sxs-lookup"><span data-stu-id="17297-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="17297-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="17297-107">Members</span></span>
|<span data-ttu-id="17297-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="17297-108">Member</span></span>|<span data-ttu-id="17297-109">値</span><span class="sxs-lookup"><span data-stu-id="17297-109">Value</span></span>|<span data-ttu-id="17297-110">説明</span><span class="sxs-lookup"><span data-stu-id="17297-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="17297-111">なし</span><span class="sxs-lookup"><span data-stu-id="17297-111">none</span></span>|<span data-ttu-id="17297-112">.0</span><span class="sxs-lookup"><span data-stu-id="17297-112">0</span></span>|<span data-ttu-id="17297-113">要件セットなし</span><span class="sxs-lookup"><span data-stu-id="17297-113">no requirement set</span></span>|
|<span data-ttu-id="17297-114">basicintegrity</span><span class="sxs-lookup"><span data-stu-id="17297-114">basicIntegrity</span></span>|<span data-ttu-id="17297-115">1 </span><span class="sxs-lookup"><span data-stu-id="17297-115">1</span></span>|<span data-ttu-id="17297-116">Android デバイスが安全であることを必要とするのは、安全な整合性検証</span><span class="sxs-lookup"><span data-stu-id="17297-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="17297-117">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="17297-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="17297-118">2 </span><span class="sxs-lookup"><span data-stu-id="17297-118">2</span></span>|<span data-ttu-id="17297-119">Android デバイスが安全であることを必要とする、の基本的な整合性とデバイス証明の検証</span><span class="sxs-lookup"><span data-stu-id="17297-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|





