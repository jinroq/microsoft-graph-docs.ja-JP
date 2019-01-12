---
title: Microsoft Intune 内の共有リソース
description: これらのエンドポイントは、Intune ワークフローの複数の Microsoft グラフ API で使用されます。  意図、目的、および特定のリソースを使用する必要なアクセス許可は、特定のワークフローと基になる呼び出しのコンテキストによって異なります。  さらに、特定のメソッド、プロパティ、およびアクションが特定のワークフローに対してのみサポートします。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: cfb3acbb3b736fcb96d22773301ca6e2e3e4403f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966777"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="8065f-105">Microsoft Intune 内の共有リソース</span><span class="sxs-lookup"><span data-stu-id="8065f-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="8065f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8065f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="8065f-107">これらのエンドポイントは、Intune ワークフローの複数の Microsoft グラフ API で使用されます。</span><span class="sxs-lookup"><span data-stu-id="8065f-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="8065f-108">意図、目的、および特定のリソースを使用する必要なアクセス許可は、特定のワークフローと基になる呼び出しのコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="8065f-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="8065f-109">さらに、特定のメソッド、プロパティ、およびアクションが特定のワークフローに対してのみサポートします。</span><span class="sxs-lookup"><span data-stu-id="8065f-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="8065f-110">Intune ワークフローとの間は、次のグラフのリソースを共有します。</span><span class="sxs-lookup"><span data-stu-id="8065f-110">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="8065f-111">すべてのデバイスの割り当て先</span><span class="sxs-lookup"><span data-stu-id="8065f-111">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="8065f-112">すべてのライセンス ユーザーの割り当て先</span><span class="sxs-lookup"><span data-stu-id="8065f-112">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="8065f-113">準拠の状態</span><span class="sxs-lookup"><span data-stu-id="8065f-113">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="8065f-114">デバイスおよびアプリ管理の割り当て先</span><span class="sxs-lookup"><span data-stu-id="8065f-114">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="8065f-115">デバイス アプリの管理</span><span class="sxs-lookup"><span data-stu-id="8065f-115">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="8065f-116">デバイス カテゴリ</span><span class="sxs-lookup"><span data-stu-id="8065f-116">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="8065f-117">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="8065f-117">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="8065f-118">除外グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="8065f-118">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="8065f-119">グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="8065f-119">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="8065f-120">目的をインストールします。</span><span class="sxs-lookup"><span data-stu-id="8065f-120">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="8065f-121">MIME コンテンツ</span><span class="sxs-lookup"><span data-stu-id="8065f-121">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="8065f-122">Report</span><span class="sxs-lookup"><span data-stu-id="8065f-122">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="8065f-123">レポートのルート</span><span class="sxs-lookup"><span data-stu-id="8065f-123">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="8065f-124">UI 状態の生成オプションを保存</span><span class="sxs-lookup"><span data-stu-id="8065f-124">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="8065f-125">URI</span><span class="sxs-lookup"><span data-stu-id="8065f-125">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="8065f-126">ユーザー</span><span class="sxs-lookup"><span data-stu-id="8065f-126">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="8065f-127">VPP トークン アカウントの種類</span><span class="sxs-lookup"><span data-stu-id="8065f-127">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
