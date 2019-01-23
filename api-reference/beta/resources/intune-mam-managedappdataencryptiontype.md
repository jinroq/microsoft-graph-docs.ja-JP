---
title: managedAppDataEncryptionType 列挙型
description: マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 00174e7fba8a8da7490d04815b07a794a966179c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413690"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="5b3df-103">managedAppDataEncryptionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="5b3df-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="5b3df-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5b3df-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5b3df-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5b3df-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b3df-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5b3df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b3df-107">マネージ アプリケーションのアプリケーション データを暗号化するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="5b3df-107">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="5b3df-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5b3df-108">Members</span></span>
|<span data-ttu-id="5b3df-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="5b3df-109">Member</span></span>|<span data-ttu-id="5b3df-110">値</span><span class="sxs-lookup"><span data-stu-id="5b3df-110">Value</span></span>|<span data-ttu-id="5b3df-111">説明</span><span class="sxs-lookup"><span data-stu-id="5b3df-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b3df-112">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="5b3df-112">useDeviceSettings</span></span>|<span data-ttu-id="5b3df-113">0</span><span class="sxs-lookup"><span data-stu-id="5b3df-113">0</span></span>|<span data-ttu-id="5b3df-114">デバイスの既定の設定に基づいて、アプリケーション データが暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="5b3df-114">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="5b3df-115">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="5b3df-115">afterDeviceRestart</span></span>|<span data-ttu-id="5b3df-116">1</span><span class="sxs-lookup"><span data-stu-id="5b3df-116">1</span></span>|<span data-ttu-id="5b3df-117">デバイスが再起動されると、アプリケーション データが暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="5b3df-117">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="5b3df-118">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="5b3df-118">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="5b3df-119">2</span><span class="sxs-lookup"><span data-stu-id="5b3df-119">2</span></span>|<span data-ttu-id="5b3df-120">開かれているファイル内のデータを除いて、デバイスがロックされている場合、このポリシーに関連付けられているアプリケーションのデータは暗号化されて</span><span class="sxs-lookup"><span data-stu-id="5b3df-120">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="5b3df-121">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="5b3df-121">whenDeviceLocked</span></span>|<span data-ttu-id="5b3df-122">3</span><span class="sxs-lookup"><span data-stu-id="5b3df-122">3</span></span>|<span data-ttu-id="5b3df-123">デバイスがロックされている場合、このポリシーに関連付けられているアプリケーション データが暗号化されて</span><span class="sxs-lookup"><span data-stu-id="5b3df-123">App data associated with this policy is encrypted when the device is locked</span></span>|




