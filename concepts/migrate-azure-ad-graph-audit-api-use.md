---
title: Azure AD Graph Api アプリの使用状況を調べる
description: Azure Active Directory (Azure AD) Api を監査して、アプリを Microsoft Graph API に移行する方法について説明します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 14cc61039d97fa43f64599310cf86cce6c348fb2
ms.sourcegitcommit: ca55fc5f5711966eaa41da31cd1ae99820e9e586
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/13/2019
ms.locfileid: "35645248"
---
# <a name="examine-azure-ad-graph-apis-app-usage"></a><span data-ttu-id="2425f-103">Azure AD Graph Api アプリの使用状況を調べる</span><span class="sxs-lookup"><span data-stu-id="2425f-103">Examine Azure AD Graph APIs app usage</span></span>

<span data-ttu-id="2425f-104">これは、[アプリを移行するプロセス](migrate-azure-ad-graph-planning-checklist.md)の手順2です。</span><span class="sxs-lookup"><span data-stu-id="2425f-104">This is step 2 of the [process to migrate apps](migrate-azure-ad-graph-planning-checklist.md).</span></span>

<span data-ttu-id="2425f-105">Microsoft Graph への移行を計画する際には、既存のアプリケーションを確認し、現在使用している Azure AD Graph Api をカタログ化する時間を取ります。</span><span class="sxs-lookup"><span data-stu-id="2425f-105">While planning your migration to Microsoft Graph, take time to review your existing application and to catalog the Azure AD Graph APIs you're currently using.</span></span>

<span data-ttu-id="2425f-106">リストを既知の相違点と比較します。</span><span class="sxs-lookup"><span data-stu-id="2425f-106">Compare your list to the known differences.</span></span>  <span data-ttu-id="2425f-107">これにより、アプリを移行するために必要な変更を特定することができます。</span><span class="sxs-lookup"><span data-stu-id="2425f-107">This helps identify specific changes you'll need to make to migrate your app.</span></span>  <span data-ttu-id="2425f-108">これには、エディターの検索と置換機能や、より多くの分析を必要とする複雑な更新プログラムを使用して簡単に解決できる簡単な変更が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2425f-108">These include simple changes easily resolved using an editor's search-and-replace features or more complicated updates that might require more analysis.</span></span>

<span data-ttu-id="2425f-109">Microsoft Graph では、Azure AD Graph と同じ機能と機能の多くがサポートされています。</span><span class="sxs-lookup"><span data-stu-id="2425f-109">Microsoft Graph supports many of the same features and capabilities of Azure AD graph.</span></span>  <span data-ttu-id="2425f-110">主な違いは次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2425f-110">There are a few key differences:</span></span>

- [<span data-ttu-id="2425f-111">要求の相違点</span><span class="sxs-lookup"><span data-stu-id="2425f-111">Request differences</span></span>](migrate-azure-ad-graph-request-differences.md)
- [<span data-ttu-id="2425f-112">機能の相違点</span><span class="sxs-lookup"><span data-stu-id="2425f-112">Feature differences</span></span>](migrate-azure-ad-graph-feature-differences.md)
- [<span data-ttu-id="2425f-113">リソースの種類の違い</span><span class="sxs-lookup"><span data-stu-id="2425f-113">Resource type differences</span></span>](migrate-azure-ad-graph-resource-differences.md)
- [<span data-ttu-id="2425f-114">プロパティの違い</span><span class="sxs-lookup"><span data-stu-id="2425f-114">Property differences</span></span>](migrate-azure-ad-graph-property-differences.md)
- [<span data-ttu-id="2425f-115">メソッドの違い</span><span class="sxs-lookup"><span data-stu-id="2425f-115">Method differences</span></span>](migrate-azure-ad-graph-method-differences.md)

<span data-ttu-id="2425f-116">アプリが使用している機能に必要なアクセス許可を確認することもできます。</span><span class="sxs-lookup"><span data-stu-id="2425f-116">You'll also want to verify the permissions required for the features your app is using.</span></span>  <span data-ttu-id="2425f-117">場合によっては、より詳細なアクセス許可を使用できることがあります。</span><span class="sxs-lookup"><span data-stu-id="2425f-117">In some cases, more granular permissions are available.</span></span>

<span data-ttu-id="2425f-118">詳細については、「[アクセス許可](permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2425f-118">To learn more, see [Permissions](permissions-reference.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="2425f-119">次のステップ</span><span class="sxs-lookup"><span data-stu-id="2425f-119">Next Steps</span></span>

- <span data-ttu-id="2425f-120">Azure AD Graph と Microsoft Graph の[アプリ登録、アクセス許可、および同意の違い](migrate-azure-ad-graph-app-registration.md)について説明します。</span><span class="sxs-lookup"><span data-stu-id="2425f-120">Learn about [app registration, permissions and consent differences](migrate-azure-ad-graph-app-registration.md) between Azure AD Graph and Microsoft Graph.</span></span>
- <span data-ttu-id="2425f-121">[Microsoft Graph](/graph/overview)の概念とプラクティスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2425f-121">Explore [Microsoft Graph](/graph/overview) concepts and practices.</span></span>
- <span data-ttu-id="2425f-122">[Graph エクスプローラー](https://aka.ms/ge)を使用して、Microsoft graph を試してみてください。</span><span class="sxs-lookup"><span data-stu-id="2425f-122">Use [Graph Explorer](https://aka.ms/ge) to experiment with Microsoft Graph.</span></span>
