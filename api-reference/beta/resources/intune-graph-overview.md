---
title: Intune Graph API の使用
description: " Intune ハイブリッド展開はサポートされていません。 "
author: tfitzmac
localization_priority: Priority
ms.openlocfilehash: 606c2324476492f8dc9271646d0109bb3d57de99
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869714"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="7a487-103">Microsoft Graph での Intune の操作</span><span class="sxs-lookup"><span data-stu-id="7a487-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="7a487-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7a487-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7a487-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a487-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7a487-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7a487-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="7a487-107">Intune 用 Microsoft Graph API を使用すると、テナントの Intune の情報へのプログラムによるアクセスが可能となります。API は **Azure Portal** で使用できるものと同じ Intune 操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="7a487-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="7a487-108">モバイル デバイス管理 (MDM) の場合は、Intune の Microsoft グラフ API は、スタンドアロン導入をサポートしています。Intune[ハイブリッド展開](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7a487-108">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="7a487-109">Intune の Graph API を使用します。</span><span class="sxs-lookup"><span data-stu-id="7a487-109">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="7a487-110">Intune は、他のクラウド サービスには、エンティティの豊富な情報との関係のナビゲーションを使用して、データをグラフと同じ方法で提供します。</span><span class="sxs-lookup"><span data-stu-id="7a487-110">Intune provides data into Microsoft Graph in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="7a487-111">Intune IT プロフェッショナルやエンドユーザーのサービス間の豊富なアプリケーションを構築するのに他のサービスから情報を結合するのにには、Microsoft Graph を使用します。</span><span class="sxs-lookup"><span data-stu-id="7a487-111"> Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="7a487-112">次の使用例は、アプリケーションがユーザーのデバイスにインストールされているかどうかを判断する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="7a487-112">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="7a487-113">Azure Active Directory から、ユーザーに登録されているデバイスのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="7a487-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="7a487-114">次に、テナントのアプリケーションのリストを表示します。</span><span class="sxs-lookup"><span data-stu-id="7a487-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="7a487-115">アプリケーションから ID を取得し、アプリケーション (そしてユーザー) のインストール状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="7a487-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a><span data-ttu-id="7a487-116">Graph のアクセス許可を使用します。</span><span class="sxs-lookup"><span data-stu-id="7a487-116">Using Microsoft Graph permissions</span></span>

<span data-ttu-id="7a487-117">Microsof のグラフでは、アクセス許可を使用してリソースへのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="7a487-117">Microsof Graph controls access to resources via permissions.</span></span> <span data-ttu-id="7a487-118">開発者は、Intune リソースにアクセスするアクセス許可を指定してください。</span><span class="sxs-lookup"><span data-stu-id="7a487-118">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="7a487-119">通常、Active Directory の Azure ポータルのアクセス許可を指定します。</span><span class="sxs-lookup"><span data-stu-id="7a487-119">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="7a487-120">詳細については、 [Microsoft Graph のアクセス許可のリファレンス](https://docs.microsoft.com/en-us/graph/permissions-reference)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7a487-120">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/en-us/graph/permissions-reference).</span></span>

## <a name="next-steps"></a><span data-ttu-id="7a487-121">次のステップ</span><span class="sxs-lookup"><span data-stu-id="7a487-121">Next Steps</span></span>

- <span data-ttu-id="7a487-122">Intune の Microsoft グラフ API にアクセスするのには[Azure AD を使用する方法](https://docs.microsoft.com/en-us/intune/intune-graph-apis)について説明します。</span><span class="sxs-lookup"><span data-stu-id="7a487-122">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="7a487-123">Intune の作業例のコンテキストで Microsoft グラフ API を使用する方法を表示する[PowerShell Intune のサンプル](https://github.com/microsoftgraph/powershell-intune-samples)を表示します。</span><span class="sxs-lookup"><span data-stu-id="7a487-123">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>

