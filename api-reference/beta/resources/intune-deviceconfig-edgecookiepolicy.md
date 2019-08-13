---
title: edgeCookiePolicy 列挙型
description: Microsoft Edge で許可する cookie を指定するための値。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c08748b271b56b2fcd0f7c0a7868d9c054ef794c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332618"
---
# <a name="edgecookiepolicy-enum-type"></a><span data-ttu-id="a8f34-103">edgeCookiePolicy 列挙型</span><span class="sxs-lookup"><span data-stu-id="a8f34-103">edgeCookiePolicy enum type</span></span>

> <span data-ttu-id="a8f34-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8f34-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8f34-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8f34-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8f34-106">Microsoft Edge で許可する cookie を指定するための値。</span><span class="sxs-lookup"><span data-stu-id="a8f34-106">Possible values to specify which cookies are allowed in Microsoft Edge.</span></span>

## <a name="members"></a><span data-ttu-id="a8f34-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a8f34-107">Members</span></span>
|<span data-ttu-id="a8f34-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="a8f34-108">Member</span></span>|<span data-ttu-id="a8f34-109">値</span><span class="sxs-lookup"><span data-stu-id="a8f34-109">Value</span></span>|<span data-ttu-id="a8f34-110">説明</span><span class="sxs-lookup"><span data-stu-id="a8f34-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8f34-111">自分のもの</span><span class="sxs-lookup"><span data-stu-id="a8f34-111">userDefined</span></span>|<span data-ttu-id="a8f34-112">.0</span><span class="sxs-lookup"><span data-stu-id="a8f34-112">0</span></span>|<span data-ttu-id="a8f34-113">ユーザーがを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="a8f34-113">Allow the user to set.</span></span>|
|<span data-ttu-id="a8f34-114">使う</span><span class="sxs-lookup"><span data-stu-id="a8f34-114">allow</span></span>|<span data-ttu-id="a8f34-115">1-d</span><span class="sxs-lookup"><span data-stu-id="a8f34-115">1</span></span>|<span data-ttu-id="a8f34-116">使う.</span><span class="sxs-lookup"><span data-stu-id="a8f34-116">Allow.</span></span>|
|<span data-ttu-id="a8f34-117">blockThirdParty</span><span class="sxs-lookup"><span data-stu-id="a8f34-117">blockThirdParty</span></span>|<span data-ttu-id="a8f34-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="a8f34-118">2</span></span>|<span data-ttu-id="a8f34-119">サードパーティの cookie のみをブロックします。</span><span class="sxs-lookup"><span data-stu-id="a8f34-119">Block only third party cookies.</span></span>|
|<span data-ttu-id="a8f34-120">blockAll</span><span class="sxs-lookup"><span data-stu-id="a8f34-120">blockAll</span></span>|<span data-ttu-id="a8f34-121">1/3</span><span class="sxs-lookup"><span data-stu-id="a8f34-121">3</span></span>|<span data-ttu-id="a8f34-122">すべての cookie をブロックします。</span><span class="sxs-lookup"><span data-stu-id="a8f34-122">Block all cookies.</span></span>|



