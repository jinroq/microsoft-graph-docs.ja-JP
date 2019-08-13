---
title: managedAppDataEncryptionType 列挙型
description: 管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 273303044af0ed6b5a13c1221e99e00ccd57026e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332177"
---
# <a name="managedappdataencryptiontype-enum-type"></a><span data-ttu-id="ac385-103">managedAppDataEncryptionType 列挙型</span><span class="sxs-lookup"><span data-stu-id="ac385-103">managedAppDataEncryptionType enum type</span></span>

> <span data-ttu-id="ac385-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac385-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac385-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ac385-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac385-106">管理対象アプリについてアプリケーションデータを暗号化するレベルを表します。</span><span class="sxs-lookup"><span data-stu-id="ac385-106">Represents the level to which app data is encrypted for managed apps</span></span>

## <a name="members"></a><span data-ttu-id="ac385-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="ac385-107">Members</span></span>
|<span data-ttu-id="ac385-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ac385-108">Member</span></span>|<span data-ttu-id="ac385-109">値</span><span class="sxs-lookup"><span data-stu-id="ac385-109">Value</span></span>|<span data-ttu-id="ac385-110">説明</span><span class="sxs-lookup"><span data-stu-id="ac385-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac385-111">useDeviceSettings</span><span class="sxs-lookup"><span data-stu-id="ac385-111">useDeviceSettings</span></span>|<span data-ttu-id="ac385-112">.0</span><span class="sxs-lookup"><span data-stu-id="ac385-112">0</span></span>|<span data-ttu-id="ac385-113">アプリデータは、デバイスの既定の設定に基づいて暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="ac385-113">App data is encrypted based on the default settings on the device.</span></span>|
|<span data-ttu-id="ac385-114">afterDeviceRestart</span><span class="sxs-lookup"><span data-stu-id="ac385-114">afterDeviceRestart</span></span>|<span data-ttu-id="ac385-115">1-d</span><span class="sxs-lookup"><span data-stu-id="ac385-115">1</span></span>|<span data-ttu-id="ac385-116">アプリのデータは、デバイスの再起動時に暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="ac385-116">App data is encrypted when the device is restarted.</span></span>|
|<span data-ttu-id="ac385-117">whenDeviceLockedExceptOpenFiles</span><span class="sxs-lookup"><span data-stu-id="ac385-117">whenDeviceLockedExceptOpenFiles</span></span>|<span data-ttu-id="ac385-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="ac385-118">2</span></span>|<span data-ttu-id="ac385-119">このポリシーに関連付けられたアプリデータは、開いているファイル内のデータを除き、デバイスがロックされたときに暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="ac385-119">App data associated with this policy is encrypted when the device is locked, except data in files that are open</span></span>|
|<span data-ttu-id="ac385-120">whenDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="ac385-120">whenDeviceLocked</span></span>|<span data-ttu-id="ac385-121">1/3</span><span class="sxs-lookup"><span data-stu-id="ac385-121">3</span></span>|<span data-ttu-id="ac385-122">デバイスがロックされている場合、このポリシーに関連付けられているアプリデータは暗号化されます。</span><span class="sxs-lookup"><span data-stu-id="ac385-122">App data associated with this policy is encrypted when the device is locked</span></span>|



