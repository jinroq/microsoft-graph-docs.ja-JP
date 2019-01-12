---
title: Microsoft Graph での Office 365 使用状況レポートの使用
description: Microsoft Graph によって、Office 365 使用状況レポートのリソースにアクセスし、社内で Office 365 サービスがどのように使用されているかについての情報を取得できます。 たとえば、サービスをよく利用してクォータに到達しそうなユーザーや、Office 365 ライセンスを必要としない可能性があるユーザーなどを識別できます。
localization_priority: Priority
ms.prod: reports
ms.openlocfilehash: 4e1a139b000eb1d4f1175ddc05f818aaa0072b01
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987133"
---
# <a name="working-with-office-365-usage-reports-in-microsoft-graph"></a><span data-ttu-id="fc7f7-104">Microsoft Graph での Office 365 使用状況レポートの使用</span><span class="sxs-lookup"><span data-stu-id="fc7f7-104">Working with Office 365 usage reports in Microsoft Graph</span></span>

<span data-ttu-id="fc7f7-105">Microsoft Graph によって、Office 365 使用状況レポートのリソースにアクセスし、社内で Office 365 サービスがどのように使用されているかについての情報を取得できます。</span><span class="sxs-lookup"><span data-stu-id="fc7f7-105">With Microsoft Graph, you can access Office 365 usage reports resources to get the information about how people in your business are using Office 365 services.</span></span> <span data-ttu-id="fc7f7-106">たとえば、サービスをよく利用してクォータに到達しそうなユーザーや、Office 365 ライセンスを必要としない可能性があるユーザーなどを識別できます。</span><span class="sxs-lookup"><span data-stu-id="fc7f7-106">For example, you can identify who is using a service a lot and reaching quotas, or who may not need an Office 365 license at all.</span></span>

## <a name="authorization"></a><span data-ttu-id="fc7f7-107">認証</span><span class="sxs-lookup"><span data-stu-id="fc7f7-107">Authorization</span></span>

<span data-ttu-id="fc7f7-108">Microsoft Graph では、アクセス許可によってリソースへのアクセスを制御します。</span><span class="sxs-lookup"><span data-stu-id="fc7f7-108">Microsoft Graph controls access to resources via permissions.</span></span> <span data-ttu-id="fc7f7-109">Reports リソースにアクセスするには、アクセス許可を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc7f7-109">You must specify the permissions you need in order to access Reports resources.</span></span> <span data-ttu-id="fc7f7-110">通常は Azure Active Directory (Azure AD) ポータルでアクセス許可を指定します。</span><span class="sxs-lookup"><span data-stu-id="fc7f7-110">Typically, you specify permissions in the Azure Active Directory (Azure AD) portal.</span></span> <span data-ttu-id="fc7f7-111">詳細については、「[Microsoft Graph のアクセス許可のリファレンス](/graph/permissions-reference)」および「[Reports のアクセス許可](/graph/permissions-reference#reports-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc7f7-111">For more information, see [Microsoft Graph permissions reference](/graph/permissions-reference) and [Reports permissions](/graph/permissions-reference#reports-permissions).</span></span>

## <a name="next-steps"></a><span data-ttu-id="fc7f7-112">次の手順</span><span class="sxs-lookup"><span data-stu-id="fc7f7-112">Next steps</span></span>

<span data-ttu-id="fc7f7-113">Reports リソースと API によって、ユーザーとの連携や、ユーザーの Microsoft Graph のエクスペリエンスを管理する新しい方法が見つかります。</span><span class="sxs-lookup"><span data-stu-id="fc7f7-113">Reports resources and APIs can open up new ways for you to engage with users and manage their experiences with Microsoft Graph.</span></span> <span data-ttu-id="fc7f7-114">詳細情報</span><span class="sxs-lookup"><span data-stu-id="fc7f7-114">To learn more:</span></span>

- <span data-ttu-id="fc7f7-115">特定のシナリオに役立つ、メソッドとリソースのプロパティを詳しく調べます。</span><span class="sxs-lookup"><span data-stu-id="fc7f7-115">Drill down on the methods and properties of the resources most helpful to your scenario.</span></span>
- <span data-ttu-id="fc7f7-116">[Graph エクスプローラー](https://developer.microsoft.com/graph/graph-explorer)で API をお試しください。</span><span class="sxs-lookup"><span data-stu-id="fc7f7-116">Try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<span data-ttu-id="fc7f7-p105">さらに情報が必要な場合「[パートナーによる Microsoft Graph の活用方法](https://developer.microsoft.com/graph/graph/examples#partners)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc7f7-p105">Need more ideas? See [how some of our partners are using Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners).</span></span>
