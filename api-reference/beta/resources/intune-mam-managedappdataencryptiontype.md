---
title: managedAppDataEncryptionType 列挙型
description: 管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 962e759e83b08baf7fc150e07dc84ed7146feb0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563855"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="205e8-103">managedAppDataEncryptionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="205e8-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="205e8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="205e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="205e8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="205e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="205e8-106">管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="205e8-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="205e8-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="205e8-107">Members</span></span>
|<span data-ttu-id="205e8-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="205e8-108">Member</span></span>|<span data-ttu-id="205e8-109">値</span><span class="sxs-lookup"><span data-stu-id="205e8-109">Value</span></span>|<span data-ttu-id="205e8-110">説明</span><span class="sxs-lookup"><span data-stu-id="205e8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="205e8-111">usedevicesettings</span><span class="sxs-lookup"><span data-stu-id="205e8-111">useDeviceSettings</span></span>|<span data-ttu-id="205e8-112">.0</span><span class="sxs-lookup"><span data-stu-id="205e8-112">0</span></span>|<span data-ttu-id="205e8-113">アプリデータは、デバイスの既定の設定に基づいて暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="205e8-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="205e8-114">afterdevicerestart</span><span class="sxs-lookup"><span data-stu-id="205e8-114">afterDeviceRestart</span></span>|<span data-ttu-id="205e8-115">1 </span><span class="sxs-lookup"><span data-stu-id="205e8-115">1</span></span>|<span data-ttu-id="205e8-116">アプリのデータは、デバイスの再起動時に暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="205e8-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="205e8-117">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="205e8-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="205e8-118">2 </span><span class="sxs-lookup"><span data-stu-id="205e8-118">2</span></span>|<span data-ttu-id="205e8-119">このポリシーに関連付けられたアプリデータは、開いているファイル内のデータを除き、デバイスがロックされたときに暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="205e8-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="205e8-120">whendevicelocked</span><span class="sxs-lookup"><span data-stu-id="205e8-120">whenDeviceLocked</span></span>|<span data-ttu-id="205e8-121">3 </span><span class="sxs-lookup"><span data-stu-id="205e8-121">3</span></span>|<span data-ttu-id="205e8-122">デバイスがロックされている場合、このポリシーに関連付けられているアプリデータは暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="205e8-122">App data associated with this policy is encrypted when the device is locked</span></span>|





