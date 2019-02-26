---
title: macOSGatekeeperAppSources 列挙型
description: macOS ゲートキーパーのアプリソースオプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3e43505a745e87e52f2f1c12a5cc5ff08825c09
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166207"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="512eb-103">macOSGatekeeperAppSources 列挙型</span><span class="sxs-lookup"><span data-stu-id="512eb-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="512eb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="512eb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="512eb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="512eb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="512eb-106">macOS ゲートキーパーのアプリソースオプション。</span><span class="sxs-lookup"><span data-stu-id="512eb-106">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="512eb-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="512eb-107">Members</span></span>
|<span data-ttu-id="512eb-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="512eb-108">Member</span></span>|<span data-ttu-id="512eb-109">値</span><span class="sxs-lookup"><span data-stu-id="512eb-109">Value</span></span>|<span data-ttu-id="512eb-110">説明</span><span class="sxs-lookup"><span data-stu-id="512eb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="512eb-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="512eb-111">notConfigured</span></span>|<span data-ttu-id="512eb-112">.0</span><span class="sxs-lookup"><span data-stu-id="512eb-112">0</span></span>|<span data-ttu-id="512eb-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="512eb-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="512eb-114">macappstore</span><span class="sxs-lookup"><span data-stu-id="512eb-114">macAppStore</span></span>|<span data-ttu-id="512eb-115">1-d</span><span class="sxs-lookup"><span data-stu-id="512eb-115">1</span></span>|<span data-ttu-id="512eb-116">Mac appstore からのアプリのみを実行できます。</span><span class="sxs-lookup"><span data-stu-id="512eb-116">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="512eb-117">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="512eb-117">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="512eb-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="512eb-118">2</span></span>|<span data-ttu-id="512eb-119">Mac appstore のアプリのみを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="512eb-119">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="512eb-120">箇所</span><span class="sxs-lookup"><span data-stu-id="512eb-120">anywhere</span></span>|<span data-ttu-id="512eb-121">1/3</span><span class="sxs-lookup"><span data-stu-id="512eb-121">3</span></span>|<span data-ttu-id="512eb-122">任意の場所からアプリを実行できます。</span><span class="sxs-lookup"><span data-stu-id="512eb-122">Apps from anywhere can be run.</span></span>|




