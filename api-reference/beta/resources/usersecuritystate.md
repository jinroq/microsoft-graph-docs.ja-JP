---
title: userSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。"
localization_priority: Normal
ms.openlocfilehash: dd471b06f20327eb38734276ea0562ab35db6358
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810116"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="e1953-104">userSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1953-104">userSecurityState resource type</span></span>

 > <span data-ttu-id="e1953-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e1953-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e1953-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e1953-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e1953-107">ユーザー アカウントに関するステートフルな情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1953-107">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="e1953-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1953-108">Properties</span></span>

| <span data-ttu-id="e1953-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1953-109">Property</span></span>   | <span data-ttu-id="e1953-110">種類</span><span class="sxs-lookup"><span data-stu-id="e1953-110">Type</span></span> |<span data-ttu-id="e1953-111">説明</span><span class="sxs-lookup"><span data-stu-id="e1953-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e1953-112">aadUserId</span><span class="sxs-lookup"><span data-stu-id="e1953-112">aadUserId</span></span>|<span data-ttu-id="e1953-113">String</span><span class="sxs-lookup"><span data-stu-id="e1953-113">String</span></span>|<span data-ttu-id="e1953-114">AAD のユーザーは、物理/マルチ account ユーザー エンティティを表すオブジェクト識別子 (GUID) をします。</span><span class="sxs-lookup"><span data-stu-id="e1953-114">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="e1953-115">accountName</span><span class="sxs-lookup"><span data-stu-id="e1953-115">accountName</span></span>|<span data-ttu-id="e1953-116">String</span><span class="sxs-lookup"><span data-stu-id="e1953-116">String</span></span>|<span data-ttu-id="e1953-117">(せずに Active Directory ドメインまたは DNS ドメイン) のユーザー アカウントのアカウント名 (とも呼ばれる`mailNickName`)。</span><span class="sxs-lookup"><span data-stu-id="e1953-117">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="e1953-118">domainName</span><span class="sxs-lookup"><span data-stu-id="e1953-118">domainName</span></span>|<span data-ttu-id="e1953-119">String</span><span class="sxs-lookup"><span data-stu-id="e1953-119">String</span></span>|<span data-ttu-id="e1953-120">ユーザー アカウント (ドメイン \ アカウントの形式は、) の NetBIOS と Active Directory ドメイン。</span><span class="sxs-lookup"><span data-stu-id="e1953-120">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="e1953-121">emailRole</span><span class="sxs-lookup"><span data-stu-id="e1953-121">emailRole</span></span>|<span data-ttu-id="e1953-122">emailRole</span><span class="sxs-lookup"><span data-stu-id="e1953-122">emailRole</span></span>|<span data-ttu-id="e1953-123">電子メール関連のアラートをユーザー アカウントの電子メール 'ロール'。</span><span class="sxs-lookup"><span data-stu-id="e1953-123">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="e1953-124">可能な値は、`unknown`、`sender`、`recipient` です。</span><span class="sxs-lookup"><span data-stu-id="e1953-124">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="e1953-125">isVpn</span><span class="sxs-lookup"><span data-stu-id="e1953-125">isVpn</span></span>|<span data-ttu-id="e1953-126">ブール型</span><span class="sxs-lookup"><span data-stu-id="e1953-126">Boolean</span></span>|<span data-ttu-id="e1953-127">VPN 経由でユーザーをログオンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e1953-127">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="e1953-128">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="e1953-128">logonDateTime</span></span>|<span data-ttu-id="e1953-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e1953-129">DateTimeOffset</span></span>|<span data-ttu-id="e1953-130">サインインが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="e1953-130">Time at which the sign-in occurred.</span></span> <span data-ttu-id="e1953-131">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="e1953-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e1953-132">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e1953-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e1953-133">logonId</span><span class="sxs-lookup"><span data-stu-id="e1953-133">logonId</span></span>|<span data-ttu-id="e1953-134">String</span><span class="sxs-lookup"><span data-stu-id="e1953-134">String</span></span>|<span data-ttu-id="e1953-135">ユーザーのサインイン ID</span><span class="sxs-lookup"><span data-stu-id="e1953-135">User sign-in ID.</span></span>|
|<span data-ttu-id="e1953-136">logonIp</span><span class="sxs-lookup"><span data-stu-id="e1953-136">logonIp</span></span>|<span data-ttu-id="e1953-137">String</span><span class="sxs-lookup"><span data-stu-id="e1953-137">String</span></span>|<span data-ttu-id="e1953-138">IP アドレスは、サインイン要求が出されたからです。</span><span class="sxs-lookup"><span data-stu-id="e1953-138">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="e1953-139">logonLocation</span><span class="sxs-lookup"><span data-stu-id="e1953-139">logonLocation</span></span>|<span data-ttu-id="e1953-140">String</span><span class="sxs-lookup"><span data-stu-id="e1953-140">String</span></span>|<span data-ttu-id="e1953-141">(IP アドレスのマッピング) によって場所がこのユーザー、ユーザーのサインインがイベントに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="e1953-141">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="e1953-142">logonType</span><span class="sxs-lookup"><span data-stu-id="e1953-142">logonType</span></span>|<span data-ttu-id="e1953-143">logonType</span><span class="sxs-lookup"><span data-stu-id="e1953-143">logonType</span></span>|<span data-ttu-id="e1953-144">ユーザーのサインインの方法です。</span><span class="sxs-lookup"><span data-stu-id="e1953-144">Method of user sign in.</span></span> <span data-ttu-id="e1953-145">使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="e1953-145">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="e1953-146">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="e1953-146">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="e1953-147">String</span><span class="sxs-lookup"><span data-stu-id="e1953-147">String</span></span>|<span data-ttu-id="e1953-148">アクティブなディレクトリ (設置型) のセキュリティ識別子 (SID) ユーザーの。</span><span class="sxs-lookup"><span data-stu-id="e1953-148">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="e1953-149">riskScore</span><span class="sxs-lookup"><span data-stu-id="e1953-149">riskScore</span></span>|<span data-ttu-id="e1953-150">String</span><span class="sxs-lookup"><span data-stu-id="e1953-150">String</span></span>|<span data-ttu-id="e1953-151">ユーザー アカウントのプロバイダーによって生成されると計算されるリスク ・ スコアです。</span><span class="sxs-lookup"><span data-stu-id="e1953-151">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="e1953-152">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e1953-152">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="e1953-153">userAccountType</span><span class="sxs-lookup"><span data-stu-id="e1953-153">userAccountType</span></span>|<span data-ttu-id="e1953-154">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="e1953-154">userAccountSecurityType</span></span>|<span data-ttu-id="e1953-155">ユーザー アカウントの種類 (グループ) は、Windows の定義ごと。</span><span class="sxs-lookup"><span data-stu-id="e1953-155">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="e1953-156">可能な値は、`unknown`、`standard`、`power`、`administrator` です。</span><span class="sxs-lookup"><span data-stu-id="e1953-156">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="e1953-157">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e1953-157">userPrincipalName</span></span>|<span data-ttu-id="e1953-158">String</span><span class="sxs-lookup"><span data-stu-id="e1953-158">String</span></span>|<span data-ttu-id="e1953-159">ユーザー サインイン名をインターネット形式: (ユーザー アカウント名) @(ユーザー アカウントの DNS ドメイン名) です。</span><span class="sxs-lookup"><span data-stu-id="e1953-159">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e1953-160">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1953-160">JSON representation</span></span>

<span data-ttu-id="e1953-161">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e1953-161">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userSecurityState"
}-->

```json
{
  "aadUserId": "String",
  "accountName": "String",
  "domainName": "String",
  "emailRole": "@odata.type: microsoft.graph.emailRole",
  "isVpn": true,
  "logonDateTime": "String (timestamp)",
  "logonId": "String",
  "logonIp": "String",
  "logonLocation": "String",
  "logonType": "@odata.type: microsoft.graph.logonType",
  "onPremisesSecurityIdentifier": "String",
  "riskScore": "String",
  "userAccountType": "@odata.type: microsoft.graph.userAccountSecurityType",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
