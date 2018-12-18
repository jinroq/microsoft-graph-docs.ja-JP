---
title: appListType 列挙型
description: 準拠のアプリケーションのリストで使用できる値です。
author: tfitzmac
ms.openlocfilehash: 3f0fa162131fc1f59beba1f057fa888e0f2260c5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331193"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="eb875-103">appListType 列挙型</span><span class="sxs-lookup"><span data-stu-id="eb875-103">appListType enum type</span></span>

> <span data-ttu-id="eb875-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eb875-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eb875-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eb875-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eb875-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eb875-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eb875-107">準拠のアプリケーションのリストで使用できる値です。</span><span class="sxs-lookup"><span data-stu-id="eb875-107">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="eb875-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="eb875-108">Members</span></span>
|<span data-ttu-id="eb875-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="eb875-109">Member</span></span>|<span data-ttu-id="eb875-110">値</span><span class="sxs-lookup"><span data-stu-id="eb875-110">Value</span></span>|<span data-ttu-id="eb875-111">説明</span><span class="sxs-lookup"><span data-stu-id="eb875-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb875-112">none</span><span class="sxs-lookup"><span data-stu-id="eb875-112">none</span></span>|<span data-ttu-id="eb875-113">0</span><span class="sxs-lookup"><span data-stu-id="eb875-113">0</span></span>|<span data-ttu-id="eb875-114">既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="eb875-114">Default value, no intent.</span></span>|
|<span data-ttu-id="eb875-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="eb875-115">appsInListCompliant</span></span>|<span data-ttu-id="eb875-116">1</span><span class="sxs-lookup"><span data-stu-id="eb875-116">1</span></span>|<span data-ttu-id="eb875-117">一覧は、考慮される準拠 (準拠では、リスト上のアプリ) 専用のアプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="eb875-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="eb875-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="eb875-118">appsNotInListCompliant</span></span>|<span data-ttu-id="eb875-119">2</span><span class="sxs-lookup"><span data-stu-id="eb875-119">2</span></span>|<span data-ttu-id="eb875-120">リストと見なされます非準拠のアプリケーションを表します (すべてのアプリケーション準拠では、リスト上のアプリを除く)。</span><span class="sxs-lookup"><span data-stu-id="eb875-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





