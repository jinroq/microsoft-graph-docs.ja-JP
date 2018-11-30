---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値
ms.openlocfilehash: 27b3a48f91e9593ca0e4ebbf6d41ed2c289d20db
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069376"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="70003-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="70003-103">installIntent enum type</span></span>

> <span data-ttu-id="70003-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="70003-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="70003-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70003-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70003-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="70003-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70003-107">管理者が選択したインストールの目的に使用できる値</span><span class="sxs-lookup"><span data-stu-id="70003-107">Possible values for the install intent chosen by the admin.</span></span>
## <a name="members"></a><span data-ttu-id="70003-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="70003-108">Members</span></span>
|<span data-ttu-id="70003-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="70003-109">Member</span></span>|<span data-ttu-id="70003-110">値</span><span class="sxs-lookup"><span data-stu-id="70003-110">Value</span></span>|<span data-ttu-id="70003-111">説明</span><span class="sxs-lookup"><span data-stu-id="70003-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70003-112">使用可能</span><span class="sxs-lookup"><span data-stu-id="70003-112">available</span></span>|<span data-ttu-id="70003-113">0</span><span class="sxs-lookup"><span data-stu-id="70003-113">0</span></span>|<span data-ttu-id="70003-114">使用可能なインストールの目的です。</span><span class="sxs-lookup"><span data-stu-id="70003-114">Available install intent.</span></span>|
|<span data-ttu-id="70003-115">必須</span><span class="sxs-lookup"><span data-stu-id="70003-115">required</span></span>|<span data-ttu-id="70003-116">1</span><span class="sxs-lookup"><span data-stu-id="70003-116">1</span></span>|<span data-ttu-id="70003-117">目的のインストールが必要です。</span><span class="sxs-lookup"><span data-stu-id="70003-117">Required install intent.</span></span>|
|<span data-ttu-id="70003-118">アンインストール</span><span class="sxs-lookup"><span data-stu-id="70003-118">uninstall</span></span>|<span data-ttu-id="70003-119">2</span><span class="sxs-lookup"><span data-stu-id="70003-119">2</span></span>|<span data-ttu-id="70003-120">目的のインストールをアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="70003-120">Uninstall install intent.</span></span>|
|<span data-ttu-id="70003-121">availableWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="70003-121">availableWithoutEnrollment</span></span>|<span data-ttu-id="70003-122">3</span><span class="sxs-lookup"><span data-stu-id="70003-122">3</span></span>|<span data-ttu-id="70003-123">インストールの目的を登録しなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="70003-123">Available without enrollment install intent.</span></span>|





