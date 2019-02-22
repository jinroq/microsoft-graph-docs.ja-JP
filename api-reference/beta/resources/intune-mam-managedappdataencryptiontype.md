---
title: managedAppDataEncryptionType 列挙型
description: 管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47396f32ed23234c5fe758a29b6e97ee3602234f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159081"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="d520a-103">managedAppDataEncryptionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="d520a-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="d520a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d520a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d520a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d520a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d520a-106">管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="d520a-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="d520a-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="d520a-107">Members</span></span>
|<span data-ttu-id="d520a-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="d520a-108">Member</span></span>|<span data-ttu-id="d520a-109">値</span><span class="sxs-lookup"><span data-stu-id="d520a-109">Value</span></span>|<span data-ttu-id="d520a-110">説明</span><span class="sxs-lookup"><span data-stu-id="d520a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d520a-111">usedevicesettings</span><span class="sxs-lookup"><span data-stu-id="d520a-111">useDeviceSettings</span></span>|<span data-ttu-id="d520a-112">.0</span><span class="sxs-lookup"><span data-stu-id="d520a-112">0</span></span>|<span data-ttu-id="d520a-113">アプリデータは、デバイスの既定の設定に基づいて暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="d520a-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="d520a-114">afterdevicerestart</span><span class="sxs-lookup"><span data-stu-id="d520a-114">afterDeviceRestart</span></span>|<span data-ttu-id="d520a-115">1-d</span><span class="sxs-lookup"><span data-stu-id="d520a-115">1</span></span>|<span data-ttu-id="d520a-116">アプリのデータは、デバイスの再起動時に暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="d520a-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="d520a-117">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="d520a-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="d520a-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="d520a-118">2</span></span>|<span data-ttu-id="d520a-119">このポリシーに関連付けられたアプリデータは、開いているファイル内のデータを除き、デバイスがロックされたときに暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="d520a-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="d520a-120">whendevicelocked</span><span class="sxs-lookup"><span data-stu-id="d520a-120">whenDeviceLocked</span></span>|<span data-ttu-id="d520a-121">1/3</span><span class="sxs-lookup"><span data-stu-id="d520a-121">3</span></span>|<span data-ttu-id="d520a-122">デバイスがロックされている場合、このポリシーに関連付けられているアプリデータは暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="d520a-122">App data associated with this policy is encrypted when the device is locked</span></span>|




