---
title: macOSGatekeeperAppSources 列挙型
description: MacOS ゲートキーパーのアプリソースオプション。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5e1fe83f05bfd7d0619f4eea62970305fc467e05
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365042"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="83157-103">macOSGatekeeperAppSources 列挙型</span><span class="sxs-lookup"><span data-stu-id="83157-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="83157-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83157-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83157-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="83157-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83157-106">MacOS ゲートキーパーのアプリソースオプション。</span><span class="sxs-lookup"><span data-stu-id="83157-106">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="83157-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="83157-107">Members</span></span>
|<span data-ttu-id="83157-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="83157-108">Member</span></span>|<span data-ttu-id="83157-109">値</span><span class="sxs-lookup"><span data-stu-id="83157-109">Value</span></span>|<span data-ttu-id="83157-110">説明</span><span class="sxs-lookup"><span data-stu-id="83157-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83157-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="83157-111">notConfigured</span></span>|<span data-ttu-id="83157-112">.0</span><span class="sxs-lookup"><span data-stu-id="83157-112">0</span></span>|<span data-ttu-id="83157-113">デバイスの既定値。意図的ではありません。</span><span class="sxs-lookup"><span data-stu-id="83157-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="83157-114">macAppStore</span><span class="sxs-lookup"><span data-stu-id="83157-114">macAppStore</span></span>|<span data-ttu-id="83157-115">1-d</span><span class="sxs-lookup"><span data-stu-id="83157-115">1</span></span>|<span data-ttu-id="83157-116">Mac AppStore からのアプリのみを実行できます。</span><span class="sxs-lookup"><span data-stu-id="83157-116">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="83157-117">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="83157-117">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="83157-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="83157-118">2</span></span>|<span data-ttu-id="83157-119">Mac AppStore のアプリのみを実行することができます。</span><span class="sxs-lookup"><span data-stu-id="83157-119">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="83157-120">箇所</span><span class="sxs-lookup"><span data-stu-id="83157-120">anywhere</span></span>|<span data-ttu-id="83157-121">1/3</span><span class="sxs-lookup"><span data-stu-id="83157-121">3</span></span>|<span data-ttu-id="83157-122">任意の場所からアプリを実行できます。</span><span class="sxs-lookup"><span data-stu-id="83157-122">Apps from anywhere can be run.</span></span>|



