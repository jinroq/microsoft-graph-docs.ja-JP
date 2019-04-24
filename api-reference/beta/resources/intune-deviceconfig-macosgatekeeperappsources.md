---
title: macOSGatekeeperAppSources 列挙型
description: macOS ゲートキーパーのアプリソースオプション。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dbe261b223a180f64016d41495a0f4fcec22868
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460631"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="45ad7-103">macOSGatekeeperAppSources 列挙型</span><span class="sxs-lookup"><span data-stu-id="45ad7-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="45ad7-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45ad7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45ad7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="45ad7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45ad7-106">macOS ゲートキーパーのアプリソースオプション。</span><span class="sxs-lookup"><span data-stu-id="45ad7-106">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="45ad7-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="45ad7-107">Members</span></span>
|<span data-ttu-id="45ad7-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="45ad7-108">Member</span></span>|<span data-ttu-id="45ad7-109">値</span><span class="sxs-lookup"><span data-stu-id="45ad7-109">Value</span></span>|<span data-ttu-id="45ad7-110">説明</span><span class="sxs-lookup"><span data-stu-id="45ad7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45ad7-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="45ad7-111">notConfigured</span></span>|<span data-ttu-id="45ad7-112">.0</span><span class="sxs-lookup"><span data-stu-id="45ad7-112">0</span></span>|<span data-ttu-id="45ad7-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="45ad7-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="45ad7-114">macappstore</span><span class="sxs-lookup"><span data-stu-id="45ad7-114">macAppStore</span></span>|<span data-ttu-id="45ad7-115">1-d</span><span class="sxs-lookup"><span data-stu-id="45ad7-115">1</span></span>|<span data-ttu-id="45ad7-116">Mac appstore からのアプリのみを実行できます。</span><span class="sxs-lookup"><span data-stu-id="45ad7-116">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="45ad7-117">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="45ad7-117">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="45ad7-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="45ad7-118">2</span></span>|<span data-ttu-id="45ad7-119">Mac appstore のアプリのみを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="45ad7-119">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="45ad7-120">箇所</span><span class="sxs-lookup"><span data-stu-id="45ad7-120">anywhere</span></span>|<span data-ttu-id="45ad7-121">1/3</span><span class="sxs-lookup"><span data-stu-id="45ad7-121">3</span></span>|<span data-ttu-id="45ad7-122">任意の場所からアプリを実行できます。</span><span class="sxs-lookup"><span data-stu-id="45ad7-122">Apps from anywhere can be run.</span></span>|





