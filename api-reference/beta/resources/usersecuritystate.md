---
title: userSecurityState リソースの種類
description: " > **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。"
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3c0f9cb91484f23702329a38de26189176dacb13
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964236"
---
# <a name="usersecuritystate-resource-type"></a><span data-ttu-id="e971c-104">userSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e971c-104">userSecurityState resource type</span></span>

 [!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e971c-105">ユーザーアカウントに関するステートフルな情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="e971c-105">Contains stateful information about the user account.</span></span>

## <a name="properties"></a><span data-ttu-id="e971c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e971c-106">Properties</span></span>

| <span data-ttu-id="e971c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e971c-107">Property</span></span>   | <span data-ttu-id="e971c-108">型</span><span class="sxs-lookup"><span data-stu-id="e971c-108">Type</span></span> |<span data-ttu-id="e971c-109">説明</span><span class="sxs-lookup"><span data-stu-id="e971c-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e971c-110">Usersecuritystate</span><span class="sxs-lookup"><span data-stu-id="e971c-110">aadUserId</span></span>|<span data-ttu-id="e971c-111">String</span><span class="sxs-lookup"><span data-stu-id="e971c-111">String</span></span>|<span data-ttu-id="e971c-112">AAD User オブジェクト識別子 (GUID)-物理/マルチアカウントユーザーエンティティを表します。</span><span class="sxs-lookup"><span data-stu-id="e971c-112">AAD User object identifier (GUID) - represents the physical/multi-account user entity.</span></span>|
|<span data-ttu-id="e971c-113">accountName</span><span class="sxs-lookup"><span data-stu-id="e971c-113">accountName</span></span>|<span data-ttu-id="e971c-114">String</span><span class="sxs-lookup"><span data-stu-id="e971c-114">String</span></span>|<span data-ttu-id="e971c-115">ユーザーアカウントのアカウント名 (Active Directory ドメインまたは DNS ドメインなし)-(と`mailNickName`も呼ばれます)。</span><span class="sxs-lookup"><span data-stu-id="e971c-115">Account name of user account (without Active Directory domain or DNS domain) - (also called `mailNickName`).</span></span>|
|<span data-ttu-id="e971c-116">domainName</span><span class="sxs-lookup"><span data-stu-id="e971c-116">domainName</span></span>|<span data-ttu-id="e971c-117">String</span><span class="sxs-lookup"><span data-stu-id="e971c-117">String</span></span>|<span data-ttu-id="e971c-118">ユーザーアカウントの NetBIOS/Active Directory ドメイン (つまり、"ドメイン \ ユーザー名" の形式)。</span><span class="sxs-lookup"><span data-stu-id="e971c-118">NetBIOS/Active Directory domain of user account (that is, domain\account format).</span></span>|
|<span data-ttu-id="e971c-119">emailRole</span><span class="sxs-lookup"><span data-stu-id="e971c-119">emailRole</span></span>|<span data-ttu-id="e971c-120">emailRole</span><span class="sxs-lookup"><span data-stu-id="e971c-120">emailRole</span></span>|<span data-ttu-id="e971c-121">電子メール関連の警告の場合-ユーザーアカウントの電子メール ' ロール '。</span><span class="sxs-lookup"><span data-stu-id="e971c-121">For email-related alerts - user account's email 'role'.</span></span> <span data-ttu-id="e971c-122">可能な値は、`unknown`、`sender`、`recipient` です。</span><span class="sxs-lookup"><span data-stu-id="e971c-122">Possible values are: `unknown`, `sender`, `recipient`.</span></span>|
|<span data-ttu-id="e971c-123">isVpn</span><span class="sxs-lookup"><span data-stu-id="e971c-123">isVpn</span></span>|<span data-ttu-id="e971c-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="e971c-124">Boolean</span></span>|<span data-ttu-id="e971c-125">ユーザーが VPN を介してログオンしたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e971c-125">Indicates whether the user logged on through a VPN.</span></span>|
|<span data-ttu-id="e971c-126">logonDateTime</span><span class="sxs-lookup"><span data-stu-id="e971c-126">logonDateTime</span></span>|<span data-ttu-id="e971c-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e971c-127">DateTimeOffset</span></span>|<span data-ttu-id="e971c-128">サインインが発生した時刻。</span><span class="sxs-lookup"><span data-stu-id="e971c-128">Time at which the sign-in occurred.</span></span> <span data-ttu-id="e971c-129">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="e971c-129">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e971c-130">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e971c-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="e971c-131">logonId</span><span class="sxs-lookup"><span data-stu-id="e971c-131">logonId</span></span>|<span data-ttu-id="e971c-132">String</span><span class="sxs-lookup"><span data-stu-id="e971c-132">String</span></span>|<span data-ttu-id="e971c-133">ユーザーのサインイン ID。</span><span class="sxs-lookup"><span data-stu-id="e971c-133">User sign-in ID.</span></span>|
|<span data-ttu-id="e971c-134">logonIp</span><span class="sxs-lookup"><span data-stu-id="e971c-134">logonIp</span></span>|<span data-ttu-id="e971c-135">String</span><span class="sxs-lookup"><span data-stu-id="e971c-135">String</span></span>|<span data-ttu-id="e971c-136">サインイン要求の送信元の IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="e971c-136">IP Address the sign-in request originated from.</span></span>|
|<span data-ttu-id="e971c-137">logonLocation</span><span class="sxs-lookup"><span data-stu-id="e971c-137">logonLocation</span></span>|<span data-ttu-id="e971c-138">String</span><span class="sxs-lookup"><span data-stu-id="e971c-138">String</span></span>|<span data-ttu-id="e971c-139">このユーザーによってユーザーのサインインイベントに関連付けられている場所 (IP アドレスマッピング)。</span><span class="sxs-lookup"><span data-stu-id="e971c-139">Location (by IP address mapping) associated with a user sign-in event by this user.</span></span>|
|<span data-ttu-id="e971c-140">logonType</span><span class="sxs-lookup"><span data-stu-id="e971c-140">logonType</span></span>|<span data-ttu-id="e971c-141">logonType</span><span class="sxs-lookup"><span data-stu-id="e971c-141">logonType</span></span>|<span data-ttu-id="e971c-142">ユーザーのサインイン方法。</span><span class="sxs-lookup"><span data-stu-id="e971c-142">Method of user sign in.</span></span> <span data-ttu-id="e971c-143">使用可能な値: `unknown`、`interactive`、`remoteInteractive`、`network`、`batch`、`service`。</span><span class="sxs-lookup"><span data-stu-id="e971c-143">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|
|<span data-ttu-id="e971c-144">onPremisesSecurityIdentifier</span><span class="sxs-lookup"><span data-stu-id="e971c-144">onPremisesSecurityIdentifier</span></span>|<span data-ttu-id="e971c-145">String</span><span class="sxs-lookup"><span data-stu-id="e971c-145">String</span></span>|<span data-ttu-id="e971c-146">ユーザーの Active Directory (社内) セキュリティ識別子 (SID)。</span><span class="sxs-lookup"><span data-stu-id="e971c-146">Active Directory (on-premises) Security Identifier (SID) of the user.</span></span>|
|<span data-ttu-id="e971c-147">riskScore</span><span class="sxs-lookup"><span data-stu-id="e971c-147">riskScore</span></span>|<span data-ttu-id="e971c-148">String</span><span class="sxs-lookup"><span data-stu-id="e971c-148">String</span></span>|<span data-ttu-id="e971c-149">ユーザーアカウントのプロバイダーが生成/計算したリスクスコア。</span><span class="sxs-lookup"><span data-stu-id="e971c-149">Provider-generated/calculated risk score of the user account.</span></span> <span data-ttu-id="e971c-150">推奨値の範囲0-1。パーセンテージに相当します。</span><span class="sxs-lookup"><span data-stu-id="e971c-150">Recommended value range of 0-1, which equates to a percentage.</span></span>|
|<span data-ttu-id="e971c-151">userAccountType</span><span class="sxs-lookup"><span data-stu-id="e971c-151">userAccountType</span></span>|<span data-ttu-id="e971c-152">userAccountSecurityType</span><span class="sxs-lookup"><span data-stu-id="e971c-152">userAccountSecurityType</span></span>|<span data-ttu-id="e971c-153">ユーザーアカウントの種類 (グループメンバーシップ) (Windows 定義あたり)。</span><span class="sxs-lookup"><span data-stu-id="e971c-153">User account type (group membership), per Windows definition.</span></span> <span data-ttu-id="e971c-154">使用可能な値は、`unknown`、`standard`、`power`、`administrator` です。</span><span class="sxs-lookup"><span data-stu-id="e971c-154">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="e971c-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e971c-155">userPrincipalName</span></span>|<span data-ttu-id="e971c-156">String</span><span class="sxs-lookup"><span data-stu-id="e971c-156">String</span></span>|<span data-ttu-id="e971c-157">ユーザーのサインイン名-インターネット形式: (ユーザーアカウント名) @ (ユーザーアカウントの DNS ドメイン名)。</span><span class="sxs-lookup"><span data-stu-id="e971c-157">User sign-in name - internet format: (user account name)@(user account DNS domain name).</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e971c-158">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e971c-158">JSON representation</span></span>

<span data-ttu-id="e971c-159">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e971c-159">The following is a JSON representation of the resource.</span></span>

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
