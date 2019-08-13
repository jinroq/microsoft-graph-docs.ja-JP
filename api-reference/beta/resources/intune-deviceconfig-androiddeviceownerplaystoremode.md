---
title: androidDeviceOwnerPlayStoreMode 列挙型
description: Android デバイス所有者再生ストアモードの種類。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d883091a7162c7cb0da40113430edbdc66a9cfa7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36334809"
---
# <a name="androiddeviceownerplaystoremode-enum-type"></a><span data-ttu-id="9127f-103">androidDeviceOwnerPlayStoreMode 列挙型</span><span class="sxs-lookup"><span data-stu-id="9127f-103">androidDeviceOwnerPlayStoreMode enum type</span></span>

> <span data-ttu-id="9127f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9127f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9127f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9127f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9127f-106">Android デバイス所有者再生ストアモードの種類。</span><span class="sxs-lookup"><span data-stu-id="9127f-106">Android Device Owner Play Store mode type.</span></span>

## <a name="members"></a><span data-ttu-id="9127f-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="9127f-107">Members</span></span>
|<span data-ttu-id="9127f-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="9127f-108">Member</span></span>|<span data-ttu-id="9127f-109">値</span><span class="sxs-lookup"><span data-stu-id="9127f-109">Value</span></span>|<span data-ttu-id="9127f-110">説明</span><span class="sxs-lookup"><span data-stu-id="9127f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9127f-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9127f-111">notConfigured</span></span>|<span data-ttu-id="9127f-112">.0</span><span class="sxs-lookup"><span data-stu-id="9127f-112">0</span></span>|<span data-ttu-id="9127f-113">Not Configured</span><span class="sxs-lookup"><span data-stu-id="9127f-113">Not Configured</span></span>|
|<span data-ttu-id="9127f-114">allowList</span><span class="sxs-lookup"><span data-stu-id="9127f-114">allowList</span></span>|<span data-ttu-id="9127f-115">1-d</span><span class="sxs-lookup"><span data-stu-id="9127f-115">1</span></span>|<span data-ttu-id="9127f-116">ポリシーに含まれるアプリのみが利用可能であり、ポリシーに含まれていないアプリはデバイスから自動的にアンインストールされます。</span><span class="sxs-lookup"><span data-stu-id="9127f-116">Only apps that are in the policy are available and any app not in the policy will be automatically uninstalled from the device.</span></span>|
|<span data-ttu-id="9127f-117">blockList</span><span class="sxs-lookup"><span data-stu-id="9127f-117">blockList</span></span>|<span data-ttu-id="9127f-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="9127f-118">2</span></span>|<span data-ttu-id="9127f-119">すべてのアプリが利用可能で、デバイス上に配置する必要がないアプリは、アプリケーションポリシーで明示的に ' ブロック ' としてマークされている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9127f-119">All apps are available and any app that should not be on the device should be explicitly marked as 'BLOCKED' in the applications policy.</span></span>|



