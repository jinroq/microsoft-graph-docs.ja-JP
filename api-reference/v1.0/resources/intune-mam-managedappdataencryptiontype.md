---
title: managedAppDataEncryptionType 列挙型
description: マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。
author: tfitzmac
ms.openlocfilehash: 3cbb733eb578ca839e32851d8a6d217f69d6799d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330325"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="89d2e-103">managedAppDataEncryptionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="89d2e-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="89d2e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="89d2e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89d2e-105">マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="89d2e-105">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="89d2e-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="89d2e-106">Members</span></span>
|<span data-ttu-id="89d2e-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="89d2e-107">Member</span></span>|<span data-ttu-id="89d2e-108">値</span><span class="sxs-lookup"><span data-stu-id="89d2e-108">Value</span></span>|<span data-ttu-id="89d2e-109">説明</span><span class="sxs-lookup"><span data-stu-id="89d2e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89d2e-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="89d2e-110">useDeviceSettings</span></span>|<span data-ttu-id="89d2e-111">0</span><span class="sxs-lookup"><span data-stu-id="89d2e-111">0</span></span>|<span data-ttu-id="89d2e-112">デバイスの既定の設定に基づいて、アプリケーション データが暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="89d2e-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="89d2e-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="89d2e-113">afterDeviceRestart</span></span>|<span data-ttu-id="89d2e-114">1</span><span class="sxs-lookup"><span data-stu-id="89d2e-114">1</span></span>|<span data-ttu-id="89d2e-115">デバイスが再起動されると、アプリケーション データが暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="89d2e-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="89d2e-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="89d2e-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="89d2e-117">2</span><span class="sxs-lookup"><span data-stu-id="89d2e-117">2</span></span>|<span data-ttu-id="89d2e-118">開かれているファイル内のデータを除いて、デバイスがロックされている場合、このポリシーに関連付けられているアプリケーションのデータは暗号化されて</span><span class="sxs-lookup"><span data-stu-id="89d2e-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="89d2e-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="89d2e-119">whenDeviceLocked</span></span>|<span data-ttu-id="89d2e-120">3</span><span class="sxs-lookup"><span data-stu-id="89d2e-120">3</span></span>|<span data-ttu-id="89d2e-121">デバイスがロックされている場合、このポリシーに関連付けられているアプリケーション データが暗号化されて</span><span class="sxs-lookup"><span data-stu-id="89d2e-121">App data associated with this policy is encrypted when the device is locked</span></span>|



