---
title: macOSGatekeeperAppSources 列挙型
description: MacOS ゲートキーパーのアプリケーション ソースのオプションです。
ms.openlocfilehash: 97e8159c575c99fe142b67b4c6eeb24642cd0754
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072262"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="364b3-103">macOSGatekeeperAppSources 列挙型</span><span class="sxs-lookup"><span data-stu-id="364b3-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="364b3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="364b3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="364b3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="364b3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="364b3-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="364b3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="364b3-107">MacOS ゲートキーパーのアプリケーション ソースのオプションです。</span><span class="sxs-lookup"><span data-stu-id="364b3-107">App source options for macOS Gatekeeper.</span></span>
## <a name="members"></a><span data-ttu-id="364b3-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="364b3-108">Members</span></span>
|<span data-ttu-id="364b3-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="364b3-109">Member</span></span>|<span data-ttu-id="364b3-110">値</span><span class="sxs-lookup"><span data-stu-id="364b3-110">Value</span></span>|<span data-ttu-id="364b3-111">説明</span><span class="sxs-lookup"><span data-stu-id="364b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="364b3-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="364b3-112">notConfigured</span></span>|<span data-ttu-id="364b3-113">0</span><span class="sxs-lookup"><span data-stu-id="364b3-113">0</span></span>|<span data-ttu-id="364b3-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="364b3-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="364b3-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="364b3-115">macAppStore</span></span>|<span data-ttu-id="364b3-116">1</span><span class="sxs-lookup"><span data-stu-id="364b3-116">1</span></span>|<span data-ttu-id="364b3-117">Mac AppStore からのアプリのみを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="364b3-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="364b3-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="364b3-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="364b3-119">2</span><span class="sxs-lookup"><span data-stu-id="364b3-119">2</span></span>|<span data-ttu-id="364b3-120">Mac AppStore と識別された開発者からの唯一のアプリケーションを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="364b3-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="364b3-121">任意の場所</span><span class="sxs-lookup"><span data-stu-id="364b3-121">anywhere</span></span>|<span data-ttu-id="364b3-122">3</span><span class="sxs-lookup"><span data-stu-id="364b3-122">3</span></span>|<span data-ttu-id="364b3-123">任意の場所からアプリケーションを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="364b3-123">Apps from anywhere can be run.</span></span>|





