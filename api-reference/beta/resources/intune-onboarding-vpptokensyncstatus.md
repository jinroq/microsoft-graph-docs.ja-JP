---
title: vppTokenSyncStatus 列挙型
description: Apple Volume Purchase Program のトークンに関連付けられている同期状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ede152d056c082e3b55c9142730ce61af86ae48c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369347"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="41d48-103">vppTokenSyncStatus 列挙型</span><span class="sxs-lookup"><span data-stu-id="41d48-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="41d48-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41d48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41d48-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="41d48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41d48-106">Apple Volume Purchase Program のトークンに関連付けられている同期状態。</span><span class="sxs-lookup"><span data-stu-id="41d48-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="41d48-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="41d48-107">Members</span></span>
|<span data-ttu-id="41d48-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="41d48-108">Member</span></span>|<span data-ttu-id="41d48-109">値</span><span class="sxs-lookup"><span data-stu-id="41d48-109">Value</span></span>|<span data-ttu-id="41d48-110">説明</span><span class="sxs-lookup"><span data-stu-id="41d48-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41d48-111">none</span><span class="sxs-lookup"><span data-stu-id="41d48-111">none</span></span>|<span data-ttu-id="41d48-112">.0</span><span class="sxs-lookup"><span data-stu-id="41d48-112">0</span></span>|<span data-ttu-id="41d48-113">既定の状態です。</span><span class="sxs-lookup"><span data-stu-id="41d48-113">Default status.</span></span>|
|<span data-ttu-id="41d48-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="41d48-114">inProgress</span></span>|<span data-ttu-id="41d48-115">1-d</span><span class="sxs-lookup"><span data-stu-id="41d48-115">1</span></span>|<span data-ttu-id="41d48-116">前回の同期が進行中です。</span><span class="sxs-lookup"><span data-stu-id="41d48-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="41d48-117">せ</span><span class="sxs-lookup"><span data-stu-id="41d48-117">completed</span></span>|<span data-ttu-id="41d48-118">pbm-2</span><span class="sxs-lookup"><span data-stu-id="41d48-118">2</span></span>|<span data-ttu-id="41d48-119">前回の同期が正常に完了しました。</span><span class="sxs-lookup"><span data-stu-id="41d48-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="41d48-120">フェール</span><span class="sxs-lookup"><span data-stu-id="41d48-120">failed</span></span>|<span data-ttu-id="41d48-121">1/3</span><span class="sxs-lookup"><span data-stu-id="41d48-121">3</span></span>|<span data-ttu-id="41d48-122">前回の同期に失敗しました。</span><span class="sxs-lookup"><span data-stu-id="41d48-122">Last Sync failed.</span></span>|



