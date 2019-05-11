---
title: androidDeviceOwnerPlayStoreMode 列挙型
description: Android デバイス所有者再生ストアモードの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d37f57dc2481e18871fca840499142eda30ab8fd
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949004"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="96636-103">androidDeviceOwnerPlayStoreMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="96636-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

> <span data-ttu-id="96636-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="96636-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96636-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="96636-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96636-106">Android デバイス所有者再生ストアモードの種類。</span><span class="sxs-lookup"><span data-stu-id="96636-106">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="96636-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="96636-107">Members</span></span>
|<span data-ttu-id="96636-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="96636-108">Member</span></span>|<span data-ttu-id="96636-109">値</span><span class="sxs-lookup"><span data-stu-id="96636-109">Value</span></span>|<span data-ttu-id="96636-110">説明</span><span class="sxs-lookup"><span data-stu-id="96636-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96636-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="96636-111">notConfigured</span></span>|<span data-ttu-id="96636-112">.0</span><span class="sxs-lookup"><span data-stu-id="96636-112">0</span></span>|<span data-ttu-id="96636-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="96636-113">Not Configured</span></span>|
|<span data-ttu-id="96636-114">allowList</span><span class="sxs-lookup"><span data-stu-id="96636-114">allowList</span></span>|<span data-ttu-id="96636-115">1-d</span><span class="sxs-lookup"><span data-stu-id="96636-115">1</span></span>|<span data-ttu-id="96636-116">ポリシーに含まれるアプリのみが利用可能であり、ポリシーに含まれていないアプリはデバイスから自動的にアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="96636-116">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="96636-117">blockList</span><span class="sxs-lookup"><span data-stu-id="96636-117">blockList</span></span>|<span data-ttu-id="96636-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="96636-118">2</span></span>|<span data-ttu-id="96636-119">すべてのアプリが利用可能で、デバイス上に配置する必要がないアプリは、アプリケーションポリシーで明示的に ' ブロック ' としてマークされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="96636-119">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|




