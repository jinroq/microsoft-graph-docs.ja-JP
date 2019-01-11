---
title: windowsPrivacyDataAccessLevel 列挙型
description: Windows プライバシー データの特定のカテゴリへのアクセス レベルを決定します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 74ab32a703422203fec7a6c9ed1bc035e01949a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888775"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="6cba4-103">windowsPrivacyDataAccessLevel 列挙型</span><span class="sxs-lookup"><span data-stu-id="6cba4-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="6cba4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6cba4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6cba4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6cba4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6cba4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6cba4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cba4-107">Windows プライバシー データの特定のカテゴリへのアクセス レベルを決定します。</span><span class="sxs-lookup"><span data-stu-id="6cba4-107">Determine the access level to specific Windows privacy data category.</span></span>
## <a name="members"></a><span data-ttu-id="6cba4-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="6cba4-108">Members</span></span>
|<span data-ttu-id="6cba4-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="6cba4-109">Member</span></span>|<span data-ttu-id="6cba4-110">値</span><span class="sxs-lookup"><span data-stu-id="6cba4-110">Value</span></span>|<span data-ttu-id="6cba4-111">説明</span><span class="sxs-lookup"><span data-stu-id="6cba4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cba4-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6cba4-112">notConfigured</span></span>|<span data-ttu-id="6cba4-113">0</span><span class="sxs-lookup"><span data-stu-id="6cba4-113">0</span></span>|<span data-ttu-id="6cba4-114">目的なしアクセス レベルが指定されませんでした。</span><span class="sxs-lookup"><span data-stu-id="6cba4-114">No access level specified, no intents.</span></span> <span data-ttu-id="6cba4-115">デバイスは、UserInControl や ForceAllow のように動作可能性があります。</span><span class="sxs-lookup"><span data-stu-id="6cba4-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="6cba4-116">プライバシー ・ データによりますが、されたバージョンの Windows およびその他の要素にアクセスします。</span><span class="sxs-lookup"><span data-stu-id="6cba4-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="6cba4-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="6cba4-117">forceAllow</span></span>|<span data-ttu-id="6cba4-118">1</span><span class="sxs-lookup"><span data-stu-id="6cba4-118">1</span></span>|<span data-ttu-id="6cba4-119">アプリケーションは、指定したプライバシー データへのアクセスが許可されます。</span><span class="sxs-lookup"><span data-stu-id="6cba4-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="6cba4-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="6cba4-120">forceDeny</span></span>|<span data-ttu-id="6cba4-121">2</span><span class="sxs-lookup"><span data-stu-id="6cba4-121">2</span></span>|<span data-ttu-id="6cba4-122">指定したプライバシー ・ データにアクセスするアプリケーションは拒否されます。</span><span class="sxs-lookup"><span data-stu-id="6cba4-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="6cba4-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="6cba4-123">userInControl</span></span>|<span data-ttu-id="6cba4-124">3</span><span class="sxs-lookup"><span data-stu-id="6cba4-124">3</span></span>|<span data-ttu-id="6cba4-125">アプリケーションが指定したプライバシー ・ データにアクセスしようとした場合、ユーザーが要求されます。</span><span class="sxs-lookup"><span data-stu-id="6cba4-125">Users will be prompted when apps try to access specified privacy data.</span></span>|





