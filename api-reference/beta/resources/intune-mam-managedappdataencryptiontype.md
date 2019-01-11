---
title: managedAppDataEncryptionType 列挙型
description: マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2c494b6822a2a85cd4a3d295ac70b80efffcd10
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885947"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="4ba3e-103">managedAppDataEncryptionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4ba3e-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="4ba3e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4ba3e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4ba3e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4ba3e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4ba3e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4ba3e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4ba3e-107">マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="4ba3e-107">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="4ba3e-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="4ba3e-108">Members</span></span>
|<span data-ttu-id="4ba3e-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="4ba3e-109">Member</span></span>|<span data-ttu-id="4ba3e-110">値</span><span class="sxs-lookup"><span data-stu-id="4ba3e-110">Value</span></span>|<span data-ttu-id="4ba3e-111">説明</span><span class="sxs-lookup"><span data-stu-id="4ba3e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ba3e-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="4ba3e-112">useDeviceSettings</span></span>|<span data-ttu-id="4ba3e-113">0</span><span class="sxs-lookup"><span data-stu-id="4ba3e-113">0</span></span>|<span data-ttu-id="4ba3e-114">デバイスの既定の設定に基づいて、アプリケーション データが暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="4ba3e-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="4ba3e-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="4ba3e-115">afterDeviceRestart</span></span>|<span data-ttu-id="4ba3e-116">1</span><span class="sxs-lookup"><span data-stu-id="4ba3e-116">1</span></span>|<span data-ttu-id="4ba3e-117">デバイスが再起動されると、アプリケーション データが暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="4ba3e-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="4ba3e-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="4ba3e-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="4ba3e-119">2</span><span class="sxs-lookup"><span data-stu-id="4ba3e-119">2</span></span>|<span data-ttu-id="4ba3e-120">開かれているファイル内のデータを除いて、デバイスがロックされている場合、このポリシーに関連付けられているアプリケーションのデータは暗号化されて</span><span class="sxs-lookup"><span data-stu-id="4ba3e-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="4ba3e-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="4ba3e-121">whenDeviceLocked</span></span>|<span data-ttu-id="4ba3e-122">3</span><span class="sxs-lookup"><span data-stu-id="4ba3e-122">3</span></span>|<span data-ttu-id="4ba3e-123">デバイスがロックされている場合、このポリシーに関連付けられているアプリケーション データが暗号化されて</span><span class="sxs-lookup"><span data-stu-id="4ba3e-123">App data associated with this policy is encrypted when the device is locked</span></span>|





