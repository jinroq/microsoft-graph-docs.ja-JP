---
title: userSecurityState リソースの種類
description: ユーザー アカウントに関するステートフルな情報が含まれています。
ms.openlocfilehash: dbb4b6600cc11a75c84f2f0b233535d012309f88
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022738"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="e9780-103">userSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e9780-103">userSecurityState resource type</span></span>

<span data-ttu-id="e9780-104">ユーザー アカウントに関するステートフルな情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e9780-104">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="e9780-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9780-105">Properties</span></span>

| <span data-ttu-id="e9780-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9780-106">Property</span></span>   | <span data-ttu-id="e9780-107">型</span><span class="sxs-lookup"><span data-stu-id="e9780-107">Type</span></span> |<span data-ttu-id="e9780-108">説明</span><span class="sxs-lookup"><span data-stu-id="e9780-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9780-109">aadUserId</span><span class="sxs-lookup"><span data-stu-id="e9780-109">aadUserId</span></span>|<span data-ttu-id="e9780-110">String</span><span class="sxs-lookup"><span data-stu-id="e9780-110">String</span></span>|<span data-ttu-id="e9780-111">AAD のユーザーは、物理/マルチ account ユーザー エンティティを表すオブジェクト識別子 (GUID) をします。</span><span class="sxs-lookup"><span data-stu-id="e9780-111">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="e9780-112">accountName</span><span class="sxs-lookup"><span data-stu-id="e9780-112">accountName</span></span>|<span data-ttu-id="e9780-113">String</span><span class="sxs-lookup"><span data-stu-id="e9780-113">String</span></span>|<span data-ttu-id="e9780-114">(せずに Active Directory ドメインまたは DNS ドメイン) のユーザー アカウントのアカウント名 (とも呼ばれる`mailNickName`)。</span><span class="sxs-lookup"><span data-stu-id="e9780-114">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="e9780-115">domainName</span><span class="sxs-lookup"><span data-stu-id="e9780-115">domainName</span></span>|<span data-ttu-id="e9780-116">String</span><span class="sxs-lookup"><span data-stu-id="e9780-116">String</span></span>|<span data-ttu-id="e9780-117">ユーザー アカウント (ドメイン \ アカウントの形式は、) の NetBIOS と Active Directory ドメイン。</span><span class="sxs-lookup"><span data-stu-id="e9780-117">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="e9780-118">emailRole</span><span class="sxs-lookup"><span data-stu-id="e9780-118">emailRole</span></span>|<span data-ttu-id="e9780-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="e9780-119">emailRole</span></span>|<span data-ttu-id="e9780-120">電子メール関連のアラートをユーザー アカウントの電子メール 'ロール'。</span><span class="sxs-lookup"><span data-stu-id="e9780-120">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="e9780-121">可能な値は、`unknown`、`sender`、`recipient` です。</span><span class="sxs-lookup"><span data-stu-id="e9780-121">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="e9780-122">isVpn</span><span class="sxs-lookup"><span data-stu-id="e9780-122">isVpn</span></span>|<span data-ttu-id="e9780-123">ブール値</span><span class="sxs-lookup"><span data-stu-id="e9780-123">Boolean</span></span>|<span data-ttu-id="e9780-124">VPN 経由でユーザーをログオンするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e9780-124">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="e9780-125">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="e9780-125">logonDateTime</span></span>|<span data-ttu-id="e9780-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e9780-126">DateTimeOffset</span></span>|<span data-ttu-id="e9780-127">サインインが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="e9780-127">Time at which the sign-in occurred.</span></span> <span data-ttu-id="e9780-128">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="e9780-128">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e9780-129">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e9780-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e9780-130">logonId</span><span class="sxs-lookup"><span data-stu-id="e9780-130">logonId</span></span>|<span data-ttu-id="e9780-131">String</span><span class="sxs-lookup"><span data-stu-id="e9780-131">String</span></span>|<span data-ttu-id="e9780-132">ユーザーのサインイン ID</span><span class="sxs-lookup"><span data-stu-id="e9780-132">User sign-in ID.</span></span>|
|<span data-ttu-id="e9780-133">logonIp</span><span class="sxs-lookup"><span data-stu-id="e9780-133">logonIp</span></span>|<span data-ttu-id="e9780-134">String</span><span class="sxs-lookup"><span data-stu-id="e9780-134">String</span></span>|<span data-ttu-id="e9780-135">IP アドレスは、サインイン要求が出されたからです。</span><span class="sxs-lookup"><span data-stu-id="e9780-135">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="e9780-136">logonLocation</span><span class="sxs-lookup"><span data-stu-id="e9780-136">logonLocation</span></span>|<span data-ttu-id="e9780-137">String</span><span class="sxs-lookup"><span data-stu-id="e9780-137">String</span></span>|<span data-ttu-id="e9780-138">(IP アドレスのマッピング) によって場所がこのユーザー、ユーザーのサインインがイベントに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="e9780-138">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="e9780-139">logonType</span><span class="sxs-lookup"><span data-stu-id="e9780-139">logonType</span></span>|<span data-ttu-id="e9780-140">logonType</span><span class="sxs-lookup"><span data-stu-id="e9780-140">logonType</span></span>|<span data-ttu-id="e9780-141">ユーザーのサインインの方法です。</span><span class="sxs-lookup"><span data-stu-id="e9780-141">Method of user sign in.</span></span> <span data-ttu-id="e9780-142">使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="e9780-142">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="e9780-143">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="e9780-143">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="e9780-144">String</span><span class="sxs-lookup"><span data-stu-id="e9780-144">String</span></span>|<span data-ttu-id="e9780-145">アクティブなディレクトリ (設置型) のセキュリティ識別子 (SID) ユーザーの。</span><span class="sxs-lookup"><span data-stu-id="e9780-145">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="e9780-146">riskScore</span><span class="sxs-lookup"><span data-stu-id="e9780-146">riskScore</span></span>|<span data-ttu-id="e9780-147">String</span><span class="sxs-lookup"><span data-stu-id="e9780-147">String</span></span>|<span data-ttu-id="e9780-148">ユーザー アカウントのプロバイダーによって生成されると計算されるリスク ・ スコアです。</span><span class="sxs-lookup"><span data-stu-id="e9780-148">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="e9780-149">0 - 1 パーセントに相当する値の範囲をお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e9780-149">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="e9780-150">userAccountType</span><span class="sxs-lookup"><span data-stu-id="e9780-150">userAccountType</span></span>|<span data-ttu-id="e9780-151">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="e9780-151">userAccountSecurityType</span></span>|<span data-ttu-id="e9780-152">ユーザー アカウントの種類 (グループ) は、Windows の定義ごと。</span><span class="sxs-lookup"><span data-stu-id="e9780-152">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="e9780-153">可能な値は、`unknown`、`standard`、`power`、`administrator` です。</span><span class="sxs-lookup"><span data-stu-id="e9780-153">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="e9780-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e9780-154">userPrincipalName</span></span>|<span data-ttu-id="e9780-155">String</span><span class="sxs-lookup"><span data-stu-id="e9780-155">String</span></span>|<span data-ttu-id="e9780-156">ユーザー サインイン名をインターネット形式: (ユーザー アカウント名) @(ユーザー アカウントの DNS ドメイン名) です。</span><span class="sxs-lookup"><span data-stu-id="e9780-156">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9780-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9780-157">JSON representation</span></span>

<span data-ttu-id="e9780-158">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9780-158">The following is a JSON representation of the resource.</span></span>

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
