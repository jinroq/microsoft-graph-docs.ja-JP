---
title: applicationGuardBlockClipboardSharingType 列挙型
description: ApplicationGuardBlockClipboardSharingType に指定できる値
author: tfitzmac
ms.openlocfilehash: af1843a8d7515e5ca14997256968942f485eab64
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304082"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="e7b49-103">applicationGuardBlockClipboardSharingType 列挙型</span><span class="sxs-lookup"><span data-stu-id="e7b49-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="e7b49-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7b49-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7b49-105">ApplicationGuardBlockClipboardSharingType に指定できる値</span><span class="sxs-lookup"><span data-stu-id="e7b49-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="e7b49-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="e7b49-106">Members</span></span>
|<span data-ttu-id="e7b49-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="e7b49-107">Member</span></span>|<span data-ttu-id="e7b49-108">値</span><span class="sxs-lookup"><span data-stu-id="e7b49-108">Value</span></span>|<span data-ttu-id="e7b49-109">説明</span><span class="sxs-lookup"><span data-stu-id="e7b49-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7b49-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e7b49-110">notConfigured</span></span>|<span data-ttu-id="e7b49-111">0</span><span class="sxs-lookup"><span data-stu-id="e7b49-111">0</span></span>|<span data-ttu-id="e7b49-112">構成されていません</span><span class="sxs-lookup"><span data-stu-id="e7b49-112">Not Configured</span></span>|
|<span data-ttu-id="e7b49-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="e7b49-113">blockBoth</span></span>|<span data-ttu-id="e7b49-114">1</span><span class="sxs-lookup"><span data-stu-id="e7b49-114">1</span></span>|<span data-ttu-id="e7b49-115">ブロックのクリップボード データのコンテナーにホストとホスト コンテナーの両方を共有するには</span><span class="sxs-lookup"><span data-stu-id="e7b49-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="e7b49-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="e7b49-116">blockHostToContainer</span></span>|<span data-ttu-id="e7b49-117">2</span><span class="sxs-lookup"><span data-stu-id="e7b49-117">2</span></span>|<span data-ttu-id="e7b49-118">コンテナーにホストからのデータを共有するためのブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="e7b49-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="e7b49-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="e7b49-119">blockContainerToHost</span></span>|<span data-ttu-id="e7b49-120">3</span><span class="sxs-lookup"><span data-stu-id="e7b49-120">3</span></span>|<span data-ttu-id="e7b49-121">コンテナーからホストへのデータを共有するためのブロックのクリップボード</span><span class="sxs-lookup"><span data-stu-id="e7b49-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="e7b49-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="e7b49-122">blockNone</span></span>|<span data-ttu-id="e7b49-123">4</span><span class="sxs-lookup"><span data-stu-id="e7b49-123">4</span></span>|<span data-ttu-id="e7b49-124">ブロックのクリップボード データのコンテナーにホストもホストするためのコンテナーを共有するには</span><span class="sxs-lookup"><span data-stu-id="e7b49-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



