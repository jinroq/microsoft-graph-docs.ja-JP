---
title: managedAppDataEncryptionType 列挙型
description: 管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 67c74dea08eac63fe22aa003af1c282be85669b6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038062"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="0fbed-103">managedAppDataEncryptionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="0fbed-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="0fbed-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0fbed-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fbed-105">管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="0fbed-105">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="0fbed-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="0fbed-106">Members</span></span>
|<span data-ttu-id="0fbed-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="0fbed-107">Member</span></span>|<span data-ttu-id="0fbed-108">値</span><span class="sxs-lookup"><span data-stu-id="0fbed-108">Value</span></span>|<span data-ttu-id="0fbed-109">説明</span><span class="sxs-lookup"><span data-stu-id="0fbed-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0fbed-110">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="0fbed-110">useDeviceSettings</span></span>|<span data-ttu-id="0fbed-111">.0</span><span class="sxs-lookup"><span data-stu-id="0fbed-111">0</span></span>|<span data-ttu-id="0fbed-112">アプリデータは、デバイスの既定の設定に基づいて暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="0fbed-112">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="0fbed-113">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="0fbed-113">afterDeviceRestart</span></span>|<span data-ttu-id="0fbed-114">1-d</span><span class="sxs-lookup"><span data-stu-id="0fbed-114">1</span></span>|<span data-ttu-id="0fbed-115">アプリのデータは、デバイスの再起動時に暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="0fbed-115">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="0fbed-116">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="0fbed-116">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="0fbed-117">pbm-2</span><span class="sxs-lookup"><span data-stu-id="0fbed-117">2</span></span>|<span data-ttu-id="0fbed-118">このポリシーに関連付けられたアプリデータは、開いているファイル内のデータを除き、デバイスがロックされたときに暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="0fbed-118">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="0fbed-119">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="0fbed-119">whenDeviceLocked</span></span>|<span data-ttu-id="0fbed-120">1/3</span><span class="sxs-lookup"><span data-stu-id="0fbed-120">3</span></span>|<span data-ttu-id="0fbed-121">デバイスがロックされている場合、このポリシーに関連付けられているアプリデータは暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="0fbed-121">App data associated with this policy is encrypted when the device is locked</span></span>|



