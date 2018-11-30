---
title: Microsoft Intune 内の共有リソース
description: これらのエンドポイントは、Intune ワークフローの複数の Microsoft グラフ API で使用されます。  意図、目的、および特定のリソースを使用する必要なアクセス許可は、特定のワークフローと基になる呼び出しのコンテキストによって異なります。  さらに、特定のメソッド、プロパティ、およびアクションが特定のワークフローに対してのみサポートします。
ms.openlocfilehash: a0e896b2aed219679ec45804dc94b22b7cb9d727
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073899"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="54aa0-105">Microsoft Intune 内の共有リソース</span><span class="sxs-lookup"><span data-stu-id="54aa0-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="54aa0-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="54aa0-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54aa0-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54aa0-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54aa0-108">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="54aa0-108">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="54aa0-109">これらのエンドポイントは、Intune ワークフローの複数の Microsoft グラフ API で使用されます。</span><span class="sxs-lookup"><span data-stu-id="54aa0-109">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="54aa0-110">意図、目的、および特定のリソースを使用する必要なアクセス許可は、特定のワークフローと基になる呼び出しのコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="54aa0-110">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="54aa0-111">さらに、特定のメソッド、プロパティ、およびアクションが特定のワークフローに対してのみサポートします。</span><span class="sxs-lookup"><span data-stu-id="54aa0-111">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="54aa0-112">Intune ワークフローとの間は、次のグラフのリソースを共有します。</span><span class="sxs-lookup"><span data-stu-id="54aa0-112">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="54aa0-113">動作状態</span><span class="sxs-lookup"><span data-stu-id="54aa0-113">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="54aa0-114">すべてのデバイスの割り当て先</span><span class="sxs-lookup"><span data-stu-id="54aa0-114">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="54aa0-115">すべてのライセンス ユーザーの割り当て先</span><span class="sxs-lookup"><span data-stu-id="54aa0-115">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="54aa0-116">準拠の状態</span><span class="sxs-lookup"><span data-stu-id="54aa0-116">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="54aa0-117">デバイスおよびアプリ管理の割り当て先</span><span class="sxs-lookup"><span data-stu-id="54aa0-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="54aa0-118">デバイス アプリの管理</span><span class="sxs-lookup"><span data-stu-id="54aa0-118">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="54aa0-119">デバイス カテゴリ</span><span class="sxs-lookup"><span data-stu-id="54aa0-119">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="54aa0-120">デバイス登録の種類</span><span class="sxs-lookup"><span data-stu-id="54aa0-120">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="54aa0-121">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="54aa0-121">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="54aa0-122">デバイス プラットフォームの種類</span><span class="sxs-lookup"><span data-stu-id="54aa0-122">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="54aa0-123">デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="54aa0-123">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="54aa0-124">有効化</span><span class="sxs-lookup"><span data-stu-id="54aa0-124">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="54aa0-125">除外グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="54aa0-125">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="54aa0-126">グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="54aa0-126">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="54aa0-127">目的をインストールします。</span><span class="sxs-lookup"><span data-stu-id="54aa0-127">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="54aa0-128">IP 範囲</span><span class="sxs-lookup"><span data-stu-id="54aa0-128">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="54aa0-129">IPv4 の範囲</span><span class="sxs-lookup"><span data-stu-id="54aa0-129">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="54aa0-130">IPv6 の範囲</span><span class="sxs-lookup"><span data-stu-id="54aa0-130">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="54aa0-131">キー/値のペア</span><span class="sxs-lookup"><span data-stu-id="54aa0-131">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="54aa0-132">MIME コンテンツ</span><span class="sxs-lookup"><span data-stu-id="54aa0-132">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="54aa0-133">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="54aa0-133">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="54aa0-134">Report</span><span class="sxs-lookup"><span data-stu-id="54aa0-134">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="54aa0-135">レポートのルート</span><span class="sxs-lookup"><span data-stu-id="54aa0-135">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="54aa0-136">結果のアプリケーションの状態</span><span class="sxs-lookup"><span data-stu-id="54aa0-136">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="54aa0-137">RGB カラー</span><span class="sxs-lookup"><span data-stu-id="54aa0-137">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="54aa0-138">実行アカウントの種類として</span><span class="sxs-lookup"><span data-stu-id="54aa0-138">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="54aa0-139">状態を実行します。</span><span class="sxs-lookup"><span data-stu-id="54aa0-139">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="54aa0-140">UI 状態の生成オプションを保存</span><span class="sxs-lookup"><span data-stu-id="54aa0-140">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="54aa0-141">URI</span><span class="sxs-lookup"><span data-stu-id="54aa0-141">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="54aa0-142">User</span><span class="sxs-lookup"><span data-stu-id="54aa0-142">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="54aa0-143">VPP トークン アカウントの種類</span><span class="sxs-lookup"><span data-stu-id="54aa0-143">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="54aa0-144">VPP トークンの操作の失敗の理由</span><span class="sxs-lookup"><span data-stu-id="54aa0-144">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="54aa0-145">Windows ドメインの結合の構成</span><span class="sxs-lookup"><span data-stu-id="54aa0-145">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
