---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fd64622fd9471c0aff9f9d50ef9c0ad1a9e2ef63
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874978"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="5cb50-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="5cb50-103">installIntent enum type</span></span>

> <span data-ttu-id="5cb50-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5cb50-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5cb50-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5cb50-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5cb50-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5cb50-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5cb50-107">管理者が選択したインストールの目的に使用できる値</span><span class="sxs-lookup"><span data-stu-id="5cb50-107">Possible values for the install intent chosen by the admin.</span></span>
## <a name="members"></a><span data-ttu-id="5cb50-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="5cb50-108">Members</span></span>
|<span data-ttu-id="5cb50-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="5cb50-109">Member</span></span>|<span data-ttu-id="5cb50-110">値</span><span class="sxs-lookup"><span data-stu-id="5cb50-110">Value</span></span>|<span data-ttu-id="5cb50-111">説明</span><span class="sxs-lookup"><span data-stu-id="5cb50-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cb50-112">使用可能</span><span class="sxs-lookup"><span data-stu-id="5cb50-112">available</span></span>|<span data-ttu-id="5cb50-113">0</span><span class="sxs-lookup"><span data-stu-id="5cb50-113">0</span></span>|<span data-ttu-id="5cb50-114">使用可能なインストールの目的です。</span><span class="sxs-lookup"><span data-stu-id="5cb50-114">Available install intent.</span></span>|
|<span data-ttu-id="5cb50-115">必須</span><span class="sxs-lookup"><span data-stu-id="5cb50-115">required</span></span>|<span data-ttu-id="5cb50-116">1</span><span class="sxs-lookup"><span data-stu-id="5cb50-116">1</span></span>|<span data-ttu-id="5cb50-117">目的のインストールが必要です。</span><span class="sxs-lookup"><span data-stu-id="5cb50-117">Required install intent.</span></span>|
|<span data-ttu-id="5cb50-118">アンインストール</span><span class="sxs-lookup"><span data-stu-id="5cb50-118">uninstall</span></span>|<span data-ttu-id="5cb50-119">2</span><span class="sxs-lookup"><span data-stu-id="5cb50-119">2</span></span>|<span data-ttu-id="5cb50-120">目的のインストールをアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="5cb50-120">Uninstall install intent.</span></span>|
|<span data-ttu-id="5cb50-121">availableWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="5cb50-121">availableWithoutEnrollment</span></span>|<span data-ttu-id="5cb50-122">3</span><span class="sxs-lookup"><span data-stu-id="5cb50-122">3</span></span>|<span data-ttu-id="5cb50-123">インストールの目的を登録しなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="5cb50-123">Available without enrollment install intent.</span></span>|





