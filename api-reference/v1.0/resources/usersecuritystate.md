---
title: userSecurityState リソースの種類
description: ユーザー アカウントに関するステートフルな情報が含まれています。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9f451f2bc42500eee15bd59809c124a79186916f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27992057"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="2798d-103">userSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2798d-103">userSecurityState resource type</span></span>

<span data-ttu-id="2798d-104">ユーザー アカウントに関するステートフルな情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2798d-104">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="2798d-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2798d-105">Properties</span></span>

| <span data-ttu-id="2798d-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2798d-106">Property</span></span>   | <span data-ttu-id="2798d-107">型</span><span class="sxs-lookup"><span data-stu-id="2798d-107">Type</span></span> |<span data-ttu-id="2798d-108">説明</span><span class="sxs-lookup"><span data-stu-id="2798d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2798d-109">aadUserId</span><span class="sxs-lookup"><span data-stu-id="2798d-109">aadUserId</span></span>|<span data-ttu-id="2798d-110">String</span><span class="sxs-lookup"><span data-stu-id="2798d-110">String</span></span>|<span data-ttu-id="2798d-111">AAD のユーザーは、物理/マルチ account ユーザー エンティティを表すオブジェクト識別子 (GUID) をします。</span><span class="sxs-lookup"><span data-stu-id="2798d-111">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="2798d-112">accountName</span><span class="sxs-lookup"><span data-stu-id="2798d-112">accountName</span></span>|<span data-ttu-id="2798d-113">String</span><span class="sxs-lookup"><span data-stu-id="2798d-113">String</span></span>|<span data-ttu-id="2798d-114">(せずに Active Directory ドメインまたは DNS ドメイン) のユーザー アカウントのアカウント名 (とも呼ばれる`mailNickName`)。</span><span class="sxs-lookup"><span data-stu-id="2798d-114">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="2798d-115">domainName</span><span class="sxs-lookup"><span data-stu-id="2798d-115">domainName</span></span>|<span data-ttu-id="2798d-116">String</span><span class="sxs-lookup"><span data-stu-id="2798d-116">String</span></span>|<span data-ttu-id="2798d-117">ユーザー アカウント (ドメイン \ アカウントの形式は、) の NetBIOS と Active Directory ドメイン。</span><span class="sxs-lookup"><span data-stu-id="2798d-117">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="2798d-118">emailRole</span><span class="sxs-lookup"><span data-stu-id="2798d-118">emailRole</span></span>|<span data-ttu-id="2798d-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="2798d-119">emailRole</span></span>|<span data-ttu-id="2798d-120">電子メール関連のアラートをユーザー アカウントの電子メール 'ロール'。</span><span class="sxs-lookup"><span data-stu-id="2798d-120">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="2798d-121">可能な値は、`unknown`、`sender`、`recipient` です。</span><span class="sxs-lookup"><span data-stu-id="2798d-121">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="2798d-122">isVpn</span><span class="sxs-lookup"><span data-stu-id="2798d-122">isVpn</span></span>|<span data-ttu-id="2798d-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="2798d-123">Boolean</span></span>|<span data-ttu-id="2798d-124">VPN 経由でユーザーをログオンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2798d-124">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="2798d-125">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="2798d-125">logonDateTime</span></span>|<span data-ttu-id="2798d-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2798d-126">DateTimeOffset</span></span>|<span data-ttu-id="2798d-127">サインインが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="2798d-127">Time at which the sign-in occurred.</span></span> <span data-ttu-id="2798d-128">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2798d-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2798d-129">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2798d-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="2798d-130">logonId</span><span class="sxs-lookup"><span data-stu-id="2798d-130">logonId</span></span>|<span data-ttu-id="2798d-131">String</span><span class="sxs-lookup"><span data-stu-id="2798d-131">String</span></span>|<span data-ttu-id="2798d-132">ユーザーのサインイン ID</span><span class="sxs-lookup"><span data-stu-id="2798d-132">User sign-in ID.</span></span>|
|<span data-ttu-id="2798d-133">logonIp</span><span class="sxs-lookup"><span data-stu-id="2798d-133">logonIp</span></span>|<span data-ttu-id="2798d-134">String</span><span class="sxs-lookup"><span data-stu-id="2798d-134">String</span></span>|<span data-ttu-id="2798d-135">IP アドレスは、サインイン要求が出されたからです。</span><span class="sxs-lookup"><span data-stu-id="2798d-135">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="2798d-136">logonLocation</span><span class="sxs-lookup"><span data-stu-id="2798d-136">logonLocation</span></span>|<span data-ttu-id="2798d-137">String</span><span class="sxs-lookup"><span data-stu-id="2798d-137">String</span></span>|<span data-ttu-id="2798d-138">(IP アドレスのマッピング) によって場所がこのユーザー、ユーザーのサインインがイベントに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="2798d-138">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="2798d-139">logonType</span><span class="sxs-lookup"><span data-stu-id="2798d-139">logonType</span></span>|<span data-ttu-id="2798d-140">logonType</span><span class="sxs-lookup"><span data-stu-id="2798d-140">logonType</span></span>|<span data-ttu-id="2798d-141">ユーザーのサインインの方法です。</span><span class="sxs-lookup"><span data-stu-id="2798d-141">Method of user sign in.</span></span> <span data-ttu-id="2798d-142">使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="2798d-142">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="2798d-143">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="2798d-143">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="2798d-144">String</span><span class="sxs-lookup"><span data-stu-id="2798d-144">String</span></span>|<span data-ttu-id="2798d-145">アクティブなディレクトリ (設置型) のセキュリティ識別子 (SID) ユーザーの。</span><span class="sxs-lookup"><span data-stu-id="2798d-145">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="2798d-146">riskScore</span><span class="sxs-lookup"><span data-stu-id="2798d-146">riskScore</span></span>|<span data-ttu-id="2798d-147">String</span><span class="sxs-lookup"><span data-stu-id="2798d-147">String</span></span>|<span data-ttu-id="2798d-148">ユーザー アカウントのプロバイダーによって生成されると計算されるリスク ・ スコアです。</span><span class="sxs-lookup"><span data-stu-id="2798d-148">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="2798d-149">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="2798d-149">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="2798d-150">userAccountType</span><span class="sxs-lookup"><span data-stu-id="2798d-150">userAccountType</span></span>|<span data-ttu-id="2798d-151">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="2798d-151">userAccountSecurityType</span></span>|<span data-ttu-id="2798d-152">ユーザー アカウントの種類 (グループ) は、Windows の定義ごと。</span><span class="sxs-lookup"><span data-stu-id="2798d-152">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="2798d-153">可能な値は、`unknown`、`standard`、`power`、`administrator` です。</span><span class="sxs-lookup"><span data-stu-id="2798d-153">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="2798d-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2798d-154">userPrincipalName</span></span>|<span data-ttu-id="2798d-155">String</span><span class="sxs-lookup"><span data-stu-id="2798d-155">String</span></span>|<span data-ttu-id="2798d-156">ユーザー サインイン名をインターネット形式: (ユーザー アカウント名) @(ユーザー アカウントの DNS ドメイン名) です。</span><span class="sxs-lookup"><span data-stu-id="2798d-156">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2798d-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2798d-157">JSON representation</span></span>

<span data-ttu-id="2798d-158">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2798d-158">The following is a JSON representation of the resource.</span></span>

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
