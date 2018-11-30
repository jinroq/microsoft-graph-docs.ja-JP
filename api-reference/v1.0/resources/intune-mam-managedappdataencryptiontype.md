---
title: managedAppDataEncryptionType 列挙型
description: マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。
ms.openlocfilehash: 7efda037bc2b4d5794c575823845c0955be46477
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023043"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="793f9-103">managedAppDataEncryptionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="793f9-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="793f9-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="793f9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="793f9-105">マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="793f9-105">Represents the level to which app data is encrypted for managed apps</span></span>
## <a name="members"></a><span data-ttu-id="793f9-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="793f9-106">Members</span></span>
|<span data-ttu-id="793f9-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="793f9-107">Member</span></span>|<span data-ttu-id="793f9-108">値</span><span class="sxs-lookup"><span data-stu-id="793f9-108">Value</span></span>|<span data-ttu-id="793f9-109">説明</span><span class="sxs-lookup"><span data-stu-id="793f9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="793f9-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="793f9-110">useDeviceSettings</span></span>|<span data-ttu-id="793f9-111">0</span><span class="sxs-lookup"><span data-stu-id="793f9-111">0</span></span>|<span data-ttu-id="793f9-112">デバイスの既定の設定に基づいて、アプリケーション データが暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="793f9-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="793f9-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="793f9-113">afterDeviceRestart</span></span>|<span data-ttu-id="793f9-114">1</span><span class="sxs-lookup"><span data-stu-id="793f9-114">1</span></span>|<span data-ttu-id="793f9-115">デバイスが再起動されると、アプリケーション データが暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="793f9-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="793f9-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="793f9-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="793f9-117">2</span><span class="sxs-lookup"><span data-stu-id="793f9-117">2</span></span>|<span data-ttu-id="793f9-118">開かれているファイル内のデータを除いて、デバイスがロックされている場合、このポリシーに関連付けられているアプリケーションのデータは暗号化されて</span><span class="sxs-lookup"><span data-stu-id="793f9-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="793f9-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="793f9-119">whenDeviceLocked</span></span>|<span data-ttu-id="793f9-120">3</span><span class="sxs-lookup"><span data-stu-id="793f9-120">3</span></span>|<span data-ttu-id="793f9-121">デバイスがロックされている場合、このポリシーに関連付けられているアプリケーション データが暗号化されて</span><span class="sxs-lookup"><span data-stu-id="793f9-121">App data associated with this policy is encrypted when the device is locked</span></span>|


