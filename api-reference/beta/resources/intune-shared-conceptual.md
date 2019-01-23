---
title: Microsoft Intune 内の共有リソース
description: これらのエンドポイントは、Intune ワークフローの複数の Microsoft グラフ API で使用されます。  意図、目的、および特定のリソースを使用する必要なアクセス許可は、特定のワークフローと基になる呼び出しのコンテキストによって異なります。  さらに、特定のメソッド、プロパティ、およびアクションが特定のワークフローに対してのみサポートします。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: 11ee529edd3d74b5d6fb0c2d9d4e63bada0b0b22
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415433"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="191bc-105">Microsoft Intune 内の共有リソース</span><span class="sxs-lookup"><span data-stu-id="191bc-105">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="191bc-106">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="191bc-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="191bc-107">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="191bc-107">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="191bc-108">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="191bc-108">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="191bc-109">これらのエンドポイントは、Intune ワークフローの複数の Microsoft グラフ API で使用されます。</span><span class="sxs-lookup"><span data-stu-id="191bc-109">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="191bc-110">意図、目的、および特定のリソースを使用する必要なアクセス許可は、特定のワークフローと基になる呼び出しのコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="191bc-110">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="191bc-111">さらに、特定のメソッド、プロパティ、およびアクションが特定のワークフローに対してのみサポートします。</span><span class="sxs-lookup"><span data-stu-id="191bc-111">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="191bc-112">Intune ワークフローとの間は、次のグラフのリソースを共有します。</span><span class="sxs-lookup"><span data-stu-id="191bc-112">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="191bc-113">動作状態</span><span class="sxs-lookup"><span data-stu-id="191bc-113">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="191bc-114">すべてのデバイスの割り当て先</span><span class="sxs-lookup"><span data-stu-id="191bc-114">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="191bc-115">すべてのライセンス ユーザーの割り当て先</span><span class="sxs-lookup"><span data-stu-id="191bc-115">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="191bc-116">準拠の状態</span><span class="sxs-lookup"><span data-stu-id="191bc-116">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="191bc-117">デバイスおよびアプリ管理の割り当て先</span><span class="sxs-lookup"><span data-stu-id="191bc-117">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="191bc-118">デバイス アプリの管理</span><span class="sxs-lookup"><span data-stu-id="191bc-118">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="191bc-119">デバイス カテゴリ</span><span class="sxs-lookup"><span data-stu-id="191bc-119">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="191bc-120">デバイス登録の種類</span><span class="sxs-lookup"><span data-stu-id="191bc-120">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="191bc-121">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="191bc-121">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="191bc-122">デバイス プラットフォームの種類</span><span class="sxs-lookup"><span data-stu-id="191bc-122">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="191bc-123">デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="191bc-123">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="191bc-124">有効化</span><span class="sxs-lookup"><span data-stu-id="191bc-124">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="191bc-125">除外グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="191bc-125">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="191bc-126">グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="191bc-126">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="191bc-127">目的をインストールします。</span><span class="sxs-lookup"><span data-stu-id="191bc-127">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="191bc-128">IP 範囲</span><span class="sxs-lookup"><span data-stu-id="191bc-128">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="191bc-129">IPv4 の範囲</span><span class="sxs-lookup"><span data-stu-id="191bc-129">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="191bc-130">IPv6 の範囲</span><span class="sxs-lookup"><span data-stu-id="191bc-130">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="191bc-131">キー/値のペア</span><span class="sxs-lookup"><span data-stu-id="191bc-131">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="191bc-132">MIME コンテンツ</span><span class="sxs-lookup"><span data-stu-id="191bc-132">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="191bc-133">モバイル アプリケーションのトラブルシューティング イベント</span><span class="sxs-lookup"><span data-stu-id="191bc-133">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="191bc-134">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="191bc-134">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="191bc-135">Report</span><span class="sxs-lookup"><span data-stu-id="191bc-135">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="191bc-136">レポートのルート</span><span class="sxs-lookup"><span data-stu-id="191bc-136">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="191bc-137">結果のアプリケーションの状態</span><span class="sxs-lookup"><span data-stu-id="191bc-137">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="191bc-138">RGB カラー</span><span class="sxs-lookup"><span data-stu-id="191bc-138">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="191bc-139">実行アカウントの種類として</span><span class="sxs-lookup"><span data-stu-id="191bc-139">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="191bc-140">状態を実行します。</span><span class="sxs-lookup"><span data-stu-id="191bc-140">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="191bc-141">UI 状態の生成オプションを保存</span><span class="sxs-lookup"><span data-stu-id="191bc-141">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="191bc-142">URI</span><span class="sxs-lookup"><span data-stu-id="191bc-142">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="191bc-143">ユーザー</span><span class="sxs-lookup"><span data-stu-id="191bc-143">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="191bc-144">VPP トークン アカウントの種類</span><span class="sxs-lookup"><span data-stu-id="191bc-144">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="191bc-145">VPP トークンの操作の失敗の理由</span><span class="sxs-lookup"><span data-stu-id="191bc-145">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="191bc-146">Windows ドメインの結合の構成</span><span class="sxs-lookup"><span data-stu-id="191bc-146">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
