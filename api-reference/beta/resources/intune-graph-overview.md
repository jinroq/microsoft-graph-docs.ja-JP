---
title: Intune Graph API の使用 - Microsoft Graph API
description: テナント組織、そのデバイス、アプリ、アクセス、リソースを管理するために使用できる、Intune エンドポイント用 Microsoft Graph API (REST) の一覧を示します。
author: tfitzmac
localization_priority: Priority
ms.prod: intune
ms.openlocfilehash: fc254772a5b4db131a5cda45fc83b336bf12f993
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575962"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="a310c-103">Microsoft Graph での Intune の操作</span><span class="sxs-lookup"><span data-stu-id="a310c-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="a310c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a310c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a310c-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a310c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a310c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/ja-JP/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a310c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/ja-JP/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="a310c-107">Intune 用 Microsoft Graph API を使用すると、テナントの Intune の情報へのプログラムによるアクセスが可能となります。API は **Azure Portal** で使用できるものと同じ Intune 操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="a310c-107">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="a310c-108">モバイル デバイス管理 (MDM) のシナリオの場合、Intune 用 Microsoft Graph API はスタンドアロンの展開をサポートします。Intune の[ハイブリッド展開](https://docs.microsoft.com/ja-JP/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a310c-108">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/ja-JP/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="a310c-109">Intune 用 Microsoft Graph API の使用</span><span class="sxs-lookup"><span data-stu-id="a310c-109">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="a310c-110">Intune は、豊富なエンティティ情報とリレーションシップのナビゲーションを使用して、他のクラウド サービスと同じ方法で Microsoft Graph にデータを提供します。</span><span class="sxs-lookup"><span data-stu-id="a310c-110">Intune provides data into Microsoft Graph in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="a310c-111"> Microsoft Graph を使用して、他のサービスからの情報と Intune を結合し、IT プロフェッショナルやエンド ユーザー向けの豊富なサービス間アプリケーションをビルドします。</span><span class="sxs-lookup"><span data-stu-id="a310c-111"> Use Microsoft Graph to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="a310c-112">以下に、アプリケーションがユーザーのデバイスにインストールされているかどうかを判断する方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="a310c-112">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="a310c-113">Azure Active Directory から、ユーザーに登録されているデバイスのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="a310c-113">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/beta/users/{user}/ownedDevices 

2. <span data-ttu-id="a310c-114">次に、テナントのアプリケーションのリストを表示します。</span><span class="sxs-lookup"><span data-stu-id="a310c-114">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps  

3. <span data-ttu-id="a310c-115">アプリケーションから ID を取得し、アプリケーション (そしてユーザー) のインストール状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="a310c-115">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{id}/deviceStatuses/


## <a name="using-microsoft-graph-permissions"></a><span data-ttu-id="a310c-116">Microsoft Graph アクセス許可の使用</span><span class="sxs-lookup"><span data-stu-id="a310c-116">Using Microsoft Graph permissions</span></span>

<span data-ttu-id="a310c-117">Microsoft Graph では、アクセス許可によってリソースへのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="a310c-117">Microsof Graph controls access to resources via permissions.</span></span> <span data-ttu-id="a310c-118">開発者は、Intune リソースにアクセスするために必要となるアクセス許可を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a310c-118">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="a310c-119">通常は Azure Active Directory ポータルでアクセス許可を指定します。</span><span class="sxs-lookup"><span data-stu-id="a310c-119">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="a310c-120">詳細については、「[Microsoft Graph のアクセス許可リファレンス](https://docs.microsoft.com/ja-JP/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a310c-120">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/ja-JP/graph/permissions-reference).</span></span>

## <a name="next-steps"></a><span data-ttu-id="a310c-121">次のステップ</span><span class="sxs-lookup"><span data-stu-id="a310c-121">Next Steps</span></span>

- <span data-ttu-id="a310c-122">Microsoft Graph の Intune API に [Azure AD を使用してアクセスする方法](https://docs.microsoft.com/ja-JP/intune/intune-graph-apis)について確認します。</span><span class="sxs-lookup"><span data-stu-id="a310c-122">Learn [how to use Azure AD](https://docs.microsoft.com/ja-JP/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="a310c-123">[PowerShell Intune サンプル](https://github.com/microsoftgraph/powershell-intune-samples)について調べます。これは、サンプルを操作しながら Intune 用 Microsoft Graph API の使用方法を示します。</span><span class="sxs-lookup"><span data-stu-id="a310c-123">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>

