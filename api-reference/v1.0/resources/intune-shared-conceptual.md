---
title: Microsoft Intune での共有リソース
description: これらのエンドポイントは、Intune ワークフロー用の複数の Microsoft Graph API で使用されます。  特定のリソースを使用するために必要な目的、およびアクセス許可は、基になる呼び出しの特定のワークフローおよびコンテキストによって異なります。  さらに、特定のワークフローに対してのみ、特定のメソッド、プロパティ、およびアクションがサポートされます。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
doc_type: conceptualPageType
ms.openlocfilehash: 7f04077278a3765a27abd30f02bcc2361c7cd08e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037017"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="c4ef6-105">Microsoft Intune での共有リソース</span><span class="sxs-lookup"><span data-stu-id="c4ef6-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="c4ef6-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c4ef6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="c4ef6-107">これらのエンドポイントは、Intune ワークフロー用の複数の Microsoft Graph API で使用されます。</span><span class="sxs-lookup"><span data-stu-id="c4ef6-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="c4ef6-108">特定のリソースを使用するために必要な目的、およびアクセス許可は、基になる呼び出しの特定のワークフローおよびコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="c4ef6-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="c4ef6-109">さらに、特定のワークフローに対してのみ、特定のメソッド、プロパティ、およびアクションがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="c4ef6-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="c4ef6-110">次の Graph リソースは、Intune ワークフロー間で共有されます。</span><span class="sxs-lookup"><span data-stu-id="c4ef6-110">The following Graph resources are shared between Intune workflows:</span></span>  

- [<span data-ttu-id="c4ef6-111">すべてのデバイスの割り当て先</span><span class="sxs-lookup"><span data-stu-id="c4ef6-111">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="c4ef6-112">すべてのライセンス ユーザーの割り当て先</span><span class="sxs-lookup"><span data-stu-id="c4ef6-112">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="c4ef6-113">コンプライアンスのステータス</span><span class="sxs-lookup"><span data-stu-id="c4ef6-113">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="c4ef6-114">デバイスおよびアプリ管理の割り当て先</span><span class="sxs-lookup"><span data-stu-id="c4ef6-114">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="c4ef6-115">デバイス アプリの管理</span><span class="sxs-lookup"><span data-stu-id="c4ef6-115">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="c4ef6-116">デバイス カテゴリ</span><span class="sxs-lookup"><span data-stu-id="c4ef6-116">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="c4ef6-117">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="c4ef6-117">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="c4ef6-118">除外グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="c4ef6-118">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="c4ef6-119">グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="c4ef6-119">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="c4ef6-120">インストール目的</span><span class="sxs-lookup"><span data-stu-id="c4ef6-120">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="c4ef6-121">MIME コンテンツ</span><span class="sxs-lookup"><span data-stu-id="c4ef6-121">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="c4ef6-122">Report</span><span class="sxs-lookup"><span data-stu-id="c4ef6-122">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="c4ef6-123">レポートのルート</span><span class="sxs-lookup"><span data-stu-id="c4ef6-123">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="c4ef6-124">保存 UI 状態生成オプション</span><span class="sxs-lookup"><span data-stu-id="c4ef6-124">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="c4ef6-125">URI</span><span class="sxs-lookup"><span data-stu-id="c4ef6-125">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="c4ef6-126">ユーザー</span><span class="sxs-lookup"><span data-stu-id="c4ef6-126">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="c4ef6-127">VPP トークン アカウントのタイプ</span><span class="sxs-lookup"><span data-stu-id="c4ef6-127">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
