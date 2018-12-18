---
title: appListType 列挙型
description: 準拠のアプリケーションのリストで使用できる値です。
author: tfitzmac
ms.openlocfilehash: ab5d8f45343b017693906b13be25c88d5b06e8f7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27354720"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="49de5-103">appListType 列挙型</span><span class="sxs-lookup"><span data-stu-id="49de5-103">appListType enum type</span></span>

> <span data-ttu-id="49de5-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="49de5-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49de5-105">準拠のアプリケーションのリストで使用できる値です。</span><span class="sxs-lookup"><span data-stu-id="49de5-105">Possible values of the compliance app list.</span></span>
## <a name="members"></a><span data-ttu-id="49de5-106">メンバー</span><span class="sxs-lookup"><span data-stu-id="49de5-106">Members</span></span>
|<span data-ttu-id="49de5-107">メンバー</span><span class="sxs-lookup"><span data-stu-id="49de5-107">Member</span></span>|<span data-ttu-id="49de5-108">値</span><span class="sxs-lookup"><span data-stu-id="49de5-108">Value</span></span>|<span data-ttu-id="49de5-109">説明</span><span class="sxs-lookup"><span data-stu-id="49de5-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49de5-110">none</span><span class="sxs-lookup"><span data-stu-id="49de5-110">none</span></span>|<span data-ttu-id="49de5-111">0</span><span class="sxs-lookup"><span data-stu-id="49de5-111">0</span></span>|<span data-ttu-id="49de5-112">既定値でことを目的しません。</span><span class="sxs-lookup"><span data-stu-id="49de5-112">Default value, no intent.</span></span>|
|<span data-ttu-id="49de5-113">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="49de5-113">appsInListCompliant</span></span>|<span data-ttu-id="49de5-114">1</span><span class="sxs-lookup"><span data-stu-id="49de5-114">1</span></span>|<span data-ttu-id="49de5-115">一覧は、考慮される準拠 (準拠では、リスト上のアプリ) 専用のアプリケーションを表します。</span><span class="sxs-lookup"><span data-stu-id="49de5-115">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="49de5-116">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="49de5-116">appsNotInListCompliant</span></span>|<span data-ttu-id="49de5-117">2</span><span class="sxs-lookup"><span data-stu-id="49de5-117">2</span></span>|<span data-ttu-id="49de5-118">リストと見なされます非準拠のアプリケーションを表します (すべてのアプリケーション準拠では、リスト上のアプリを除く)。</span><span class="sxs-lookup"><span data-stu-id="49de5-118">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|



