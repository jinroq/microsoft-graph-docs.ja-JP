---
title: usersecuritystate リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7ca02b6582898e8a0184c6c37115c9ac96b386ff
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345089"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="56aff-104">usersecuritystate リソースの種類</span><span class="sxs-lookup"><span data-stu-id="56aff-104">userSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56aff-105">ユーザーアカウントに関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="56aff-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="56aff-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56aff-106">Properties</span></span>

| <span data-ttu-id="56aff-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56aff-107">Property</span></span>   | <span data-ttu-id="56aff-108">型</span><span class="sxs-lookup"><span data-stu-id="56aff-108">Type</span></span> |<span data-ttu-id="56aff-109">説明</span><span class="sxs-lookup"><span data-stu-id="56aff-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="56aff-110">usersecuritystate</span><span class="sxs-lookup"><span data-stu-id="56aff-110">aadUserId</span></span>|<span data-ttu-id="56aff-111">String</span><span class="sxs-lookup"><span data-stu-id="56aff-111">String</span></span>|<span data-ttu-id="56aff-112">AAD user オブジェクト識別子 (GUID)-物理/マルチアカウントユーザーエンティティを表します。</span><span class="sxs-lookup"><span data-stu-id="56aff-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="56aff-113">accountName</span><span class="sxs-lookup"><span data-stu-id="56aff-113">accountName</span></span>|<span data-ttu-id="56aff-114">String</span><span class="sxs-lookup"><span data-stu-id="56aff-114">String</span></span>|<span data-ttu-id="56aff-115">ユーザーアカウントのアカウント名 (Active Directory ドメインまたは DNS ドメインなし)-(と`mailNickName`も呼ばれます)。</span><span class="sxs-lookup"><span data-stu-id="56aff-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="56aff-116">domainName</span><span class="sxs-lookup"><span data-stu-id="56aff-116">domainName</span></span>|<span data-ttu-id="56aff-117">String</span><span class="sxs-lookup"><span data-stu-id="56aff-117">String</span></span>|<span data-ttu-id="56aff-118">ユーザーアカウントの NetBIOS/Active Directory ドメイン (つまり、"ドメイン \ ユーザー名" の形式)。</span><span class="sxs-lookup"><span data-stu-id="56aff-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="56aff-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="56aff-119">emailRole</span></span>|<span data-ttu-id="56aff-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="56aff-120">emailRole</span></span>|<span data-ttu-id="56aff-121">電子メール関連の警告の場合-ユーザーアカウントの電子メール ' ロール '。</span><span class="sxs-lookup"><span data-stu-id="56aff-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="56aff-122">可能な値は、`unknown`、`sender`、`recipient` です。</span><span class="sxs-lookup"><span data-stu-id="56aff-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="56aff-123">isvpn</span><span class="sxs-lookup"><span data-stu-id="56aff-123">isVpn</span></span>|<span data-ttu-id="56aff-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="56aff-124">Boolean</span></span>|<span data-ttu-id="56aff-125">ユーザーが VPN を介してログオンしたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="56aff-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="56aff-126">logondatetime</span><span class="sxs-lookup"><span data-stu-id="56aff-126">logonDateTime</span></span>|<span data-ttu-id="56aff-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="56aff-127">DateTimeOffset</span></span>|<span data-ttu-id="56aff-128">サインインが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="56aff-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="56aff-129">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="56aff-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="56aff-130">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、`'2014-01-01T00:00:00Z'` のようになります。</span><span class="sxs-lookup"><span data-stu-id="56aff-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="56aff-131">logonId</span><span class="sxs-lookup"><span data-stu-id="56aff-131">logonId</span></span>|<span data-ttu-id="56aff-132">String</span><span class="sxs-lookup"><span data-stu-id="56aff-132">String</span></span>|<span data-ttu-id="56aff-133">ユーザーのサインイン ID。</span><span class="sxs-lookup"><span data-stu-id="56aff-133">User sign-in ID.</span></span>|
|<span data-ttu-id="56aff-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="56aff-134">logonIp</span></span>|<span data-ttu-id="56aff-135">String</span><span class="sxs-lookup"><span data-stu-id="56aff-135">String</span></span>|<span data-ttu-id="56aff-136">サインイン要求の送信元の IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="56aff-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="56aff-137">logonlocation</span><span class="sxs-lookup"><span data-stu-id="56aff-137">logonLocation</span></span>|<span data-ttu-id="56aff-138">String</span><span class="sxs-lookup"><span data-stu-id="56aff-138">String</span></span>|<span data-ttu-id="56aff-139">このユーザーによってユーザーのサインインイベントに関連付けられている場所 (IP アドレスマッピング)。</span><span class="sxs-lookup"><span data-stu-id="56aff-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="56aff-140">logonType</span><span class="sxs-lookup"><span data-stu-id="56aff-140">logonType</span></span>|<span data-ttu-id="56aff-141">logonType</span><span class="sxs-lookup"><span data-stu-id="56aff-141">logonType</span></span>|<span data-ttu-id="56aff-142">ユーザーのサインイン方法。</span><span class="sxs-lookup"><span data-stu-id="56aff-142">Method of user sign in.</span></span> <span data-ttu-id="56aff-143">使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="56aff-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="56aff-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="56aff-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="56aff-145">String</span><span class="sxs-lookup"><span data-stu-id="56aff-145">String</span></span>|<span data-ttu-id="56aff-146">ユーザーの Active Directory (社内) セキュリティ識別子 (SID)。</span><span class="sxs-lookup"><span data-stu-id="56aff-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="56aff-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="56aff-147">riskScore</span></span>|<span data-ttu-id="56aff-148">String</span><span class="sxs-lookup"><span data-stu-id="56aff-148">String</span></span>|<span data-ttu-id="56aff-149">ユーザーアカウントのプロバイダーが生成/計算したリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="56aff-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="56aff-150">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="56aff-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="56aff-151">userAccountType</span><span class="sxs-lookup"><span data-stu-id="56aff-151">userAccountType</span></span>|<span data-ttu-id="56aff-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="56aff-152">userAccountSecurityType</span></span>|<span data-ttu-id="56aff-153">ユーザーアカウントの種類 (グループメンバーシップ) (Windows 定義あたり)。</span><span class="sxs-lookup"><span data-stu-id="56aff-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="56aff-154">使用可能な値は、`unknown`、`standard`、`power`、`administrator` です。</span><span class="sxs-lookup"><span data-stu-id="56aff-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="56aff-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="56aff-155">userPrincipalName</span></span>|<span data-ttu-id="56aff-156">String</span><span class="sxs-lookup"><span data-stu-id="56aff-156">String</span></span>|<span data-ttu-id="56aff-157">ユーザーのサインイン名-インターネット形式: (ユーザーアカウント名) @ (ユーザーアカウントの DNS ドメイン名)。</span><span class="sxs-lookup"><span data-stu-id="56aff-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56aff-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="56aff-158">JSON representation</span></span>

<span data-ttu-id="56aff-159">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="56aff-159">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "userSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
