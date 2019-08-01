---
title: Intune Graph API の使用
description: " Intune ハイブリッド展開はサポートされていません。 "
author: tfitzmac
localization_priority: Priority
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: a5007c629fd48165ceedd6a829ce8c21fc5e9c10
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027343"
---
# <a name="working-with-intune-in-microsoft-graph"></a><span data-ttu-id="47111-103">Microsoft Graph での Intune の操作</span><span class="sxs-lookup"><span data-stu-id="47111-103">Working with Intune in Microsoft Graph</span></span>  

> <span data-ttu-id="47111-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="47111-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="47111-105">Intune 用 Microsoft Graph API を使用すると、テナントの Intune の情報へのプログラムによるアクセスが可能となります。API は **Azure Portal** で使用できるものと同じ Intune 操作を実行します。</span><span class="sxs-lookup"><span data-stu-id="47111-105">The Microsoft Graph API for Intune enables programmatic access to Intune information for your tenant; the API performs the same Intune operations as those available through the **Azure Portal**.</span></span>  

<span data-ttu-id="47111-106">モバイル デバイス管理 (MDM) のシナリオの場合、Intune 用 Microsoft Graph API はスタンドアロンの展開をサポートします。Intune の[ハイブリッド展開](https://docs.microsoft.com/ja-JP/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management)はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="47111-106">For mobile device management (MDM) scenarios, the Microsoft Graph API for Intune supports standalone deployments; Intune [hybrid deployments](https://docs.microsoft.com/en-us/sccm/mdm/understand/choose-between-standalone-intune-and-hybrid-mobile-device-management) are not supported.</span></span> 

## <a name="using-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="47111-107">Intune 用 Microsoft Graph API の使用</span><span class="sxs-lookup"><span data-stu-id="47111-107">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="47111-108">Intune は、豊富なエンティティ情報とリレーションシップのナビゲーションを使用して、他のクラウド サービスと同じ方法で Microsoft Graph API にデータを提供します。</span><span class="sxs-lookup"><span data-stu-id="47111-108">Intune provides data into the Microsoft Graph API in the same way as other cloud services do, with rich entity information and relationship navigation.</span></span><span data-ttu-id="47111-109"> Microsoft Graph API を使用して、他のサービスからの情報と Intune を結合し、IT プロフェッショナルやエンド ユーザー向けの豊富なサービス間アプリケーションをビルドします。</span><span class="sxs-lookup"><span data-stu-id="47111-109"> Use the Microsoft Graph API to combine information from other services and Intune to build rich cross-service applications for IT professionals or end users.</span></span>     

<span data-ttu-id="47111-110">以下に、アプリケーションがユーザーのデバイスにインストールされているかどうかを判断する方法の例を示します。</span><span class="sxs-lookup"><span data-stu-id="47111-110">The following example shows how you can determine whether an application is installed on a user's device:</span></span> 

1. <span data-ttu-id="47111-111">Azure Active Directory から、ユーザーに登録されているデバイスのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="47111-111">Get from Azure Active Directory a list of devices registered to a user:</span></span> 

    https://graph.microsoft.com/users/{user}/ownedDevices 

2. <span data-ttu-id="47111-112">次に、テナントのアプリケーションのリストを表示します。</span><span class="sxs-lookup"><span data-stu-id="47111-112">Then view the list of applications for your tenant:</span></span> 

    https://graph.microsoft.com/deviceAppManagement/mobileApps  

3. <span data-ttu-id="47111-113">アプリケーションから ID を取得し、アプリケーション (そしてユーザー) のインストール状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="47111-113">Take the ID from the application and determine the installation state for the application (and therefore user):</span></span>

    https://graph.microsoft.com/deviceAppManagement/mobileApps/{id}/deviceStatuses/

## <a name="accessing-the-microsoft-graph-api-for-intune"></a><span data-ttu-id="47111-114">Intune 用 Microsoft Graph API へのアクセス</span><span class="sxs-lookup"><span data-stu-id="47111-114">Using the Microsoft Graph API for Intune</span></span>

<span data-ttu-id="47111-115">Intune は、[委任されたアクセス許可](https://docs.microsoft.com/graph/auth-v2-user)と[アプリケーションのアクセス許可](https://docs.microsoft.com/graph/auth-v2-service)の両方をサポートします。</span><span class="sxs-lookup"><span data-stu-id="47111-115">Intune supports both [delegated permissions](https://docs.microsoft.com/graph/auth-v2-user) and [application permissions](https://docs.microsoft.com/graph/auth-v2-service).</span></span> <span data-ttu-id="47111-116">委任されたアクセス許可は、読み取り操作と書き込み操作の両方でサポートされています。</span><span class="sxs-lookup"><span data-stu-id="47111-116">Delegated permissions are supported for both read and write operations.</span></span> <span data-ttu-id="47111-117">アプリケーションのアクセス許可は、現在、読み取り操作でのみサポートされています。</span><span class="sxs-lookup"><span data-stu-id="47111-117">Application permissions are currently supported for read operations only.</span></span> <span data-ttu-id="47111-118">委任されたアクセス許可およびアプリケーションのアクセス許可は、シングル テナント アプリケーションおよびマルチテナント アプリケーションの両方をサポートします。</span><span class="sxs-lookup"><span data-stu-id="47111-118">Delegated and application permissions support both single tenant applications, as well as multi-tenant applications.</span></span> <span data-ttu-id="47111-119">Microsoft Graph で使用できるアクセス許可の詳細については、「[Microsoft Graph のアクセス許可のリファレンス](https://docs.microsoft.com/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47111-119">For more information about the permissions available through Microsoft Graph, see [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference).</span></span>

## <a name="using-permissions"></a><span data-ttu-id="47111-120">アクセス許可の使用</span><span class="sxs-lookup"><span data-stu-id="47111-120">Using permissions</span></span>

<span data-ttu-id="47111-121">Microsoft Graph API は、アクセス許可によってリソースへのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="47111-121">The Microsoft Graph API controls access to resources via permissions.</span></span> <span data-ttu-id="47111-122">開発者は、Intune リソースにアクセスするために必要となるアクセス許可を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="47111-122">As a developer, you must specify the permissions you need to access Intune resources.</span></span> <span data-ttu-id="47111-123">通常は Azure Active Directory ポータルでアクセス許可を指定します。</span><span class="sxs-lookup"><span data-stu-id="47111-123">Typically, you specify the permissions in the Azure Active Directory portal.</span></span> <span data-ttu-id="47111-124">詳細については、「[Microsoft Graph のアクセス許可リファレンス](https://docs.microsoft.com/ja-JP/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47111-124">For more information, see [Microsoft Graph permissions reference](https://docs.microsoft.com/en-us/graph/permissions-reference).</span></span>

## <a name="next-steps"></a><span data-ttu-id="47111-125">次のステップ</span><span class="sxs-lookup"><span data-stu-id="47111-125">Next Steps</span></span>

- <span data-ttu-id="47111-126">Microsoft Graph の Intune API に [Azure AD を使用してアクセスする方法](https://docs.microsoft.com/ja-JP/intune/intune-graph-apis)について確認します。</span><span class="sxs-lookup"><span data-stu-id="47111-126">Learn [how to use Azure AD](https://docs.microsoft.com/en-us/intune/intune-graph-apis) to access the Microsoft Graph API for Intune.</span></span>  
- <span data-ttu-id="47111-127">[PowerShell Intune サンプル](https://github.com/microsoftgraph/powershell-intune-samples)について調べます。これは、サンプルを操作しながら Intune 用 Microsoft Graph API の使用方法を示します。</span><span class="sxs-lookup"><span data-stu-id="47111-127">Explore the [PowerShell Intune samples](https://github.com/microsoftgraph/powershell-intune-samples), which show how to use the Microsoft Graph API for Intune in context of working examples.</span></span>
