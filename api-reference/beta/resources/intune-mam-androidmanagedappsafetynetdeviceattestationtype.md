---
title: androidManagedAppSafetyNetDeviceAttestationType 列挙型
description: 管理者が管理対象アプリに Android の Saf Etynet デバイスの構成証明の要件を適用している。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 03c7496fe5e3d1fce5f73cc0f5954d8415668641
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968079"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="5728a-103">androidManagedAppSafetyNetDeviceAttestationType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5728a-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="5728a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5728a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5728a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5728a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5728a-106">管理者が管理対象アプリに Android の Saf Etynet デバイスの構成証明の要件を適用している。</span><span class="sxs-lookup"><span data-stu-id="5728a-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="5728a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="5728a-107">Members</span></span>
|<span data-ttu-id="5728a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5728a-108">Member</span></span>|<span data-ttu-id="5728a-109">値</span><span class="sxs-lookup"><span data-stu-id="5728a-109">Value</span></span>|<span data-ttu-id="5728a-110">説明</span><span class="sxs-lookup"><span data-stu-id="5728a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5728a-111">none</span><span class="sxs-lookup"><span data-stu-id="5728a-111">none</span></span>|<span data-ttu-id="5728a-112">.0</span><span class="sxs-lookup"><span data-stu-id="5728a-112">0</span></span>|<span data-ttu-id="5728a-113">要件セットなし</span><span class="sxs-lookup"><span data-stu-id="5728a-113">no requirement set</span></span>|
|<span data-ttu-id="5728a-114">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="5728a-114">basicIntegrity</span></span>|<span data-ttu-id="5728a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="5728a-115">1</span></span>|<span data-ttu-id="5728a-116">Android デバイスが安全であることを必要とするのは、安全な整合性検証</span><span class="sxs-lookup"><span data-stu-id="5728a-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="5728a-117">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="5728a-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="5728a-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="5728a-118">2</span></span>|<span data-ttu-id="5728a-119">Android デバイスが安全であることを必要とする、の基本的な整合性とデバイス証明の検証</span><span class="sxs-lookup"><span data-stu-id="5728a-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|





