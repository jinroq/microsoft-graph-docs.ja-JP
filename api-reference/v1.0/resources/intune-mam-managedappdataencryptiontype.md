---
title: managedAppDataEncryptionType 列挙型
description: 管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 774312d5f19b223fd33e2c156610f516ae7f48a3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32465256"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="4e25b-103">managedAppDataEncryptionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="4e25b-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="4e25b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4e25b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4e25b-105">管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="4e25b-105">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="4e25b-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="4e25b-106">Members</span></span>
|<span data-ttu-id="4e25b-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="4e25b-107">Member</span></span>|<span data-ttu-id="4e25b-108">値</span><span class="sxs-lookup"><span data-stu-id="4e25b-108">Value</span></span>|<span data-ttu-id="4e25b-109">説明</span><span class="sxs-lookup"><span data-stu-id="4e25b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e25b-110">usedevicesettings</span><span class="sxs-lookup"><span data-stu-id="4e25b-110">useDeviceSettings</span></span>|<span data-ttu-id="4e25b-111">.0</span><span class="sxs-lookup"><span data-stu-id="4e25b-111">0</span></span>|<span data-ttu-id="4e25b-112">アプリデータは、デバイスの既定の設定に基づいて暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="4e25b-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="4e25b-113">afterdevicerestart</span><span class="sxs-lookup"><span data-stu-id="4e25b-113">afterDeviceRestart</span></span>|<span data-ttu-id="4e25b-114">1-d</span><span class="sxs-lookup"><span data-stu-id="4e25b-114">1</span></span>|<span data-ttu-id="4e25b-115">アプリのデータは、デバイスの再起動時に暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="4e25b-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="4e25b-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="4e25b-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="4e25b-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="4e25b-117">2</span></span>|<span data-ttu-id="4e25b-118">このポリシーに関連付けられたアプリデータは、開いているファイル内のデータを除き、デバイスがロックされたときに暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="4e25b-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="4e25b-119">whendevicelocked</span><span class="sxs-lookup"><span data-stu-id="4e25b-119">whenDeviceLocked</span></span>|<span data-ttu-id="4e25b-120">1/3</span><span class="sxs-lookup"><span data-stu-id="4e25b-120">3</span></span>|<span data-ttu-id="4e25b-121">デバイスがロックされている場合、このポリシーに関連付けられているアプリデータは暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="4e25b-121">App data associated with this policy is encrypted when the device is locked</span></span>|



