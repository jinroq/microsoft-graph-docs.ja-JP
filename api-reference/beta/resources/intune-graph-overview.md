---
title: Intune Graph API の使用
description: " Intune ハイブリッド展開はサポートされていません。 "
ms.openlocfilehash: 2502b5209e9935fc923570947c38c0467534f4ef
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071319"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="accae-103">Microsoft Graph での Intune の操作</span><span class="sxs-lookup"><span data-stu-id="accae-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="accae-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="accae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="accae-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="accae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="accae-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="accae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="accae-107">Intune 用 Microsoft Graph API を使用すると、テナントの Intune の情報へのプログラムによるアクセスが可能となります。API は **Azure Portal** で使用できるものと同じ Intune 操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="accae-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="accae-108">モバイル デバイス管理 (MDM) のシナリオの場合、Intune 用 Graph API はスタンドアロンの展開をサポートします。Intune の[ハイブリッド展開](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="accae-108">For mobile device management (MDM) scenarios, the Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-intune-graph-api"></a><span data-ttu-id="accae-109">Intune Graph API の使用</span><span class="sxs-lookup"><span data-stu-id="accae-109">Using the Intune Graph API</span></span>

<span data-ttu-id="accae-110">Intune は、他のクラウド サービスには、エンティティの豊富な情報との関係のナビゲーションを使用して、データをグラフと同じ方法で提供します。</span><span class="sxs-lookup"><span data-stu-id="accae-110">Intune provides data into the Microsoft Graph in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="accae-111">Intune IT プロフェッショナルやエンドユーザーのサービス間の豊富なアプリケーションを構築するのに他のサービスから情報を結合するのにには、Microsoft Graph を使用します。</span><span class="sxs-lookup"><span data-stu-id="accae-111">  Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="accae-112">以下に、アプリケーションがユーザーのデバイスにインストールされているかどうかを判断する方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="accae-112">Here is an example of how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="accae-113">Azure Active Directory から、ユーザーに登録されているデバイスのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="accae-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="accae-114">次に、テナントのアプリケーションのリストを表示します。</span><span class="sxs-lookup"><span data-stu-id="accae-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="accae-115">アプリケーションから ID を取得し、アプリケーション (そしてユーザー) のインストール状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="accae-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-graph-permission-scopes"></a><span data-ttu-id="accae-116">グラフのためのアクセス許可のスコープを使用します。</span><span class="sxs-lookup"><span data-stu-id="accae-116">Using Graph permission scopes</span></span>

<span data-ttu-id="accae-117">Microsof のグラフでは、アクセス許可のスコープを使用するリソースへのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="accae-117">Microsof Graph controls access to resources using permission scopes.</span></span> <span data-ttu-id="accae-118">開発者は、Intune リソースにアクセスするために必要となる、アクセス許可のスコープを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="accae-118">As a developer, you must specify the permission scopes you need to access Intune resources.</span></span> <span data-ttu-id="accae-119">通常は Azure Active Directory ポータルで必要なアクセス許可のスコープを指定します。</span><span class="sxs-lookup"><span data-stu-id="accae-119">Typically, you specify the permission scopes you need in the Azure Active Directory portal.</span></span> <span data-ttu-id="accae-120">詳細については、「[Microsoft Graph のアクセス許可スコープ](https://developer.microsoft.com/graph/docs/authorization/permission_scopes)」および「[Intune のアクセス許可のスコープ](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="accae-120">For more information, see [Microsoft Graph permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) and [Intune permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span></span>

## <a name="to-use-the-table-of-contents-on-the-microsoft-graph-site"></a><span data-ttu-id="accae-121">Graph のサイトの内容のテーブルを使用するには</span><span class="sxs-lookup"><span data-stu-id="accae-121">To use the Table of Contents on the Microsoft Graph site</span></span>
  
<span data-ttu-id="accae-122">Intune グラフ API とリソースを表示するドキュメントのパーツを検索する (サイトの左側のペイン) の目次を参照できます。</span><span class="sxs-lookup"><span data-stu-id="accae-122">You can browse the Table of Contents (in the left pane of the site) to find the parts of the Intune Graph API and resource documentation you want to see.</span></span>

1. <span data-ttu-id="accae-123">ベータ版ドキュメントを開くには、 **/Beta 参照**をクリックします。</span><span class="sxs-lookup"><span data-stu-id="accae-123">Click **/Beta Reference** to open the beta docs.</span></span>
2. <span data-ttu-id="accae-124">下にスクロールし、 **Intune**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="accae-124">Scroll down and click **Intune**.</span></span>
3. <span data-ttu-id="accae-125">API の部分の**Intune**の下のサブセクションをクリックします。</span><span class="sxs-lookup"><span data-stu-id="accae-125">Continue to click subsections below **Intune** for the parts of the API you</span></span> 
