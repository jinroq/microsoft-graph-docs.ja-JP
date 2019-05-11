---
title: macOSGatekeeperAppSources 列挙型
description: MacOS ゲートキーパーのアプリソースオプション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b178072bd4364b2fc0df813d5b8e56423c2b29fa
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946148"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="66187-103">macOSGatekeeperAppSources 列挙型</span><span class="sxs-lookup"><span data-stu-id="66187-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="66187-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66187-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66187-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="66187-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66187-106">MacOS ゲートキーパーのアプリソースオプション。</span><span class="sxs-lookup"><span data-stu-id="66187-106">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="66187-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="66187-107">Members</span></span>
|<span data-ttu-id="66187-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="66187-108">Member</span></span>|<span data-ttu-id="66187-109">値</span><span class="sxs-lookup"><span data-stu-id="66187-109">Value</span></span>|<span data-ttu-id="66187-110">説明</span><span class="sxs-lookup"><span data-stu-id="66187-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66187-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="66187-111">notConfigured</span></span>|<span data-ttu-id="66187-112">.0</span><span class="sxs-lookup"><span data-stu-id="66187-112">0</span></span>|<span data-ttu-id="66187-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="66187-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="66187-114">macAppStore</span><span class="sxs-lookup"><span data-stu-id="66187-114">macAppStore</span></span>|<span data-ttu-id="66187-115">1-d</span><span class="sxs-lookup"><span data-stu-id="66187-115">1</span></span>|<span data-ttu-id="66187-116">Mac AppStore からのアプリのみを実行できます。</span><span class="sxs-lookup"><span data-stu-id="66187-116">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="66187-117">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="66187-117">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="66187-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="66187-118">2</span></span>|<span data-ttu-id="66187-119">Mac AppStore のアプリのみを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="66187-119">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="66187-120">箇所</span><span class="sxs-lookup"><span data-stu-id="66187-120">anywhere</span></span>|<span data-ttu-id="66187-121">1/3</span><span class="sxs-lookup"><span data-stu-id="66187-121">3</span></span>|<span data-ttu-id="66187-122">任意の場所からアプリを実行できます。</span><span class="sxs-lookup"><span data-stu-id="66187-122">Apps from anywhere can be run.</span></span>|




