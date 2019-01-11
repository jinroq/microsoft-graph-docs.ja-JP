---
title: managedAppDataEncryptionType 列挙型
description: マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f57904d45b24f6aaae9d67394facb07692add67e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834147"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="6151b-103">managedAppDataEncryptionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="6151b-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="6151b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6151b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6151b-105">マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="6151b-105">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="6151b-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="6151b-106">Members</span></span>
|<span data-ttu-id="6151b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="6151b-107">Member</span></span>|<span data-ttu-id="6151b-108">値</span><span class="sxs-lookup"><span data-stu-id="6151b-108">Value</span></span>|<span data-ttu-id="6151b-109">説明</span><span class="sxs-lookup"><span data-stu-id="6151b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6151b-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="6151b-110">useDeviceSettings</span></span>|<span data-ttu-id="6151b-111">0</span><span class="sxs-lookup"><span data-stu-id="6151b-111">0</span></span>|<span data-ttu-id="6151b-112">デバイスの既定の設定に基づいて、アプリケーション データが暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="6151b-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="6151b-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="6151b-113">afterDeviceRestart</span></span>|<span data-ttu-id="6151b-114">1</span><span class="sxs-lookup"><span data-stu-id="6151b-114">1</span></span>|<span data-ttu-id="6151b-115">デバイスが再起動されると、アプリケーション データが暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="6151b-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="6151b-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="6151b-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="6151b-117">2</span><span class="sxs-lookup"><span data-stu-id="6151b-117">2</span></span>|<span data-ttu-id="6151b-118">開かれているファイル内のデータを除いて、デバイスがロックされている場合、このポリシーに関連付けられているアプリケーションのデータは暗号化されて</span><span class="sxs-lookup"><span data-stu-id="6151b-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="6151b-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="6151b-119">whenDeviceLocked</span></span>|<span data-ttu-id="6151b-120">3</span><span class="sxs-lookup"><span data-stu-id="6151b-120">3</span></span>|<span data-ttu-id="6151b-121">デバイスがロックされている場合、このポリシーに関連付けられているアプリケーション データが暗号化されて</span><span class="sxs-lookup"><span data-stu-id="6151b-121">App data associated with this policy is encrypted when the device is locked</span></span>|



