---
title: macOSGatekeeperAppSources 列挙型
description: MacOS ゲートキーパーのアプリケーション ソースのオプションです。
author: tfitzmac
ms.openlocfilehash: 323c913cf9136e26a060d98e399806370700094d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342834"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="1fdfc-103">macOSGatekeeperAppSources 列挙型</span><span class="sxs-lookup"><span data-stu-id="1fdfc-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="1fdfc-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1fdfc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1fdfc-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1fdfc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1fdfc-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1fdfc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1fdfc-107">MacOS ゲートキーパーのアプリケーション ソースのオプションです。</span><span class="sxs-lookup"><span data-stu-id="1fdfc-107">App source options for macOS Gatekeeper.</span></span>
## <a name="members"></a><span data-ttu-id="1fdfc-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="1fdfc-108">Members</span></span>
|<span data-ttu-id="1fdfc-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="1fdfc-109">Member</span></span>|<span data-ttu-id="1fdfc-110">値</span><span class="sxs-lookup"><span data-stu-id="1fdfc-110">Value</span></span>|<span data-ttu-id="1fdfc-111">説明</span><span class="sxs-lookup"><span data-stu-id="1fdfc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fdfc-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1fdfc-112">notConfigured</span></span>|<span data-ttu-id="1fdfc-113">0</span><span class="sxs-lookup"><span data-stu-id="1fdfc-113">0</span></span>|<span data-ttu-id="1fdfc-114">デバイスの既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="1fdfc-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="1fdfc-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="1fdfc-115">macAppStore</span></span>|<span data-ttu-id="1fdfc-116">1</span><span class="sxs-lookup"><span data-stu-id="1fdfc-116">1</span></span>|<span data-ttu-id="1fdfc-117">Mac AppStore からのアプリのみを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="1fdfc-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="1fdfc-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="1fdfc-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="1fdfc-119">2</span><span class="sxs-lookup"><span data-stu-id="1fdfc-119">2</span></span>|<span data-ttu-id="1fdfc-120">Mac AppStore と識別された開発者からの唯一のアプリケーションを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="1fdfc-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="1fdfc-121">任意の場所</span><span class="sxs-lookup"><span data-stu-id="1fdfc-121">anywhere</span></span>|<span data-ttu-id="1fdfc-122">3</span><span class="sxs-lookup"><span data-stu-id="1fdfc-122">3</span></span>|<span data-ttu-id="1fdfc-123">任意の場所からアプリケーションを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="1fdfc-123">Apps from anywhere can be run.</span></span>|





