---
title: Intune Graph API の使用
description: " Intune ハイブリッド展開はサポートされていません。 "
ms.openlocfilehash: 23f6550fca708b64357b7b5132a2a42060cfa4bd
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020175"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="dca3e-103">Microsoft Graph での Intune の操作</span><span class="sxs-lookup"><span data-stu-id="dca3e-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="dca3e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dca3e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="dca3e-105">Intune 用 Microsoft Graph API を使用すると、テナントの Intune の情報へのプログラムによるアクセスが可能となります。API は **Azure Portal** で使用できるものと同じ Intune 操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="dca3e-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="dca3e-106">モバイル デバイス管理 (MDM) のシナリオの場合、Intune 用 Graph API はスタンドアロンの展開をサポートします。Intune の[ハイブリッド展開](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dca3e-106">For mobile device management (MDM) scenarios, the Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-intune-graph-api"></a><span data-ttu-id="dca3e-107">Intune Graph API の使用</span><span class="sxs-lookup"><span data-stu-id="dca3e-107">Using the Intune Graph API</span></span>

<span data-ttu-id="dca3e-108">Intune は、豊富なエンティティ情報とリレーションシップのナビゲーションを使用して、他のクラウド サービスと同じ方法で Microsoft Graph API にデータを提供します。</span><span class="sxs-lookup"><span data-stu-id="dca3e-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="dca3e-109">Microsoft Graph API を使用して、他のサービスからの情報と Intune を結合し、IT プロフェッショナルやエンド ユーザー向けの豊富なサービス間アプリケーションをビルドします。</span><span class="sxs-lookup"><span data-stu-id="dca3e-109">  Use Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="dca3e-110">以下に、アプリケーションがユーザーのデバイスにインストールされているかどうかを判断する方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="dca3e-110">Here is an example of how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="dca3e-111">Azure Active Directory から、ユーザーに登録されているデバイスのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="dca3e-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="dca3e-112">次に、テナントのアプリケーションのリストを表示します。</span><span class="sxs-lookup"><span data-stu-id="dca3e-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="dca3e-113">アプリケーションから ID を取得し、アプリケーション (そしてユーザー) のインストール状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="dca3e-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permission-scopes"></a><span data-ttu-id="dca3e-114">アクセス許可のスコープの使用</span><span class="sxs-lookup"><span data-stu-id="dca3e-114">Using permission scopes</span></span>

<span data-ttu-id="dca3e-115">Microsoft Graph API では、アクセス許可のスコープによってリソースへのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="dca3e-115">Microsoft Graph API controls access to resources using permission scopes.</span></span> <span data-ttu-id="dca3e-116">開発者は、Intune リソースにアクセスするために必要となる、アクセス許可のスコープを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="dca3e-116">As a developer, you must specify the permission scopes you need to access Intune resources.</span></span> <span data-ttu-id="dca3e-117">通常は Azure Active Directory ポータルで必要なアクセス許可のスコープを指定します。</span><span class="sxs-lookup"><span data-stu-id="dca3e-117">Typically, you specify the permission scopes you need in the Azure Active Directory portal.</span></span> <span data-ttu-id="dca3e-118">詳細については、「[Microsoft Graph のアクセス許可スコープ](https://developer.microsoft.com/graph/docs/authorization/permission_scopes)」および「[Intune のアクセス許可のスコープ](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dca3e-118">For more information, see [Microsoft Graph permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) and [Intune permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes#permission-scopes-in-preview).</span></span>

## <a name="next-steps"></a><span data-ttu-id="dca3e-119">次の手順</span><span class="sxs-lookup"><span data-stu-id="dca3e-119">Next Steps</span></span>

- <span data-ttu-id="dca3e-120">Intune の Microsoft グラフ API にアクセスするのには[Azure AD を使用する方法](https://docs.microsoft.com/en-us/intune/intune-graph-apis)について説明します。</span><span class="sxs-lookup"><span data-stu-id="dca3e-120">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="dca3e-121">Intune の作業例のコンテキストでのグラフの API を使用する方法を表示する[PowerShell Intune のサンプル](https://github.com/microsoftgraph/powershell-intune-samples)を表示します。</span><span class="sxs-lookup"><span data-stu-id="dca3e-121">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use Graph API for Intune in context of working examples.</span></span>