---
title: appListType 列挙型
description: 準拠のアプリケーションのリストで使用できる値です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1439ab860ab6a1fbf9ff4deb30320bb57fba338
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967239"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="a1daa-103">appListType 列挙型</span><span class="sxs-lookup"><span data-stu-id="a1daa-103">appListType enum type</span></span>

> <span data-ttu-id="a1daa-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a1daa-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1daa-105">準拠のアプリケーションのリストで使用できる値です。</span><span class="sxs-lookup"><span data-stu-id="a1daa-105">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="a1daa-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="a1daa-106">Members</span></span>
|<span data-ttu-id="a1daa-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="a1daa-107">Member</span></span>|<span data-ttu-id="a1daa-108">値</span><span class="sxs-lookup"><span data-stu-id="a1daa-108">Value</span></span>|<span data-ttu-id="a1daa-109">説明</span><span class="sxs-lookup"><span data-stu-id="a1daa-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1daa-110">none</span><span class="sxs-lookup"><span data-stu-id="a1daa-110">none</span></span>|<span data-ttu-id="a1daa-111">0</span><span class="sxs-lookup"><span data-stu-id="a1daa-111">0</span></span>|<span data-ttu-id="a1daa-112">既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="a1daa-112">Default value, no intent.</span></span>|
|<span data-ttu-id="a1daa-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="a1daa-113">appsInListCompliant</span></span>|<span data-ttu-id="a1daa-114">1</span><span class="sxs-lookup"><span data-stu-id="a1daa-114">1</span></span>|<span data-ttu-id="a1daa-115">一覧は、考慮される準拠 (準拠では、リスト上のアプリ) 専用のアプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="a1daa-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="a1daa-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="a1daa-116">appsNotInListCompliant</span></span>|<span data-ttu-id="a1daa-117">2</span><span class="sxs-lookup"><span data-stu-id="a1daa-117">2</span></span>|<span data-ttu-id="a1daa-118">リストと見なされます非準拠のアプリケーションを表します (すべてのアプリケーション準拠では、リスト上のアプリを除く)。</span><span class="sxs-lookup"><span data-stu-id="a1daa-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



