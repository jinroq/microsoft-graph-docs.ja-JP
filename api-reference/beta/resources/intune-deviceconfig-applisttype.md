---
title: appListType 列挙型
description: 準拠のアプリケーションのリストで使用できる値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: eb2b4afa6639d70b81a59bda1250ea9ed231ccdb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939645"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="c5d64-103">appListType 列挙型</span><span class="sxs-lookup"><span data-stu-id="c5d64-103">appListType enum type</span></span>

> <span data-ttu-id="c5d64-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c5d64-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c5d64-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5d64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c5d64-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5d64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c5d64-107">準拠のアプリケーションのリストで使用できる値です。</span><span class="sxs-lookup"><span data-stu-id="c5d64-107">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="c5d64-108">メンバー</span><span class="sxs-lookup"><span data-stu-id="c5d64-108">Members</span></span>
|<span data-ttu-id="c5d64-109">メンバー</span><span class="sxs-lookup"><span data-stu-id="c5d64-109">Member</span></span>|<span data-ttu-id="c5d64-110">値</span><span class="sxs-lookup"><span data-stu-id="c5d64-110">Value</span></span>|<span data-ttu-id="c5d64-111">説明</span><span class="sxs-lookup"><span data-stu-id="c5d64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5d64-112">none</span><span class="sxs-lookup"><span data-stu-id="c5d64-112">none</span></span>|<span data-ttu-id="c5d64-113">0</span><span class="sxs-lookup"><span data-stu-id="c5d64-113">0</span></span>|<span data-ttu-id="c5d64-114">既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="c5d64-114">Default value, no intent.</span></span>|
|<span data-ttu-id="c5d64-115">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="c5d64-115">appsInListCompliant</span></span>|<span data-ttu-id="c5d64-116">1</span><span class="sxs-lookup"><span data-stu-id="c5d64-116">1</span></span>|<span data-ttu-id="c5d64-117">一覧は、考慮される準拠 (準拠では、リスト上のアプリ) 専用のアプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="c5d64-117">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="c5d64-118">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="c5d64-118">appsNotInListCompliant</span></span>|<span data-ttu-id="c5d64-119">2</span><span class="sxs-lookup"><span data-stu-id="c5d64-119">2</span></span>|<span data-ttu-id="c5d64-120">リストと見なされます非準拠のアプリケーションを表します (すべてのアプリケーション準拠では、リスト上のアプリを除く)。</span><span class="sxs-lookup"><span data-stu-id="c5d64-120">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





