---
title: macOSGatekeeperAppSources 列挙型
description: macOS ゲートキーパーのアプリソースオプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dbe261b223a180f64016d41495a0f4fcec22868
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771069"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="e5c34-103">macOSGatekeeperAppSources 列挙型</span><span class="sxs-lookup"><span data-stu-id="e5c34-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="e5c34-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5c34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e5c34-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5c34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5c34-106">macOS ゲートキーパーのアプリソースオプション。</span><span class="sxs-lookup"><span data-stu-id="e5c34-106">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="e5c34-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e5c34-107">Members</span></span>
|<span data-ttu-id="e5c34-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="e5c34-108">Member</span></span>|<span data-ttu-id="e5c34-109">値</span><span class="sxs-lookup"><span data-stu-id="e5c34-109">Value</span></span>|<span data-ttu-id="e5c34-110">説明</span><span class="sxs-lookup"><span data-stu-id="e5c34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5c34-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e5c34-111">notConfigured</span></span>|<span data-ttu-id="e5c34-112">.0</span><span class="sxs-lookup"><span data-stu-id="e5c34-112">0</span></span>|<span data-ttu-id="e5c34-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="e5c34-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="e5c34-114">macappstore</span><span class="sxs-lookup"><span data-stu-id="e5c34-114">macAppStore</span></span>|<span data-ttu-id="e5c34-115">1-d</span><span class="sxs-lookup"><span data-stu-id="e5c34-115">1</span></span>|<span data-ttu-id="e5c34-116">Mac appstore からのアプリのみを実行できます。</span><span class="sxs-lookup"><span data-stu-id="e5c34-116">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="e5c34-117">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="e5c34-117">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="e5c34-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="e5c34-118">2</span></span>|<span data-ttu-id="e5c34-119">Mac appstore のアプリのみを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="e5c34-119">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="e5c34-120">箇所</span><span class="sxs-lookup"><span data-stu-id="e5c34-120">anywhere</span></span>|<span data-ttu-id="e5c34-121">1/3</span><span class="sxs-lookup"><span data-stu-id="e5c34-121">3</span></span>|<span data-ttu-id="e5c34-122">任意の場所からアプリを実行できます。</span><span class="sxs-lookup"><span data-stu-id="e5c34-122">Apps from anywhere can be run.</span></span>|





