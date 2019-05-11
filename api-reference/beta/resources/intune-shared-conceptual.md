---
title: Microsoft Intune での共有リソース-Microsoft Graph API
description: テナント組織の複数のワークフローをサポートする Intune エンドポイント (REST) の Microsoft Graph API の一覧を示します。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: d627ebb67876c89136ba6e4e63e9879e3a0ed8d2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939904"
---
# <a name="shared-resources-in-microsoft-intune"></a><span data-ttu-id="d1c92-103">Microsoft Intune での共有リソース</span><span class="sxs-lookup"><span data-stu-id="d1c92-103">Shared resources in Microsoft Intune</span></span>

> <span data-ttu-id="d1c92-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d1c92-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1c92-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1c92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1c92-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d1c92-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://www.microsoft.com/en-us/cloud-platform/microsoft-intune-pricing) by the customer.</span></span>

<span data-ttu-id="d1c92-107">これらのエンドポイントは、Intune ワークフロー用の複数の Microsoft Graph API で使用されます。</span><span class="sxs-lookup"><span data-stu-id="d1c92-107">These endpoints are used in multiple Microsoft Graph API for Intune workflows.</span></span>  <span data-ttu-id="d1c92-108">特定のリソースを使用するために必要な目的、およびアクセス許可は、基になる呼び出しの特定のワークフローおよびコンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="d1c92-108">The intent, purpose, and permissions required to use a given resource varies according to the specific workflow and context of the underlying call.</span></span>  <span data-ttu-id="d1c92-109">さらに、特定のワークフローに対してのみ、特定のメソッド、プロパティ、およびアクションがサポートされます。</span><span class="sxs-lookup"><span data-stu-id="d1c92-109">In addition, certain methods, properties, and actions are supported only for specific workflows.</span></span>

<span data-ttu-id="d1c92-110">次の Graph リソースは、Intune ワークフロー間で共有されます。</span><span class="sxs-lookup"><span data-stu-id="d1c92-110">The following Graph resources are shared between Intune workflows:</span></span>

- [<span data-ttu-id="d1c92-111">アクションの状態</span><span class="sxs-lookup"><span data-stu-id="d1c92-111">Action state</span></span>](intune-shared-actionstate.md)
- [<span data-ttu-id="d1c92-112">すべてのデバイスの割り当て先</span><span class="sxs-lookup"><span data-stu-id="d1c92-112">All devices assignment target</span></span>](intune-shared-alldevicesassignmenttarget.md)
- [<span data-ttu-id="d1c92-113">すべてのライセンス ユーザーの割り当て先</span><span class="sxs-lookup"><span data-stu-id="d1c92-113">All licensed users assignment target</span></span>](intune-shared-alllicensedusersassignmenttarget.md)
- [<span data-ttu-id="d1c92-114">コンプライアンスのステータス</span><span class="sxs-lookup"><span data-stu-id="d1c92-114">Compliance status</span></span>](intune-shared-compliancestatus.md)
- [<span data-ttu-id="d1c92-115">デバイスおよびアプリ管理の割り当て先</span><span class="sxs-lookup"><span data-stu-id="d1c92-115">Device and app management assignment target</span></span>](intune-shared-deviceandappmanagementassignmenttarget.md)
- [<span data-ttu-id="d1c92-116">デバイス アプリの管理</span><span class="sxs-lookup"><span data-stu-id="d1c92-116">Device app management</span></span>](intune-shared-deviceappmanagement.md)
- [<span data-ttu-id="d1c92-117">デバイス カテゴリ</span><span class="sxs-lookup"><span data-stu-id="d1c92-117">Device category</span></span>](intune-shared-devicecategory.md)
- [<span data-ttu-id="d1c92-118">デバイスの登録のタイプ</span><span class="sxs-lookup"><span data-stu-id="d1c92-118">Device enrollment type</span></span>](intune-shared-deviceenrollmenttype.md)
- [<span data-ttu-id="d1c92-119">デバイスの管理</span><span class="sxs-lookup"><span data-stu-id="d1c92-119">Device management</span></span>](intune-shared-devicemanagement.md)
- [<span data-ttu-id="d1c92-120">デバイスのプラットフォームの種類</span><span class="sxs-lookup"><span data-stu-id="d1c92-120">Device platform type</span></span>](intune-shared-deviceplatformtype.md)
- [<span data-ttu-id="d1c92-121">デバイスのタイプ</span><span class="sxs-lookup"><span data-stu-id="d1c92-121">Device type</span></span>](intune-shared-devicetype.md)
- [<span data-ttu-id="d1c92-122">有効化</span><span class="sxs-lookup"><span data-stu-id="d1c92-122">Enablement</span></span>](intune-shared-enablement.md)
- [<span data-ttu-id="d1c92-123">除外グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="d1c92-123">Exclusion group assignment target</span></span>](intune-shared-exclusiongroupassignmenttarget.md)
- [<span data-ttu-id="d1c92-124">グループの割り当て先</span><span class="sxs-lookup"><span data-stu-id="d1c92-124">Group assignment target</span></span>](intune-shared-groupassignmenttarget.md)
- [<span data-ttu-id="d1c92-125">インストール目的</span><span class="sxs-lookup"><span data-stu-id="d1c92-125">Install intent</span></span>](intune-shared-installintent.md)
- [<span data-ttu-id="d1c92-126">IP 範囲</span><span class="sxs-lookup"><span data-stu-id="d1c92-126">IP range</span></span>](intune-shared-iprange.md)
- [<span data-ttu-id="d1c92-127">IPv4 の範囲</span><span class="sxs-lookup"><span data-stu-id="d1c92-127">IPv4 range</span></span>](intune-shared-ipv4range.md)
- [<span data-ttu-id="d1c92-128">IPv6 の範囲</span><span class="sxs-lookup"><span data-stu-id="d1c92-128">IPv6 range</span></span>](intune-shared-ipv6range.md)
- [<span data-ttu-id="d1c92-129">キー/値のペア</span><span class="sxs-lookup"><span data-stu-id="d1c92-129">Key/value pair</span></span>](intune-shared-keyvaluepair.md)
- [<span data-ttu-id="d1c92-130">MIME コンテンツ</span><span class="sxs-lookup"><span data-stu-id="d1c92-130">MIME content</span></span>](intune-shared-mimecontent.md)
- [<span data-ttu-id="d1c92-131">モバイル アプリのトラブルシューティング イベント</span><span class="sxs-lookup"><span data-stu-id="d1c92-131">Mobile app troubleshooting event</span></span>](intune-shared-mobileapptroubleshootingevent.md)
- [<span data-ttu-id="d1c92-132">プロキシ化されたドメイン</span><span class="sxs-lookup"><span data-stu-id="d1c92-132">Proxied domain</span></span>](intune-shared-proxieddomain.md)
- [<span data-ttu-id="d1c92-133">Report</span><span class="sxs-lookup"><span data-stu-id="d1c92-133">Report</span></span>](intune-shared-report.md)
- [<span data-ttu-id="d1c92-134">レポートのルート</span><span class="sxs-lookup"><span data-stu-id="d1c92-134">Report root</span></span>](intune-shared-reportroot.md)
- [<span data-ttu-id="d1c92-135">アプリの状態の結果</span><span class="sxs-lookup"><span data-stu-id="d1c92-135">Resultant app state</span></span>](intune-shared-resultantappstate.md)
- [<span data-ttu-id="d1c92-136">RGB カラー</span><span class="sxs-lookup"><span data-stu-id="d1c92-136">RGB color</span></span>](intune-shared-rgbcolor.md)
- [<span data-ttu-id="d1c92-137">アカウントの種類として実行</span><span class="sxs-lookup"><span data-stu-id="d1c92-137">Run as account type</span></span>](intune-shared-runasaccounttype.md)
- [<span data-ttu-id="d1c92-138">実行状態</span><span class="sxs-lookup"><span data-stu-id="d1c92-138">Run state</span></span>](intune-shared-runstate.md)
- [<span data-ttu-id="d1c92-139">保存 UI 状態生成オプション</span><span class="sxs-lookup"><span data-stu-id="d1c92-139">Saved UI state generation options</span></span>](intune-shared-saveduistategenerationoptions.md)
- [<span data-ttu-id="d1c92-140">URI</span><span class="sxs-lookup"><span data-stu-id="d1c92-140">URI</span></span>](intune-shared-uri.md)
- [<span data-ttu-id="d1c92-141">ユーザー</span><span class="sxs-lookup"><span data-stu-id="d1c92-141">User</span></span>](intune-shared-user.md)
- [<span data-ttu-id="d1c92-142">VPP トークン アカウントのタイプ</span><span class="sxs-lookup"><span data-stu-id="d1c92-142">VPP token account type</span></span>](intune-shared-vpptokenaccounttype.md)
- [<span data-ttu-id="d1c92-143">VPP トークンのアクションのエラーの理由</span><span class="sxs-lookup"><span data-stu-id="d1c92-143">VPP token action failure reason</span></span>](intune-shared-vpptokenactionfailurereason.md)
- [<span data-ttu-id="d1c92-144">Windows ドメイン参加の構成</span><span class="sxs-lookup"><span data-stu-id="d1c92-144">Windows domain join configuration</span></span>](intune-shared-windowsdomainjoinconfiguration.md)
