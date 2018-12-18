---
title: Intune Graph API の使用
description: " Intune ハイブリッド展開はサポートされていません。 "
author: tfitzmac
ms.openlocfilehash: 9ac823fcc1e3c09bfedc57d9caf4901c95aa9142
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332733"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="fead8-103">Microsoft Graph での Intune の操作</span><span class="sxs-lookup"><span data-stu-id="fead8-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="fead8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fead8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="fead8-105">Intune 用 Microsoft Graph API を使用すると、テナントの Intune の情報へのプログラムによるアクセスが可能となります。API は **Azure Portal** で使用できるものと同じ Intune 操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="fead8-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="fead8-106">モバイル デバイス管理 (MDM) の場合は、Intune の Microsoft グラフ API は、スタンドアロン導入をサポートしています。Intune[ハイブリッド展開](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fead8-106">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="fead8-107">Intune の Graph API を使用します。</span><span class="sxs-lookup"><span data-stu-id="fead8-107">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="fead8-108">Intune は、豊富なエンティティ情報とリレーションシップのナビゲーションを使用して、他のクラウド サービスと同じ方法で Microsoft Graph API にデータを提供します。</span><span class="sxs-lookup"><span data-stu-id="fead8-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="fead8-109">Microsoft グラフ API を使用すると、他のサービスや IT プロフェッショナルやエンドユーザーのサービス間の豊富なアプリケーションを構築するのに Intune から情報を結合します。</span><span class="sxs-lookup"><span data-stu-id="fead8-109"> Use the Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="fead8-110">次の使用例は、アプリケーションがユーザーのデバイスにインストールされているかどうかを判断する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="fead8-110">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="fead8-111">Azure Active Directory から、ユーザーに登録されているデバイスのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="fead8-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="fead8-112">次に、テナントのアプリケーションのリストを表示します。</span><span class="sxs-lookup"><span data-stu-id="fead8-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="fead8-113">アプリケーションから ID を取得し、アプリケーション (そしてユーザー) のインストール状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="fead8-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-permissions"></a><span data-ttu-id="fead8-114">アクセス許可を使用します。</span><span class="sxs-lookup"><span data-stu-id="fead8-114">Using permissions</span></span>

<span data-ttu-id="fead8-115">Microsoft グラフ API は、アクセス許可を使用してリソースへのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="fead8-115">The Microsoft Graph API controls access to resources via permissions.</span></span> <span data-ttu-id="fead8-116">開発者は、Intune リソースにアクセスするアクセス許可を指定してください。</span><span class="sxs-lookup"><span data-stu-id="fead8-116">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="fead8-117">通常、Active Directory の Azure ポータルのアクセス許可を指定します。</span><span class="sxs-lookup"><span data-stu-id="fead8-117">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="fead8-118">詳細については、 [Microsoft Graph のアクセス許可のリファレンス](https://docs.microsoft.com/en-us/graph/permissions-reference)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fead8-118">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/en-us/graph/permissions-reference).</span></span>

## <a name="next-steps"></a><span data-ttu-id="fead8-119">次のステップ</span><span class="sxs-lookup"><span data-stu-id="fead8-119">Next Steps</span></span>

- <span data-ttu-id="fead8-120">Intune の Microsoft グラフ API にアクセスするのには[Azure AD を使用する方法](https://docs.microsoft.com/en-us/intune/intune-graph-apis)について説明します。</span><span class="sxs-lookup"><span data-stu-id="fead8-120">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="fead8-121">Intune の作業例のコンテキストで Microsoft グラフ API を使用する方法を表示する[PowerShell Intune のサンプル](https://github.com/microsoftgraph/powershell-intune-samples)を表示します。</span><span class="sxs-lookup"><span data-stu-id="fead8-121">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>
