---
title: installIntent 列挙型
description: 管理者が選択したインストールの目的に使用できる値
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ff15f72c3f746eb433b050df61fc8f1bd73b7e89
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967057"
---
# <a name="installintent-enum-type"></a><span data-ttu-id="27cde-103">installIntent 列挙型</span><span class="sxs-lookup"><span data-stu-id="27cde-103">installIntent enum type</span></span>

> <span data-ttu-id="27cde-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="27cde-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27cde-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27cde-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="27cde-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="27cde-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27cde-107">管理者が選択したインストールの目的に使用できる値</span><span class="sxs-lookup"><span data-stu-id="27cde-107">Possible values for the install intent chosen by the admin.</span></span>
## <a name="members"></a><span data-ttu-id="27cde-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="27cde-108">Members</span></span>
|<span data-ttu-id="27cde-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="27cde-109">Member</span></span>|<span data-ttu-id="27cde-110">値</span><span class="sxs-lookup"><span data-stu-id="27cde-110">Value</span></span>|<span data-ttu-id="27cde-111">説明</span><span class="sxs-lookup"><span data-stu-id="27cde-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27cde-112">使用可能</span><span class="sxs-lookup"><span data-stu-id="27cde-112">available</span></span>|<span data-ttu-id="27cde-113">0</span><span class="sxs-lookup"><span data-stu-id="27cde-113">0</span></span>|<span data-ttu-id="27cde-114">使用可能なインストールの目的です。</span><span class="sxs-lookup"><span data-stu-id="27cde-114">Available install intent.</span></span>|
|<span data-ttu-id="27cde-115">必須</span><span class="sxs-lookup"><span data-stu-id="27cde-115">required</span></span>|<span data-ttu-id="27cde-116">1</span><span class="sxs-lookup"><span data-stu-id="27cde-116">1</span></span>|<span data-ttu-id="27cde-117">目的のインストールが必要です。</span><span class="sxs-lookup"><span data-stu-id="27cde-117">Required install intent.</span></span>|
|<span data-ttu-id="27cde-118">アンインストール</span><span class="sxs-lookup"><span data-stu-id="27cde-118">uninstall</span></span>|<span data-ttu-id="27cde-119">2</span><span class="sxs-lookup"><span data-stu-id="27cde-119">2</span></span>|<span data-ttu-id="27cde-120">目的のインストールをアンインストールします。</span><span class="sxs-lookup"><span data-stu-id="27cde-120">Uninstall install intent.</span></span>|
|<span data-ttu-id="27cde-121">availableWithoutEnrollment</span><span class="sxs-lookup"><span data-stu-id="27cde-121">availableWithoutEnrollment</span></span>|<span data-ttu-id="27cde-122">3</span><span class="sxs-lookup"><span data-stu-id="27cde-122">3</span></span>|<span data-ttu-id="27cde-123">インストールの目的を登録しなくても使用できます。</span><span class="sxs-lookup"><span data-stu-id="27cde-123">Available without enrollment install intent.</span></span>|





