---
title: prereleaseFeatures 列挙型
description: 前のリリースの新機能の使用可能な値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 25d9f74247780779ec229aacdb732276fd3c4003
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27918169"
---
# <a name="prereleasefeatures-enum-type"></a><span data-ttu-id="ff1a0-103">prereleaseFeatures 列挙型</span><span class="sxs-lookup"><span data-stu-id="ff1a0-103">prereleaseFeatures enum type</span></span>

> <span data-ttu-id="ff1a0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ff1a0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ff1a0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff1a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ff1a0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ff1a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ff1a0-107">前のリリースの新機能の使用可能な値です。</span><span class="sxs-lookup"><span data-stu-id="ff1a0-107">Possible values for pre-release features.</span></span>
## <a name="members"></a><span data-ttu-id="ff1a0-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="ff1a0-108">Members</span></span>
|<span data-ttu-id="ff1a0-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="ff1a0-109">Member</span></span>|<span data-ttu-id="ff1a0-110">値</span><span class="sxs-lookup"><span data-stu-id="ff1a0-110">Value</span></span>|<span data-ttu-id="ff1a0-111">説明</span><span class="sxs-lookup"><span data-stu-id="ff1a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff1a0-112">ユーザー定義</span><span class="sxs-lookup"><span data-stu-id="ff1a0-112">userDefined</span></span>|<span data-ttu-id="ff1a0-113">0</span><span class="sxs-lookup"><span data-stu-id="ff1a0-113">0</span></span>|<span data-ttu-id="ff1a0-114">ユーザー定義、既定値、ない目的。</span><span class="sxs-lookup"><span data-stu-id="ff1a0-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ff1a0-115">settingsOnly</span><span class="sxs-lookup"><span data-stu-id="ff1a0-115">settingsOnly</span></span>|<span data-ttu-id="ff1a0-116">1</span><span class="sxs-lookup"><span data-stu-id="ff1a0-116">1</span></span>|<span data-ttu-id="ff1a0-117">リリースの前の機能を設定します。</span><span class="sxs-lookup"><span data-stu-id="ff1a0-117">Settings only pre-release features.</span></span>|
|<span data-ttu-id="ff1a0-118">settingsAndExperimentations</span><span class="sxs-lookup"><span data-stu-id="ff1a0-118">settingsAndExperimentations</span></span>|<span data-ttu-id="ff1a0-119">2</span><span class="sxs-lookup"><span data-stu-id="ff1a0-119">2</span></span>|<span data-ttu-id="ff1a0-120">前リリースの機能を設定し、実験しました。</span><span class="sxs-lookup"><span data-stu-id="ff1a0-120">Settings and experimentations pre-release features.</span></span>|
|<span data-ttu-id="ff1a0-121">notAllowed</span><span class="sxs-lookup"><span data-stu-id="ff1a0-121">notAllowed</span></span>|<span data-ttu-id="ff1a0-122">3</span><span class="sxs-lookup"><span data-stu-id="ff1a0-122">3</span></span>|<span data-ttu-id="ff1a0-123">前のリリースの新機能が許可されていません。</span><span class="sxs-lookup"><span data-stu-id="ff1a0-123">Pre-release features not allowed.</span></span>|





