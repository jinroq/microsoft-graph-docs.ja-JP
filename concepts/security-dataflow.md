---
title: Microsoft Graph セキュリティ API データ フロー
description: Microsoft Graph セキュリティ API は、Microsoft Graph セキュリティ エコシステムの全プロバイダーに対して要求をフェデレーションします。 これは、次の図に示すように、アプリケーションによって提供されるセキュリティ プロバイダー同意に基づいています。 同意ワークフローは、Microsoft 以外のプロバイダーにのみ適用されます。
author: preetikr
localization_priority: Priority
ms.prod: security
ms.openlocfilehash: 47731520b9ae959212750aea4f9668d58ac85a08
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32521683"
---
# <a name="microsoft-graph-security-api-data-flow"></a><span data-ttu-id="ef39c-105">Microsoft Graph セキュリティ API データ フロー</span><span class="sxs-lookup"><span data-stu-id="ef39c-105">Microsoft Graph Security API data flow</span></span>

<span data-ttu-id="ef39c-106">Microsoft Graph セキュリティ API は、Microsoft Graph セキュリティ エコシステムの全プロバイダーに対して要求をフェデレーションします。</span><span class="sxs-lookup"><span data-stu-id="ef39c-106">The Microsoft Graph Security API federates requests to all providers in the Microsoft Graph Security ecosystem.</span></span> <span data-ttu-id="ef39c-107">これは、次の図に示すように、アプリケーションによって提供されるセキュリティ プロバイダー同意に基づいています。</span><span class="sxs-lookup"><span data-stu-id="ef39c-107">This is based on the security provider consent provided by the application, as shown in the following diagram.</span></span> <span data-ttu-id="ef39c-108">同意ワークフローは、Microsoft 以外のプロバイダーにのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="ef39c-108">The consent workflow only applies to non-Microsoft providers.</span></span>

![security_dataflow_1.png](./images/security-dataflow-1.png)

<span data-ttu-id="ef39c-110">フローの説明を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ef39c-110">The following is a description of the flow:</span></span>

1. <span data-ttu-id="ef39c-111">アプリケーションのユーザーは、プロバイダーのアプリケーションにサインインして、プロバイダーからの同意書を表示します。</span><span class="sxs-lookup"><span data-stu-id="ef39c-111">The application user signs in to the provider application to view the consent form from the provider.</span></span> <span data-ttu-id="ef39c-112">この同意書機能または UI はプロバイダーが所有するものであり、Microsoft 以外のプロバイダーが、Microsoft Graph セキュリティ API へ要求を送信することへの明示的な同意を顧客から得るためにのみ、適用されます。</span><span class="sxs-lookup"><span data-stu-id="ef39c-112">This consent form experience or UI is owned by the provider and applies to non-Microsoft providers only to get explicit consent from their customers to send requests to Microsoft Graph Security API.</span></span>
2. <span data-ttu-id="ef39c-113">クライアントの同意はプロバイダー側に保存されます。</span><span class="sxs-lookup"><span data-stu-id="ef39c-113">The client consent is stored on the provider side.</span></span>
3. <span data-ttu-id="ef39c-114">プロバイダーの同意サービスが Microsoft Graph セキュリティ API を呼び出し、各顧客の同意を知らせます。</span><span class="sxs-lookup"><span data-stu-id="ef39c-114">The provider consent service calls the Microsoft Graph Security API to inform consent approval for the respective customer.</span></span>
4. <span data-ttu-id="ef39c-115">アプリケーションが、Microsoft Graph セキュリティ API に要求を送信します。</span><span class="sxs-lookup"><span data-stu-id="ef39c-115">The application sends a request to the Microsoft Graph Security API.</span></span>
5. <span data-ttu-id="ef39c-116">Microsoft Graph セキュリティ API は、さまざまなプロバイダーにマップされているこの顧客の同意情報を確認します。</span><span class="sxs-lookup"><span data-stu-id="ef39c-116">The Microsoft Graph Security API checks for the consent information for this customer mapped to various providers.</span></span>
6. <span data-ttu-id="ef39c-117">Microsoft Graph セキュリティ API は、顧客が明示的な同意をプロバイダーの同意機能により示したすべてのプロバイダーを呼び出します。</span><span class="sxs-lookup"><span data-stu-id="ef39c-117">The Microsoft Graph Security API calls all those providers the customer has given explicit consent to via the provider consent experience.</span></span>
7. <span data-ttu-id="ef39c-118">そのクライアントのすべての同意済みプロバイダーから、応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="ef39c-118">The response is returned from all the consented providers for that client.</span></span>
8. <span data-ttu-id="ef39c-119">結果セットの応答がアプリケーションに返されます。</span><span class="sxs-lookup"><span data-stu-id="ef39c-119">The result set response is returned to the application.</span></span>
9. <span data-ttu-id="ef39c-120">顧客が同意していないプロバイダーが存在する場合、そのプロバイダーからの結果は応答に含まれません。</span><span class="sxs-lookup"><span data-stu-id="ef39c-120">If the customer has not consented to any provider, no results from those providers are included in the response.</span></span>
